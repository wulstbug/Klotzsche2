<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg 

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/EmwDHWSC3pwJq4f/download

author: Christian Golnik

language: de

@style
.lia-effect__circle {
    display: none !important;
}

@media (min-width: 600px) {
    .newspaper {
        column-count: 2;
        column-gap: 40px;
        column-rule: 1px solid lightblue;
    }
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
}
@end

mode: presentation

@onload
window.LIA.settings.font_size = 2
@end

@color
<bdi style="color:@1">@0</bdi>
@end

-->

# Passwortverschlüsselung (Vigneré Verschlüsselung)

> Löse die Aufgaben 1. - 3. (Pfeiltaste nach rechtsdai)


## 1. Übung Caesar - Verschlüsselung

__Übung:__

1. Entschlüssele mit (Schlüssel +3) __EDXPKDXV__: Lösung: [[BAUMHAUS]]

2. Entschlüssle das Wort __NSHKPHAVYLU__ mit Schlüssel 7: Lösung [[GLADIATOREN]]

3. Verschlüssele das Wort __TRAUM__ mit Schlüsser 3: Lösung: [[WUDXP]]

4. Entschlüssele das Wort __DSIHO__ mit Schlüssel 3: Lösung: [APFEL]]


## 2. Übung Gartenzaunmethode

1. Entschlüssele mit dem Gartenzaun: __HXNUKLEEBCE__

     Lösung (Großbuchstaben, ohne Leerzeichen): [[HEXENBUCKEL]]

2. Entschlüssele mit dem doppelten Gartenzaun: __HFSFEEERUHUDRULTRRCNAS__

     Lösung (Großbuchstaben, ohne Leerzeichen): [[HERRFUCHSUNDFRAUELSTER]]

3. Verschlüssele mit dem Gartenzaun: SCHEUERHADER

     Lösung (Großbuchstaben, ohne Leerzeichen): [[SHURAECEEHDR]]

4. Entschlüssele mit dem Gartenzaun: SHETRIGCMTELN

     Lösung (Großbuchstaben, ohne Leerzeichen): [[SCHMETTERLING]]


## 3. Übung Entschlüsseln mit Enigma

> Öffne die App Mininigma auf dem Tablet

1. Nutze die Walzenstellung: __F Z P__

Entschlüssele den folgenden Text: __WNQV VCQW ODCX VAKR BUER__

[[SAMM ELPU NKTI STQF UENF]]

2. Nutze die Walzenstellung: __H X Z__

zunächst wurde die Walzenstellung verschlüsselt: Verschlüssele __XPM__

Nutze den verschlüsselten Text als Walzeneinstellung.

Zwischenlösung: [[EQW]]

Entschlüssele anschließend den folgenden Text: __BUZR GZZI UAKN ZACF YLHU CDRK Z__

Ergebnis: [[NACH SCHU BFUE RGRU PPES IEBE N]]

## 4.1 Vigenere Verschlüsselung - Erklärung zum Lesen


![Tabelle](https://diversewolken.ddns.net/nextcloud/index.php/s/9e6RB6rCAfd73nx/download)

Wähle einen Text und einen Schlüssel. <br> {1}{z.B. Text: __HEXEN__ <br> Schlüssel: __ABC__}

{{2-3}}
**************
1. Ordne jedem Buchstaben des Textes die entsprechende Zahl (Position) im Alphabet zu.

| | | | | |
| H | E | X | E | N |
| 8 | 5 | 24 | 5 | 14 |
*************

{{3-4}}
***********
1. Ordne jedem Buchstaben des Textes die entsprechende Zahl (Position) im Alphabet zu. <br>
2. Ordne jedem Buchstaben des Schlüssels die entsprechende Zahl (Position) im Alphabet zu, wiederhole des Schlüssel von vorn, wenn er zu kurz ist.

| | | | | |
| H | E | X | E | N |
| 8 | 5 | 24 | 5 | 14 |
| A | B | C | A | B |
| 1 | 2 | 3 | 1 | 2 |
*************

{{4-5}}
*************
1. Ordne jedem Buchstaben des Textes die entsprechende Zahl (Position) im Alphabet zu. <br>
2. Ordne jedem Buchstaben des Schlüssels die entsprechende Zahl (Position) im Alphabet zu, wiederhole des Schlüssel von vorn, wenn er zu kurz ist.
3. Addiere die aufgeschriebenen Zahlen.

| | | | | |
| H | E | X | E | N |
| 8 | 5 | 24 | 5 | 14 |
| A | B | C | A | B |
| +1 | +2 | +3 | +1 | +2 |
|---|---|---|---|---|
| 9 | 7 | 27 | 6 | 16|
*************

{{5-6}}
*************
1. Ordne jedem Buchstaben des Textes die entsprechende Zahl (Position) im Alphabet zu. <br>
2. Ordne jedem Buchstaben des Schlüssels die entsprechende Zahl (Position) im Alphabet zu, wiederhole des Schlüssel von vorn, wenn er zu kurz ist.
3. Addiere die aufgeschriebenen Zahlen.
4. Subtrahiere 26, wenn der Wert größer als 26 ist.

| | | | | |
| H | E | X | E | N |
| 8 | 5 | 24 | 5 | 14 |
| A | B | C | A | B |
| +1 | +2 | +3 | +1 | +2 |
|---|---|---|---|---|
| 9 | 7 | 27-26=1 | 6 | 16|
*************


{{6}}
*************
1. Ordne jedem Buchstaben des Textes die entsprechende Zahl (Position) im Alphabet zu. <br>
2. Ordne jedem Buchstaben des Schlüssels die entsprechende Zahl (Position) im Alphabet zu, wiederhole des Schlüssel von vorn, wenn er zu kurz ist.
3. Addiere die aufgeschriebenen Zahlen.
4. Subtrahiere 26, wenn der Wert größer als 26 ist.
5. Übersetze die berechneten Zahlen in den verschlüsselten Text.

| | | | | |
| H | E | X | E | N |
| 8 | 5 | 24 | 5 | 14 |
| A | B | C | A | B |
| +1 | +2 | +3 | +1 | +2 |
| __I__ | __G__ | __A__ | __F__ | __P__ |
| 9 | 7 | 1 | 6 | 16 |
*************

{{7}}
*************
Verschlüsselter Text: __IGAFP__
*************


## 4.2 Vigenere Verschlüsselung - Zum Üben

![Tabelle](https://diversewolken.ddns.net/nextcloud/index.php/s/9e6RB6rCAfd73nx/download)

__Aufgaben:__

1. Verschlüssele den Text __HUHN__ mit dem Passwort __EI__:

     [[ MDMW ]]

2. Verschlüssele den Text __LIEBLINGSESSEN__ mit dem Passwort __BURGER__:

     [[ NDWIQAPBKLXKGI ]]

3. Verschlüssele das Wort __ABITURPRUEFUNG__ mit dem Passwort __GYM__

     [[ HAVATEWQHLEHUF ]]

4. Entschlüssle den Text __NZFHWXPJKZ__ mit dem Passwort __GESUND__:

     [[ GUMMITIERE ]]

5. Entschlüssele das Wort __SFAWMHLFDQ__ mit dem Passwort __LEICHT__

     [[ GARTENZAUN ]]

6. Finde das Passwort für den unverschlüsselten Text __KATZENFUTTER__ und den verschlüsselten Text __XBOS ROAN GUZK__ 

     [[ MAUS ]]