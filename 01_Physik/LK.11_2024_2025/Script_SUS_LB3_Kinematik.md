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

.red {
    color: red;
}

.blue {
    color: blue;
}

.darkgreen {
    color: darkgreen;
}

.orange {
    color: orange;
}

.purple {
    color: purple;
}

@end

@color
<bdi style="color:@1">@0</bdi>
@end


@rangeQuiz2
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


@onload
window.LIA.settings.font_size = 2
@end

-->

# LB 3 Kinematik und Dynamik - Praktikum

![KinematikUndDynamik](https://www.online-wissensdatenbank.de/wp-content/uploads/2023/12/kinematik-grundlagen-der-bewegungslehre.jpg "Bild-Quelle: https://www.online-wissensdatenbank.de")

## 3.1. Einführung in die Analyse von Bewegungen

Die __Kinematik__ (altgriechisch κίνημα kinema, deutsch ‚Bewegung‘) ist das Gebiet der Mechanik, in dem die Bewegung von Körpern rein geometrisch mit den Größen <bdi style="color:red">Ort, Zeit, Geschwindigkeit und Beschleunigung</bdi> beschrieben wird.

{{1}}
*******
__Formelzeichen:__

<div style="text-indent:10%">

> $t$ .. Zeit $\Big[ s \Big]$
>
> $x,y,z$ .. Ort/Position/Koordinate des Körpers $\Big[ m \Big]$
>
> $v$ .. Geschwindigkeit des Körpers $\Big[ \dfrac{m}{s} \Big]$
>
> $v_x$, $v_y$, $v_z$ .. Geschwindigkeits-Komponenten in x- y- bzw. z-Richtung
> 
> $a$ ..Beschleunigung $\Big[ \dfrac{m}{s^2} \Big]$
>
> $a_x$, $a_y$, $a_z$ .. Beschleunigungs-Komponenten in x- y- bzw. z-Richtung

</div>
*******

{{2}}
*******
__Abhängigkeiten:__ Um zu beschreiben, zu welcher Zeit sich ein Körper an welchem Ort aufhält, notiert man die Beziehung verschiedener kinematischer Größen folgender Art

_Beispiele:_

<div style="text-indent:10%">

> $x(t)$ ..  @color(_Gesprochen: x von t_,blue) bedeutet: Der Körper befindet sich zum Zeitpunkt $t$ am Ort $x$
>
> $v_x(t)$ .. Der Körper besitzt zum Zeitpunkt $t$ die x-Geschwindigkeit $v_x$ (oder Geschwindigkeit in x-Richtung)  

</div>
*******

{{3}}
*******
<bdi style="color:blue">
_Hinweis:_ Werden eindimensionale Probleme behandelt wird gelegentlich auf die Angabe der Koordinaten verzichtet. Dann kann für $x$ auch die Strecke $s$ und für die Geschwindigkeit lediglich $v$ genutzt werden.
</bdi>
******

## 3. 2. Kinematische Darstellung in Diagrammen

Häufig ist es __anschaulich__ die Bewegung eines Körpers in @color(Diagrammform, red) darzustellen.

<bdi style="color:red">
Vereinbahrung: In der Kinematik wird die Zeit __immer__ auf der x-Achse dargestellt.
</bdi>

Beispiel: x(t) Diagramm

![BeispielDiagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/EsD2fMgGed8tjRC/download)

__Aufgabe:__ Ergänze die Bewegungsarten

- P0 -> P1 

    <!-- data-solution-button="off" -->
    [(X)] Stillstand
    [( )] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung

- P1 -> P2

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [( )] gleichförmige Bewegung
    [(X)] gleichmäßig beschleunigte Bewegung

- P2 -> P3

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [(X)] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung


## 3. 3. Einführung Bewegungsanalyse

__Möglichkeiten zur zeitlichen Analyse von Bewegungen gibt es viele:__

- Stoppuhr und Maßband

- Maßband und Lichtschranke

- Videoanalyse 

- Ultraschallsensoren

- ...

{{1}}
**********
__Heute:__ Videoanalyse-Tool VIANA 2

@color(_Hinweise zur Handhabung:_,blue)

1. Positioniere die Kamera so, dass sie sich nicht bewegt.

2. Achte auf einen guten Kontrast zwischen bewegtem Objekt und Hintergrund während der gesamten Bewegung.

3. Führe vor der Aufnahme ein paar Beispielabläufe durch.

4. Markiere die vorab einen möglichst großen Streckenabschnitt im Bewegungsraum.

5. Bei eindimensionalen Bewegungen sollte das Koordinatensystem so ausgerichtet werden, dass sich das Objekt entlang der x-Achse bewegt.
*********

{{2}}
*********
__Aufgaben:__

1. Mache dich mit der Videoanalyse in VIANA 2 vertraut

2. Nimme eine gleichmäßg beschleunigte Bewegung anhand der Erklärung im Unterricht auf. 

3. Stelle das x(t) und v(t) Diagramm in der App __Numbers__ auf dem IPad dar. 

4. Ermittle die Beschleunigung aus den Messwerten der Kugel.

@rangeQuiz20($\hspace{1cm}$ $a$, 0.11, $\frac{m}{s^2}$)

_Hinweis: Bei dieser Überprüfung wird eine Ungenauigkeit von 20% gegenüber der Vergleichsmessung der Lehrkraft akzeptiert._

**********