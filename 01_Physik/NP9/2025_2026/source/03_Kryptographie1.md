<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg 

logo: https://www.projektmagazin.de/sites/default/files/inline-images/4-seiten-einer-nachricht.JPG

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

mode: textbook

@onload
window.LIA.settings.font_size = 2
@end

@color
<bdi style="color:@1">@0</bdi>
@end

-->

# MUZ GAT NETUG 

<H3> THCIRRETNUEIHPARGOTPYRK </H3>

## Caesar - Verschlüsselung

__Übung:__

Verschüssele mit (Schlüssel +4) __FEUER__: Lösung : [[JIYIV]]

Entschlüssele mit (Schlüssel +4) __DMVOYW__: Lösung: [[ZIRKUS]]

Verschlüssle das Wort __GLADIATOREN__ mit Schlüssel 7: Lösung [[NSHKPHAVYLU]].


## 2. Gartenzaunmethode

Entschlüssele mit dem Gartenzaun: __MINM ITAE ENAE SHS__

Lösung (Großbuchstaben, ohne Leerzeichen): [[MEINNAMEISTHASE]]

Entschlüssele mit dem doppelten Gartenzaun: __SONT NEND RIHS IIEC E__

Lösung (Großbuchstaben, ohne Leerzeichen): [[SEINODERNICHTSEIN]]

## 3. Vignere Verschlüsselung

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
