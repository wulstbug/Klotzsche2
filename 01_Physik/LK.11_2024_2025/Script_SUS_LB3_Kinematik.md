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

## 3. 4. Bewegungsgleichungen für gleichförmige und gleichmäßig beschleunigte Bewegung

@color(Fertige eine Übersicht mit den Bewegungsgleichungen zur gleichförmigen und gleichmäßig beschleunigten Bewegung an. Ergänze die fehlenden Punkte., blue)


| | Gleichförmige Bewegung | Gleichmäßig beschleunigte Bewegung |
| --- | --- | --- |
| Bedingungen für Gültigkeit | .. | .. |
| Bewegungsgleichungen | .. | .. |
| phys. Größen | .. | .. |


{{1}}
*****************

__Graphen zu den Bewegungsgleichungen:__

![TB_Bewegungsgraphen](https://diversewolken.ddns.net/nextcloud/index.php/s/ALC7i99HXpRtPwT/download)

*****************

## 3. 5. Analyse einer gleichmäßig beschleunigten Bewegung

<p style="color:blue">

Analysiere die gleichmäßig beschleunigte Bewegung einer Kugel auf einer schiefen Ebene auf einer Strecke von s = 1m.

1. Nutze Metzler LB S18/19. Lies den Abschnitt 1.1.4. 

2. Zeichne eine Skizze und notiere alle geometrisch notwendigen Größen. Ermittle den Neigungswinkel der Ebene.

3. Erstelle mit Hilfe der Videoanalyse-Software ein s(t) und ein zugehöriges v(t)-Diagramm. 

4. Ermittle mit Hilfe der Bewegungsgleichung und eines Messwertes die Beschleunigung.

5. Erzeuge mit Hilfe deiner berechneten Beschleunigung einen theoretische s(t) und v(t) Graph und stelle diese mit den jeweiligen Messwerten gemeinsam dar.

6. Erzeuge aus den Diagrammen ein pdf und lade es [hier hoch](https://diversewolken.ddns.net/nextcloud/index.php/s/g5fRq7MWqJWJ8Sa), du erhältst einen Ausdruck.

7. Analysiere die auf die Kugel wirkenden Kräfte. Ermittle die wirkende Rollreibungskraft $F_R$ und den Rollreibungskoeffizienten $\mu_{roll}$.

</p>

### Aufgabe: Berechnungen an zusammengesetzten Bewegungen

__Erläuterung:__ Das folgende Diagramm wurde mit Hilfe der App Phyfox auf einer Autofahrt zwischen der _Tannenstraße (Dresden Neustadt)_ und der Haltstelle _Industriegebiet Süd_ aufgezeichnet. An Punkten, wo sich die Art der Bewegung ändert sind Markierungen auf dem Diagramm hinterlegt.

Die farbig gekennzeichneten Bereiche können als gleichmäßig beschleunigte Bewegungen betrachtet werden.

![Diagramm_PraktischeFahrt](https://diversewolken.ddns.net/nextcloud/index.php/s/K9XZ7yMM9n9AtLT/download)

> __Vorbetrachtung:__ Für die Bestimmung der Beschleunigung $a$ bei einer gleichmäßig beschleunigten Bewegung lässt sich auch die Formel
>
> $$ a = \frac{\Delta v}{\Delta t} $$
>
> verwenden. Hier bei ist $\Delta v$ die Geschwindkeitsänderung während des Zeitintervals $\Delta t$.
>
> Dabei ist $\Delta v$ definiert als 
>
> $$ \Delta v = v_{2} - v_{1}, $$
>
> also die Differenz der Geschwindigkeiten am Ende des Zeitintervals ($v_2$) und der Geschwindigkeit am Anfang des Zeitintervals ($v_1$).

__Löse folgende Aufgaben. Zur Selbstüberprüfung gibt es die Kontrollkästchen. Bei fehlerhaften Lösungen bitte per E-Mail rückmelden.__

1. Bestimme die gesamte Fahrtzeit (d.h. die gesamte Messzeit).

@rangeQuiz2($\hspace{1cm}$ t, 370, s)

---

2. Bestimme den gesamten Fahrtweg (d.h. die gesamte Messstrecke). 

@rangeQuiz2($\hspace{1cm}$ s, 3060, m)

---

3. Berechne die Geschwindigkeit  $v_2$, d.h. die Geschwindigkeit zwischen den Punkten 6 und 7 in der Einheit m/s.

@rangeQuiz2($\hspace{1cm}$ $v_2$, 12.56 , $\frac{m}{s}$)

---

4. Berechne die Geschwindigkeit  $v_3$, d.h. die Geschwindigkeit zwischen den Punkten 8 und 9 in der Einheit km/h.

@rangeQuiz2($\hspace{1cm}$ $v_3$, 63.16 , $\frac{m}{s}$)

---

5. Berechne die Durchschnittsgeschwindigkeit für die gesamte Messung/Fahrt (d..h von 0->11).

@rangeQuiz2($\hspace{1cm}$ $\overline{v_{ges}}$, 8.27 , $\frac{m}{s}$)

---

6. Berechne die Durchschnittsgeschwindigkeit für die gesamte Messung/Fahrt ohne Wartephase an den Ampeln, d.h. berechne die Durchschnittsgeschwindigkeit für die reine Bewegungszeit.

@rangeQuiz2($\hspace{1cm}$ $\overline{v'_{ges}}$, 11.91 , $\frac{m}{s}$)

<div style="text-indent:10%">

<details>

<summary> Lösung 6. </summary>

$ v_D = \frac{3060\,m}{370\,s-20\,s-73\,s-20s}= \frac{3060\,m}{257\,s} = 11,91 \frac{m}{s} = 15,15 \cdot 3,6 \frac{km}{h}  = 50 \frac{km}{h}$

</details>

</div>

---

7. Bestimme die Beschleunigungszeit zwischen den Punkten 5 und 6.

@rangeQuiz2($\hspace{1cm}$ $\overline{t_{5->6}}$, 25 , s)

---

8. Ermittle die Gschwindigkeitsänderung $\Delta v_{7->8}$ zwischen den Punkten 7 und 8.

@rangeQuiz2($\hspace{1cm}$ $\Delta v_{7->8}$, 4.985 , $\frac{m}{s}$)

<div style="text-indent:10%">

<details>

<summary> Lösung 8. </summary>

Die Geschwindigkeit $v_3$ beträgt $17,54 \frac{m}{s}$. Die Geschwindigkeit $v_2$ beträgt $12,56 \frac{m}{s}$. Die Änderung der Geschwindigkeit ist dann die Differenz $4,99 \frac{m}{s}$.

</details>

</div>

---

9. Ermittle die Beschleunigungen der farbig markiert Intervalle: $a_{1->2}$, $a_{3->4}$, $a_{5->6}$, $a_{7->8}$ und $a_{9->10}$.

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{1->2}$, 1.72 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Hinweis $a_{1->2}$  </summary>

Die Beschleunigung kann ermittelt werden aus der Änderungen der Geschwindigkeit $\Delta v$ geteilt durch die dafür benötigte Zeit $\Delta t$.

</details>

<details>

<summary> Lösung $a_{1->2}$  </summary>

Die Geschwindigkeit im Abschnit 0->1 ist $0 \frac{m}{s}$. Die Geschwindigkeit im Abschnitt 2->3 ist 

$$v_{2->3} = \frac{275m-60m}{50s-25s} = 8,6 \frac{m}{s}$$ 

Damit ist die Geschwindigkeitsänderung $\Delta v_{1->2} = 8,6 -0 \frac{m}{s} = 8,6 \frac{m}{s}$.

Die benötigte Zeit $\Delta t_{1->2} = 25s-20s = 5s$. Somit ist die Beschleunigung

$$ a_{1->2} = \frac{\Delta v_{1->2}}{\Delta t_{1->2}} = \frac{8,6 \frac{m}{s}}{5s} = 1,72 \frac{m}{s^2}$$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{3->4}$, -0.319 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Hinweis $a_{3->4}$  </summary>

Eine _gleichmäßg gebremste Bewegung_ ist eine gleichmäßig beschleunigte Bewegung mit @color(negativer, red) Beschleunigung. Da hier die Geschwindigkeit von $8,6 \frac{m}{s}$ auf $0 \frac{m}{s}$ sinkt, ist die Geschwindigkeitsänderung negativ. D.h. $\Delta v_{3->4} = -8,6 \frac{m}{s}$.

</details>

<details>

<summary> Lösung $a_{3->4}$  </summary>

$$ a_{3->4} = \frac{\Delta v_{3->4}}{\Delta t_{3->4}} = \frac{-8,6 \frac{m}{s}}{27s} = -0,319 \frac{m}{s^2}$$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{5->6}$, 0.502 , $\frac{m}{s^2}$)

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{7->8}$, 0.199 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Lösung $a_{7->8}$  </summary>

$$ a_{7->8} = \frac{\Delta v_{7->8}}{\Delta t_{7->8}} = \frac{v_{8->9} - v_{6->7}}{\Delta t_{7->8}} = \frac{17,54\frac{m}{s} - 12,56\frac{m}{s}}{25s}  = 0,199 \frac{m}{s^2} $$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{9->10}$, -0.877 , $\frac{m}{s^2}$)


## Bewegungsanalyse eines schrägen Wurfes

{{1}}
************
__$y(x)$-Diagramm__:

![Diagram-x-y](https://diversewolken.ddns.net/nextcloud/index.php/s/EpjbjtLSPyRePeZ/download)
************

<p class="newspaper">

{{2}}
************
__$x(t)$__

![Diagram-t-x](https://diversewolken.ddns.net/nextcloud/index.php/s/jN69KQoCJZdy8Xf/download)
************

{{3}}
************
__$v_x(t)$__

![Diagram-t-y](https://diversewolken.ddns.net/nextcloud/index.php/s/mGjYeN46XzHgsaE/download)
************

<p class="cb">

{{2}}
************
__$y(t)$__

![Diagram-t-vx](https://diversewolken.ddns.net/nextcloud/index.php/s/Ey7B9XgB7795GA6/download)
************

{{3}}
************
__$v_y(t)$__

![Diagram-t-vy](https://diversewolken.ddns.net/nextcloud/index.php/s/XBoLRYiosKtKCsx/download)
************

</p>

</p>

## 3.6 Kinematik des schrägen Wurfs

> __Beschreibung:__ Bei einem schrägen Wurf wird ein Körper unter einem Winkel $\alpha$ mit einer Anfangsgeschwindigkeit $\vec{v_0}$ abgeschossen (geworfen). Reibungseffekte werden zunächst vernachlässigt.

> __Zerlegung der Bewegung in x- und y-Richtung:__ 
{{1}}
*******
1. die Flugbahn $y(x)$ entspricht einer Parabel.
![Parabel](https://diversewolken.ddns.net/nextcloud/index.php/s/EpjbjtLSPyRePeZ/download)<!-- style="width:40%"-->
*******
{{2}}
*******
2. die horizontale Bewegung $x(t)$ ist eine __gleichförmige Bewegung__

$$ \boxed{x(t) = v_{0x} \cdot t} \mathrm{\ \ \ und\ \ \ } \boxed{v_x(t) = v_{0x}}$$

$\hspace{1cm}$ $v_{0x}$ .. Anfangsgeschwindigkeit in x-Richtung
*******
{{3}}
*******
3. die vertikale Bewegung $y(t)$ ist eine __gleichmäßig beschleunigte Bewegung__ mit dem Ortsfaktor $g=9,81\frac{m}{s^2}$ als Beschleunigung.

$$ \boxed{y(t) = \frac{1}{2}\cdot g \cdot t^2 + v_{0y} \cdot t} \mathrm{\ \ \ und\ \ \ } \boxed{v_y(t) = g \cdot t + v_{0y}}$$

$\hspace{1cm}$ $v_{0y}$ .. Anfangsgeschwindigkeit in y-Richtung

$\hspace{1cm}$ @color(Achtung:,red) Wenn die y-Achse nicht zur Erde hin zeigt, ist @color(g=-9.81$\frac{m}{s^2}$,red).
*******
{{4}}
*******
4. Die Anfangsgeschwindigkeit $\vec{v_0}$ ist eine vektorielle Größe und lässt sich in ihre x-Kompente ($v_{0x}$) und y-Komponente ($v_{0y}$) zerlegen. <br>
![Geschwindigkeit](https://diversewolken.ddns.net/nextcloud/index.php/s/qdAbC6XTmRXztaa/download)$$ \boxed{v_{0x} = v_0 \cdot \cos\alpha} \mathrm{\ \ \ und\ \ \ } \boxed{v_{0y} = v_0 \cdot sin\alpha} $$
*******
{{5}}
*******
5. die gesamte Bewegung ist eine @color(Superposition, red) (d.h. Überlagerung) der Bewegungen in x- und y-Richtung
*******

### 3.6.1 Berechnungen am Demonstrationsexperiment: Schräger Wurf

Für das Demonstrationsexperiment beträgt der Abwurfwinkel $\alpha=59^\circ$. Die Anfangsgeschwindigkeit $v_0$ wird mit $3,21 \frac{m}{s}$ angegeben.

__Aufgaben__:

1. Ermittle die Anfangsgeschwindigkeiten $v_{0x}$ und $v_{0y}$.

@rangeQuiz2($\hspace{1cm}$$v_{0x}$, 1.65, $\frac{m}{s}$)

@rangeQuiz2($\hspace{1cm}$$v_{0y}$, 2.75, $\frac{m}{s}$)

---

2. Notiere die Bewegungsgleichungen x(t) und y(t). Schreibe alle Zahlenwerte aus.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

$$ x(t) = 1,65 \frac{m}{s} \cdot t $$

$$ y(t) = - \frac{1}{2} \cdot 9,81 \frac{m}{s^2}\cdot t^2 + 2,75 \frac{m}{s} \cdot t $$

</details>

</div>

---

3. Notiere die Bewegungsgleichungen $v_x(t)$ und $v_y(t)$.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

$$ v_x(t) = 1,65 \frac{m}{s} $$

$$ v_y(t) = - 9,81 \frac{m}{s^2}\cdot t + 2,75 \frac{m}{s}$$

</details>

</div>

---

4. Ermittle für den höchsten Punkt: $t_{max}$, $x(t_{max})$, $y(t_{max})$. Vergleiche deine Berechung mit dem experimentellen Diagramm (aus 3.6).

@rangeQuiz2($\hspace{1cm}$ $t_{max}$, 0.28, $s$)

@rangeQuiz2($\hspace{1cm}$ $x_{max}$, 0.4625, $m$)

@rangeQuiz2($\hspace{1cm}$ $y_{max}$, 0.385, $m$)



<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Im Maximum ist $v_y(t)=0$.

</details>

</div>

5. Ermittle aus den Messdaten die Wurfweite $x_{Wurf}$, d.h die Entfernung, wo die Kugel wieder die Ausgangshöhe (0) zurückkehrt.

@rangeQuiz2($\hspace{1cm}$ $x_{wurf}$, 0.925 , $m$)

<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Für den Zeitpunkt der Wurfweite gilt:  $y(t_{wurf}) = 0$.

</details>

<details>

<summary> Lösung </summary>

Setze $ y(t_{wurf}) = 0 $:

$$ 0 = -\frac{1}{2} \cdot 9,81 \frac{m}{s^2}\cdot t^2 + 2,75 \frac{m}{s} \cdot t $$

$$ t_{wurf\,1} = 0\,\,\mathrm{(Startpunkt)}$$

$$ t_{wurf\,2} = \frac{2\cdot 2,75 \frac{m}{s}}{9,81 \frac{m}{s^2}} = 0,561 s$$

Berechne $ x(t_{wurf\,2}) $:

$$ x(t_{wurf}) = 1,65 \frac{m}{s} \cdot t_{wurf\,2} = 0,925\,m$$

</details>

</div>


6. Zeichne in das y(x)-Diagramm des Experiments die Flugbahn anhand der hier berechneten Daten. Nutze als Zeitschritte z.B. 0,05 s und die Bewegungsgleichungen aus 2. <br> Diskutiere Ursachen für die Unterschiede der beiden Graphen.

<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Berechne für Zeitschritte von 0,05s x(t) und y(t) und trage die Punkte in das Diagramm ein.

</details>

<details>

<summary> Lösung </summary>

![Loesung_x_y](https://diversewolken.ddns.net/nextcloud/index.php/s/DqKyz8DiaDCfgi5/download)

</details>

<details>

<summary> Diskussion Unterschiede </summary>

In der Auswertung des Diagramms ergab sich eine Beschleunigung von ca. $-11,5 \frac{m}{s^2}$. Der hier berechnete Graph nutzt als Beschleunigung $-9,81 \frac{m}{s^2}$.

</details>

<details>

<summary> Korrektur </summary>

![Loesung_x_y_11.5](https://diversewolken.ddns.net/nextcloud/index.php/s/MStYLTsW2CfQ27a/download "Darstellung der experimentellen x-y-Graphen (exp), der theoretischen x-y-Graphen mit Beschleunigung $g=-9,81\frac{m}{s^2}$ (theor_9.81) und der theoretischen x-y-Graphen mit Beschleunigung $a=-11,5\frac{m}{s^2}$ (theor_11.5)")

</details>

</div>

## 3.7 Die Momentangeschwindigkeit

![Tafelbild_Momentangeschwindigkeit](https://diversewolken.ddns.net/nextcloud/index.php/s/2gC5MmDGj7DoSqy/download)


### Übung: Zuordnung Graphen

<p class="newspaper">

Gegeben sind folgende v(t)-Graphen für 7 verschiedene Fälle.

![Faelle_vt](https://diversewolken.ddns.net/nextcloud/index.php/s/L8Y8XrqrZpBX6Tt/download)

<p class="cb">

Ordne im folgenden Bild die x(t) Fälle den v(t) Fällen zu.

<iframe src="https://learningapps.org/watch?v=pd58g8qzt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

</p>

</p>

### Abituraufgabe 1 Bewegungsvorgänge

1. 1. Ein Pkw fährt auf der Autobahn mit der konstanten Geschwindigkeit von 130 km/h. In der Entfernung von 200 m nimmt der Fahrer die elektronische Verkehrsleiteinrichtung wahr, die die Höchstgeschwindigkeit 80 km/h vorschreibt und auf einen Unfall hinweist. Nach der Reaktionszeit 0,8 s betätigt der Fahrer die Bremse. Die Verzögerung erfolgt gleichmäßig. Der Pkw erreicht exakt beim Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit. <br> Zeichnen Sie ein s(t)- und ein v(t)-Diagramm für den Zeitraum vom Erkennen der Anzeige bis zum Passieren der Verkehrsleiteinrichtung. Berechnen Sie die notwendige Bremsbeschleunigung und die Bremszeit. (5BE)

---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Reaktionsweg: $s_{R}$, 28.9 , $m$)

@rangeQuiz2(Bremsweg: $s_{brems}$, 171.1 , $m$)

---

__Endergebnisse:__

@rangeQuiz2(Bremsbeschleunigung: $a_{brems}$, -2.4 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.9 , $s$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

Es liegen zwei Bewegungsabschnitte vor: Innerhalb der Reaktionszeit $t_R= 0,80 s$ erfolgt die Bewegung zunächst geradlinig gleichförmig mit der Anfangsgeschwindigkeit $v_0 = 130 km/h$. Während des zweiten Abschnittes verringert sich die Geschwindigkeit während der Bremszeit $t_B$_ linear bis zur vorgeschriebenen Höchstgeschwindigkeit $v_H = 80 km/h$.

</details>

<details>

<summary> Hinweis 2 </summary>

Im v-t-Diagramm wird also zunächst wegen der Konstanz der Geschwindigkeit wäh­rend der Reaktionszeit eine Parallele zur Abszissenachse gezeichnet, anschließend ein Stück einer fallenden Geraden. <br> Im s-t-Diagramm erscheint zunächst eine steigende Gerade, die in eine nach unten geöffnete Parabel übergeht. Der Anstieg dieses Parabeiabschnittes verringert sich, darf aber am Ende noch nicht den Scheitel dieser Parabel erkennen lassen.<br> Beachten Sie: Es gilt v = Also entspricht im s-t-Diagramm dem steigenden Parabei­stück mit abnehmendem Anstieg im v-t-Diagramm die fallende Gerade. Und da die
Geschwindigkeit am Ende des zweiten Abschnittes nicht Null beträgt, befindet sich ent­sprechend am Ende des Parabeiastes noch nicht der Scheitel!

</details>

<details>

<summary> Lösung Diagramme </summary>

![Diagramm_L_1.2](https://diversewolken.ddns.net/nextcloud/index.php/s/F8LAqziiJ2HTBiQ/download)

</details>

<details>

<summary> Hinweis 3: Berechnungen </summary>

Wir betrachten hier __lediglich den Bremsvorgang__. Für den Bremsweg $s_{Brems}$ ergibt sich 171,1 m. Die Geschwindigkeit verringert sich von 36,1m/s (130 km/h) auf 22,2 m/s (80 km/h). Man stellt die Bewegungsgleichungen s(t) und v(t) für den Bremsvorgang auf und ermittelt die Unbekannten t und a.

</details>

<details>

<summary> Lösungen: Berechnungen </summary>

Allgemein:

$$ s(t) = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t $$

$$ v(t) = a \cdot t + v_0 $$

Eingesetzt bedeutet das:

$$ 171,1 m = \frac{1}{2} \cdot a \cdot t^2 + 36,1\frac{m}{s} \cdot t $$

$$ 22,2 \frac{m}{s} = a \cdot t + 36,1 \frac{m}{s} $$

Der CAS bietet als Lösungen: $a=-2,38 \frac{m}{s^2}$ und $t=5,87 s$.

</details>



</div>

---

1. 2. Der Fahrer hält nach dem Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit 80 km/h zunächst ein. Durch das Geschehen an der Unfallstelle abgelenkt, bemerkt er jedoch ein 30 m vor ihm mit der Geschwindigkeit 30 km/h gleichförmig fahrendes Fahrzeug sehr spät. Er leitet nach Reaktionszeit 1,0 s eine Vollbremsung ein. Die Verzögerung erfolgt wiederum gleichmäßig. Berechnen Sie die Bremsverzögerung, die mindestens notwendig wäre, um einen Auffahrunfall zu vermeiden. Ein Ausweichen ist nicht möglich. (3BE)


---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Abstand nach Reaktion: $s_{A}$, 16.1 , $m$)

---

__Endergebnisse:__

@rangeQuiz2(minimale Bremsbeschleunigung: $a'$, -6 , $\frac{m}{s^2}$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

![H1_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/pjQocKxARbQKKi6/download)

</details>

<details>

<summary> Hinweis 2 </summary>

![H2_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/HwgKG7CQHTG87rr/download)

</details>

<details>

<summary> Hinweis 3 & Lösung</summary>

![H3_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/2HqqGAtQJQz8cfi/download)

</details>

</div>

---

1. 3. Der Unfall war nicht zu verhindern und der Pkw mit der Masse 1,1 t prallte auf das vorausfahrende Fahrzeug mit der Masse 1,8 t. Die Geschwindigkeit des Pkw betrug unmittelbar vor dem Aufprall 40 km/h. Beim Aufprall setzte der Bremsvorgang aus und die beiden Fahrzeuge verhakten sich. Berechnen Sie den Betrag der während des Zusammenstoßes verrichteten Verformungsarbeit. (3BE)

---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Geschwindigkeit nach Zusammenstoß: $v'$, 9.39 , $\frac{m}{s}$)

---

__Endergebnisse:__

@rangeQuiz2(Verformungsarbeit: $W$, 2600 , $J$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

Für die gemeinsame Geschwindigkeit $v'$ nach dem Stoß gilt:

$$ v' = \frac{m_1\cdot v_1 + m_2 \cdot v_2}{m_1+m_2} = 9,39 \frac{m}{s} $$

</details>

<details>

<summary> Hinweis 2 </summary>

Der Betrag der Verformungsarbeit $W$ ergibt sich aus der Differenz der kinetischen Energien vor und nach dem Stoß.

$$ W = \frac{1}{2} \cdot m_1 \cdot v_1^2 + \frac{1}{2} \cdot m_2 \cdot v_2^2 - \frac{1}{2} \cdot (m_1+m_2) \cdot v'^2 = 2,6 kJ $$

</details>

</div>


### Abituraufgabe 2 Bewegungsvorgänge

In der Vorbereitungsphase eines Autorennens finden Tests statt. 

2. 1. Zunächst werden die Bremsen des Rennwagens A getestet. Dazu wird der Wagen von 230 km/h auf 80 km/h gleichmäßig abgebremst. Aus den elektronisch über­mittel­ten Daten wird der Bremsweg 240 m bestimmt. <br> Berechnen Sie die Beschleunigung und die Bremszeit. Zeichnen Sie ein zugehöriges s(t)-Diagramm. (6 BE)

---

<div style="margin-left:10%">

__Endergebnisse:__

@rangeQuiz2(Beschleunigung: $a$, -7.5 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.6 , $a$)

---

__Hilfestellungen:__

<details>

<summary> Hinweis 1 </summary>

Wenden Sie die vollständigen Bewegungsgleichungen auf den Rennwagen A an. 

</details>

<details>

<summary> Lösung Diagramm </summary>


![L_Diagramm_H1_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/oZXtydeE2KQgP2p/download)


![L_Diagramm_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/YZAcS83Xd64Nybp/download)

</details>

</div>

---

2. 2. Danach wird der Rennwagen B getestet. Der Rennwagen beschleunigt aus der Ruhe he­r­aus auf die Endgeschwindigkeit $v_1$. Die Geschwindigkeit nimmt linear mit dem zu­rück­gelegten Weg zu. <br> Begründen Sie, dass die Beschleunigung nicht konstant ist. 	(2 BE)


---

<div style="margin-left:10%">


__Hilfestellungen:__

<details>

<summary> Hinweis 1</summary>

![H1_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/BHsxffnyDFjLG5a/download)

</details>

<details>

<summary> Lösung</summary>

![L1_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/RoseCfNeNfHxiwK/download)

</details>

</div>

---

2. 3. Nun werden beide Fahrzeuge gleichzeitig getestet. <br> Rennwagen A und Rennwagen B passieren gleichzeitig ein und denselben Ort mit der Ge­schwindigkeit 180 km/h bzw. 200 km/h. Ab diesem Zeitpunkt ($t = 0$) treten beim Renn­wagen B Motorprobleme auf und dessen Geschwindigkeit sinkt danach ge­mäß der in der Tabelle dargestellten Daten.

<div style="margin-left:10%">

|         |      |      |      |     |     |    |
| t in s  | 0    | 5    | 10   | 15  | 20  | 25 |
| v in m/s| 55,6 | 35,6 | 20,0 | 8,9 | 2,2 | 0  |


Die Geschwindigkeit von Rennwagen A bleibt konstant und er überholt Rennwagen B we­gen dessen Motorschadens. Weisen Sie nach, dass dies etwa nach 2,7 s geschieht. (4BE)

</div>


---

<div style="margin-left:10%">



__Hilfestellungen:__

<details>

<summary> Hinweis 1</summary>

Den Nachweis des Überholens können Sie führen, indem Sie zeigen, dass sich beide Fahrzeuge zum Zeitpunkt $t_Ü = 2,7s$ am gleichen Ort befinden. 

</details>

<details>

<summary> Lösung Teil A</summary>

![L1_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/XqGj6J8W3TTyXF9/download)

</details>

<details>

<summary> Lösung Teil B</summary>

![L2_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/QEBAgfKodnbDHsj/download)

</details>

</div>


### Übung 3. (auf Zeit) - Gleichungssysteme lösen

<p style="color:blue">

Die folgenden Übungsaufgaben sollen das zügige Lösen von Gleichungssystemen für kinematische Aufgabenstellungen trainieren.
 
Notiere die Bewegungsgleichungen und löse die Aufgabe mit dem CAS. Überprüfe deine Lösungen hier.

</p>

3. 1. Zwei Körper (A und B) beginnen ihre Bewegung zum Zeitpunkt t=0s am Ort x=0m. Körper A führt eine gleichmäßig beschleunigte Bewegung aus mit der Anfangsgeschwindigkeit 0m/s. Körper B bewegt sich gleichförmig. Körper A überholt Körper B nach 100m und 30s. Ermitteln Sie Beschleunigung $a_A$ und die Anfangsgeschwindigkeit $v_{0B}$.

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort A}: 100 m = \frac{1}{2} \cdot a_A \cdot (30))^2$$

$$ \mathrm{Ort B}: 100 m = v_{0B} \cdot t \frac{m}{s} $$

</details>

---

@rangeQuiz2($a_{A}$, 0.222 , $\frac{m}{s^2}$)

@rangeQuiz2($v_{0B}$, 3.33 , $\frac{m}{s}$)

</p>

3. 2. Ein Ball wird aus einer Höhe $h_0 = 5m$ mit einer Anfangsgeschwindigkeit $v_0$ senkrecht nach oben geworfen. Der Ball schlägt mit einer Geschwindigkeit von 15 m/s auf den Boden auf. Reibung wird vernachlässigt. Ermittle Anfangshöhe $h_0$ und Flugzeit $t_{Flug}$. <br> @color(Achte auf die Vorzeichen der Zahlenwerte., red)

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort}:  0 = \frac{1}{2} \cdot -9,81 \frac{m}{s^2}\cdot t^2 + v_0 \cdot t + 5m$$

$$ \mathrm{Geschwindigkeit}: -15 \frac{m}{s} = -9,81\frac{m}{s^2} \cdot t + v_0 $$

</details>

---

@rangeQuiz2($v_0$, 11.265 , $\frac{m}{s}$)

@rangeQuiz2($t$, 2.677 , $s$)

</p>

3. 3. Zwei Motoradfahrer fahren auf geradliniger Strecke. Beide befinden sich wie dargestellt zum Zeitpunkt t=0s an den Markierungen A bzw. B. P ist in Fahrtrichtung 50m von A entfernt. Im Punkt M hat A eine Geschwindigkeit von 90 km/h und verzögert gleichmäßig. Im Punkt P hat B eine Geschwindigkeit von 72 km/h und verzögert gleichmäßig mit 1 m/s². Ermitteln $a_A$ derart, dass A und B zu einem Zeitpunkt dieselbe Geschwindigkeit und denselben Ort haben. Ermittle den zugehörigen Abstand s zwischen B und dem Treffpunkt.

![Pitty_713](https://physikaufgaben.de/bild/a713_1.gif)<!-- style="max-width:80%;margin-left:10%"-->

---

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{A}: x_A(t) = \frac{1}{2}\cdot a_A \cdot t^2 + 25 \frac{m}{s} \cdot t \hspace{1cm} v_A(t) = a_A \cdot t + 25 \frac{m}{s} $$

$$ \mathrm{B}: x_B(t) = \frac{1}{2}\cdot (-1 \frac{m}{s^2}) \cdot t^2 + 20 \frac{m}{s} \cdot t + 50m \hspace{1cm} v_B(t) = (-1 \frac{m}{s^2}) \cdot t + 20 \frac{m}{s}  $$

$$ \mathrm{Setze} : x_A(t) = x_B(t) \hspace{1cm} \mathrm{und} \hspace{1cm} v_A(t) = v_B(t) $$

</details>

---

@rangeQuiz2($a_{A}$, -1.25 , $\frac{m}{s^2}$)

@rangeQuiz2($t$, 20 , $s$)

@rangeQuiz2($s$, 200 , $m$)

</p>

---

3. 4. __(Wdh. Abi 1)__ Ein Pkw fährt auf der Autobahn mit der konstanten Geschwindigkeit von 130 km/h. In der Entfernung von 200 m nimmt der Fahrer die elektronische Verkehrsleiteinrichtung wahr, die die Höchstgeschwindigkeit 80 km/h vorschreibt und auf einen Unfall hinweist. Nach der Reaktionszeit 0,8 s betätigt der Fahrer die Bremse. Die Verzögerung erfolgt gleichmäßig. Der Pkw erreicht exakt beim Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit. <br> Berechnen Sie für den Bremsvorgang die notwendige Bremsbeschleunigung und die Bremszeit.

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort:} 171,1 m = \frac{1}{2} \cdot a \cdot t^2 + 36,1\frac{m}{s} \cdot t $$

$$ \mathrm{Geschwindigkeit}: 22,2 \frac{m}{s} = a \cdot t + 36,1 \frac{m}{s} $$

</details>

---

@rangeQuiz2(Bremsbeschleunigung: $a_{brems}$, -2.4 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.9 , $s$)

</p>