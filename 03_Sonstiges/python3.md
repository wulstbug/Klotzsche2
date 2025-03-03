<!--
author: Christian Golnik

import: https://raw.githubusercontent.com/LiaScript/CodeRunner/master/README.md

-->

# Vigenere Verschlüsselung

```text +data.txt
TEXT: ABC
PASSWORT: ABC
```
``` python -vignere.py
def vigenere_encrypt(text: str, key: str) -> str:
    text = text.upper()
    key = key.upper()
    alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
    encrypted_text = ""
    key_length = len(key)
    
    for i, char in enumerate(text):
        if char in alphabet:
            text_index = alphabet.index(char)  # Convert char to number (0-based index)
            key_index = alphabet.index(key[i % key_length])  # Repeat key cyclically
            new_index = (text_index + key_index + 1) % 26  # Apply Vigenère shift (1-based indexing)
            encrypted_text += alphabet[new_index]
        else:
            encrypted_text += char  # Preserve non-alphabetic characters

        # Insert space every 4 characters
        formatted_text = " ".join([encrypted_text[i:i+4] for i in range(0, len(encrypted_text), 4)])

    return formatted_text

with open("data.txt", 'r') as file:
    lines = file.readlines()
    text1 = lines[0].strip().replace("TEXT: ", "")
    password1 = lines[1].strip().replace("PASSWORT: ", "")

formatted_text = " ".join([text1[i:i+4] for i in range(0, len(text1), 4)])

formatted_pass = " ".join([password1[i:i+4] for i in range(0, len(password1), 4)])

print ("TEXT:\t\t\t", formatted_text)
print ("PASSWORT:\t\t", formatted_pass)
print("Verschlüsselung:\t", vigenere_encrypt(text1, password1))
```
@LIA.eval(`["data.txt", "main.py"]`, `none`, `python3 main.py`)

# Vignere-JavaScript (Verschlüsseln)

<!-- style="background-color:coral"-->
| | |
| <label for="text">Text:</label> | <input type="text" id="text"> |
| <label for="password">Passwort:</label> | <input type="text" id="password"> |
| <label for="encr"> Verschlüsselter Text:</label> | <span id="output"></span> |

<script input="button">
    function vigenereEncrypt(text, key) {
        if (key.length === 0)
        return "";        
        else
            text = text.toUpperCase().replace(/[^A-Z]/g, "");
            document.getElementById("text").value = text.match(/.{1,4}/g).join(" ");
            key = key.toUpperCase().replace(/[^A-Z]/g, "");
            document.getElementById("password").value = key;
        
        let encryptedText = "";
        let keyIndex = 0;        
        for (let i = 0; i < text.length; i++) {
            let textChar = text.charCodeAt(i) - 64;
            let keyChar = key.charCodeAt(keyIndex % key.length) - 64;
            let encryptedChar = ((textChar + keyChar - 1) % 26) + 1;
            encryptedText += String.fromCharCode(encryptedChar + 64);
            keyIndex++;
        }        
        return encryptedText.match(/.{1,4}/g).join(" ");
    }
    function encrypt() {
        let text = document.getElementById("text").value;
        let password = document.getElementById("password").value;
        let encrypted = vigenereEncrypt(text, password);
        document.getElementById("output").innerText = encrypted;
    }
    encrypt();
    
    "Verschlüsseln"
</script>

# Vignere-JavaScript (Entschlüsseln)

<!-- style="background-color:coral"-->
| | |
| <label for="encr">Verschlüsserlter Text:</label> | <input type="text" id="encr"> |
| <label for="password">Passwort:</label> | <input type="text" id="password"> |
| <label for="encr"> Entschlüsselter Text:</label> | <span id="output"></span> |
<script input="button">
    function vigenereDecrypt(ciphertext, key) {
        const alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        let plaintext = "";
        let keyIndex = 0;
        ciphertext = ciphertext.toUpperCase();
        key = key.toUpperCase();

        for (let i = 0; i < ciphertext.length; i++) {
            let cipherChar = ciphertext[i];
            if (alphabet.includes(cipherChar)) {
                let shift = alphabet.indexOf(key[keyIndex % key.length]);
                let plainIndex = (alphabet.indexOf(cipherChar) - shift + 26-1) % 26;
                plaintext += alphabet[plainIndex];
                keyIndex++;
            } else {
                plaintext += cipherChar;
            }
        }
        return plaintext;
    }
    function decrypt() {
        let encrtext = document.getElementById("encr").value;
        let password = document.getElementById("password").value;
        let decrypted = vigenereDecrypt(encrtext, password);
        document.getElementById("output").innerText = decrypted;
    }
    decrypt();

    "Entschlüsseln"
</script>

# Vignere-JavaScript (Check)

<!-- style="background-color:coral"-->
| | |
| <label for="text">Entschlüsselter Text:</label> | <input type="text" id="decr"> |
| <label for="password">Passwort:</label> | <input type="text" id="password"> |
| <label for="encr"> Verschlüsselter Text:</label> | <input type="text" id="encr"> |
<script input="button">
    function vigenereEncrypt(text, key) {
        if (key.length === 0)
            return "CHECK";        
        else
            text = text.toUpperCase().replace(/[^A-Z]/g, "");
            key = key.toUpperCase().replace(/[^A-Z]/g, "");
        
        let encryptedText = "";
        let keyIndex = 0;        
        for (let i = 0; i < text.length; i++) {
            let textChar = text.charCodeAt(i) - 64;
            let keyChar = key.charCodeAt(keyIndex % key.length) - 64;
            let encryptedChar = ((textChar + keyChar - 1) % 26) + 1;
            encryptedText += String.fromCharCode(encryptedChar + 64);
            keyIndex++;
        }        
        return encryptedText;
    }
    function encrypt() {
        let decr = document.getElementById("decr").value;
        let password = document.getElementById("password").value;
        let encr = document.getElementById("encr").value;
        let encr_check = vigenereEncrypt(decr, password);

        if (decr.length === 0 || password.length === 0 || encr.length === 0)
            return "Check"
        else
            if (encr === encr_check)
                return "Richtig"
            else
                return "Falsch"
    }
    encrypt();
</script>