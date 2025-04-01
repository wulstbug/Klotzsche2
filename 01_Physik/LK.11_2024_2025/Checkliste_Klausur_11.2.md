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

@timer2

<div style="position: fixed; right:50px; top:300px;">

<details>

<summary> Timer(@0:@1) </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe width="200" height="90" src="https://webuhr.de/embed/timer/#countdown=00:@0:@1&enabled=0&onzero=0&theme=0&ampm=0&sound=xylophone" frameborder="0" allowfullscreen>

</iframe> 

</div>

</details>

</div>

@end

@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0$\ $=$\ $ 
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
    input <= 0.03
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left">
@2
</div>
</div>
@end

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0 = 
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
    input <= 0.2
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left">
@2
</div>
</div>
@end

@@@ ogy.de/11Ph2 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Checkliste Klausur 03.04.2025

- Elektrisches Feld

    - homogene und inhomogene elektrische Felder, elektrische Feldlinien, Feldformen

    - Feldformen (Plattenkondensator, Punktladung)

    - Coulombkräfte zwischen Punktladungen

    - Definition elektrisches Feld, elektrische Kraft auf Ladungen im elektrischen Feld

    - Kraftwirkungen und elektrisches Feld im Plattenkondensator

    - Energie im elektrischen Feld

- Plattenkondensator

    - Kapazitätsbegriff (allgemein und im Plattenkondensator)

    - Dielektrikum (Matierie im elektrischen Feld, Polarisation)

    - Lade- und Entladevorgänge (Spannung und Stromstärke)

- Magnetisches Feld

    - Kraftwirkungen im magnetischen Feld (stromdurchflossene Leiter, bewegte geladene Teilchen, andere Magnete)

    - Berechnung magnetische Flussdichte

    - Materie im magnetischen Feld (Ferromagnetika, Magnetisierung)

- geladene Teilchen in statischen Feldern

    - geladene Teilchen in elektrischen Felder (Längsfeld, Elektronenkanone)

    - Herleitung: Endgeschwindigkeit der Elektronen

    - Kräfte berechnen, Art der Bewegung

    - Milikan-Versuch


# Checkliste Klausur 15.01.2025

- verschiedene Arten von Bewegungen, deren Gültigkeitsbedingung, deren Beschreibung in Form von Bewegungsgleichungen bzw. deren Darstellung in Diagrammen s(t), v(t), a(t)

- Anwenden der Bewegungsgleichungen beim Lösen von Fragestellungen zur Bewegung von einem oder zwei Körpern

- Bewegungen und Reibungskräfte

- Kinematik des senkrechten und waagerechten Wurfes, Herleitung der Wurfparabel

- Ermittlung der Momentangeschwindigkeit aus dem s(t)-Diagramm, sowie des zurückgelegten Wegs aus dem v(t)-Diagramm

- Anwendung der Newton'schen Gesetze zur Ermittlung von Beschleunigungen basierend auf den wirkenden Kräften

- geeignete Zerlegung von Vektoren (z.B. Geschwindigkeitsvektor, Kraftvektor)

- Fehlertypen und Fehlerfortpflanzung für berechnete physikalische Größen

- Grundlagen der Lernbereiche I/II: Energie, Kräfte, Erhaltung
