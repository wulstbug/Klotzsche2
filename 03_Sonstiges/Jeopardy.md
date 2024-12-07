<!--
author: Christian Golnik

language: de

@style
.lia-effect__circle {
    display: none !important;
}
.lia-slide__footer {
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

@onload
window.LIA.settings.font_size = 2
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@uhr

<div style="position: fixed; right:50px; top:100px;">

<details>

<summary> Uhrzeit </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=de&size=large&timezone=Europe%2FBerlin" width="100%" height="150" frameborder="0" seamless></iframe> 

</div>

</details>

</div>

@end

@timer

<div style="position: fixed; right:50px; top:100px;">

<details>

<summary> Timer(@0:@1) </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe width="200" height="90" src="https://webuhr.de/embed/timer/#countdown=00:@0:@1&enabled=0&onzero=0&theme=0&ampm=0&sound=xylophone" frameborder="0" allowfullscreen>

</iframe> 

</div>

</details>

</div>

@end

@K1
Aufbau
@end

@K2
Anwendung
@end

@K3
Experiment
@end


@@@ ogy.de/11Ph2 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Jeopardy

## Übersicht

Dieses Spiel basiert auf dem Prinzip des beliebten Spiels "Jeopardy". Teilnehmer beantworten Fragen aus verschiedenen Kategorien und sammeln Punkte.

## Kategorien

| | | |
| @K1 | @K2 | @K3 |
| [200](#5) | [200](#9)   | [200](#13) |
| [400](#6) | [400](#10)  | [400](#14) |
| [600](#7) | [600](#11)  | [600](#15) |
| [800](#8) | [800](#12)  | [800](#16) |


---

## Spielablauf

- Jede Runde wird eine Frage ausgewählt → eine feste Person.
- Niemand antwortet zwei Mal.
- Falsche Antwort → anderes Team kann die Hälfte der Punkte stehlen.
- Kurze Diskussionen sind erlaubt.

[Zurück zur Übersicht](#übersicht)

---

## @K1 200 Punkte
- Was bedeutet das Formelzeichen **Nₚ**?  
[Zurück zu den Punkten](#Kategorien)

---

## @K1 400 Punkte
- Auf welcher Gesetzmäßigkeit beruht die Umwandlung der Primärspannung auf den Sekundärstromkreis?  
[Zurück zu den Punkten](#Kategorien)

---

## @K1 600 Punkte
- John will mit dem folgenden Aufbau eine Spannungsuntersetzung von 200 V auf 100 V erreichen. In Johns Schaltung stecken Fehler. Finde zwei dieser Fehler.  
[Zurück zu den Punkten](#Kategorien)

---

## @K1 800 Punkte
- Man wickelt die Primär- und Sekundärwicklung um den gleichen Eisenkern. Welcher Aufbau würde als Transformator fungieren?  
[Zurück zu den Punkten](#Kategorien)

---

## @K2 200 Punkte
- Wie erfolgt die Spannungsumwandlung bei einem realen Transformator?  
[Zurück zu den Punkten](#Kategorien)

---

## @K2 400 Punkte
- Was bedeutet Heruntertransformieren?  
[Zurück zu den Punkten](#Kategorien)

---

## @K2 600 Punkte
- Die Windungszahl **Nₛ** eines idealen Transformators ist das Fünffache von **Nₚ**. Stelle eine Gleichung auf, in welcher die Beziehung der Spannungen dargestellt wird.  
[Zurück zu den Punkten](#Kategorien)

---

## @K2 800 Punkte
- Zwischen welchen Spannungen wird bei einem Umspannwerk transformiert?  
[Zurück zu den Punkten](#Kategorien)

---

## @K3 200 Punkte
- Mit welcher Spannungsart betreibt man einen Transformator?  
[Zurück zu den Punkten](#Kategorien)

---

## @K3 400 Punkte
- Was fällt auf, wenn wir berechnete und gemessene Werte der Sekundärspannung vergleichen?  
[Zurück zu den Punkten](#Kategorien)

---

## @K3 600 Punkte
- Wie müssen Spannungsmessgeräte in einem Stromkreis geschaltet sein?  
[Zurück zu den Punkten](#Kategorien)

---

## @K3 800 Punkte
- Mit welcher Formel haben wir die Vergleichswerte der Sekundärspannung errechnet?  
[Zurück zu den Punkten](#Kategorien)
