<!--
author: Christian Golnik

import: https://raw.githubusercontent.com/LiaScript/CodeRunner/master/README.md

-->

# Copy to clipboard

__Generator-Aufgabe:__<br> Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Generators.
<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Generators. Ich gebe dir meine Antwort im folgenden Prompt. Bitte bewerte meine Antwort auf seine Richtigkeit. Nutze als Formelzeichen für die Spannung U.</span>
</div>

<script input="submit" style="margin-left:10%"  default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

