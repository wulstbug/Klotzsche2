
<!--
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

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->


# Aufgaben Nawi Profil 9 - Arbeit zu Hause

# Das vier Ohren-Modell nach F. Schulz von Thun

Schau dir folgendes Video an. Notiere in Stichpunkten die Inhalte des _Vier-Ohren-Modells_ nach Friedemann Schulz von Thun

!?[4OhremModellAlphaLErnen](https://www.youtube.com/watch?v=9VJn1cPbf1A)

# KI-Gespräch

Führe ein Gespräch mit einer KI. Z.B. Olympia, Hobbies, die Wahlen, Krieg, Freunschaft oder etwas deiner Wahl.

[ogy.de/gykl-ki](https://go.fobizz.com/?token=d29d855d3e33da30)

Speichere dein Gespräch als Word-Datei oder PDF. Lege es hier mit deinem Vornamen ab:

https://diversewolken.ddns.net/nextcloud/index.php/s/bTY3iNb6xjpZk6Q

# Aufbau des Internets

Schau dir folgendes Video an und notiere die wesentlichen Meilensteine, welche zum Erfolg des Internets geführt haben.

!?[EntwicklungDesInternets](https://www.youtube.com/watch?v=EKm6pJSI-aQ)

# MUZ GAT NETUG 

<H3> THCIRRETNUEIHPARGOTPYRK </H3>

# Grundlagen Verschlüsselung

Schau dir folgende Videos an zum Thema Verschlüsselung. Das Tafelbild mit den Grundlagen wird später eingefügt.

!?[Verschüsselung](https://www.youtube.com/watch?v=WaPwvaQQZjU)

!?[VerschüsselungEMail](https://www.youtube.com/watch?v=inxNRA4xK1Q)

Tafelbild verschlüsselte Kommunikation

![Tafelbild_Verschlüsselung](https://diversewolken.ddns.net/nextcloud/index.php/s/MsxAqHnd7iwMCZs/download)

# Einführung Verschlüsselung

## 1. Caesar Verschlüsselung

{{1}}
*************
Nimm jeden Buchstaben des Wortes und verschiebe ihn um eine feste Anzahl an Stellen im Alphabet (klassisch +3).

![CaesarErklärt](https://assets.serlo.org/dc09c860-3828-11ee-b962-1fa7d97ba81a/CaesarVerschlsselung.svg)
*************

{{2}}
************
> Aus dem Wort __BESEN__ wird das Wort [[EHVHQ]].
************


{{3}}
********

__Übung:__

Verschüssele mit (Schlüssel +4) __FEUER__: Lösung : [[JIYIV]]

Entschlüssele mit (Schlüssel +4) __DMVOYW__: Lösung: [[ZIRKUS]]

Verschlüssle das Wort __GLADIATOREN__ mit Schlüssel 7: Lösung [[NSHKPHAVYLU]].

************



## 2. Gartenzaunmethode

![Tafelbild_Gartenzaun](https://diversewolken.ddns.net/nextcloud/index.php/s/oJj2xDnRGEwSLpp/download)

Entschlüssele mit dem Gartenzaun: __MINM ITAE ENAE SHS__

Lösung (Großbuchstaben, ohne Leerzeichen): [[MEINNAMEISTHASE]]

Entschlüssele mit dem doppelten Gartenzaun: __SONT NEND RIHS IIEC C__

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

