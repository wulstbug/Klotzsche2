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

$$ \boxed{y(t) = \frac{1}{2}\cdot g \cdot t^2 + v_{y0} \cdot t} \mathrm{\ \ \ und\ \ \ } \boxed{v_y(t) = g \cdot t + v_{0y}}$$

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

## 3.6.1 Berechnungen am Demonstrationsexperiment: Schräger Wurf

Für das Demonstrationsexperiment beträgt der Abwurfwinkel $\alpha=59^\circ$. Die Anfangsgeschwindigkeit $v_0$ wird mit $3,2 \frac{m}{s}$ angegeben.

_Aufgaben_:

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

4. Ermittle für den höchsten Punkt: $t_{max}$, $x(t_{max})$, $y(t_{max})$. Vergleiche deine Berechung mit dem experimentellen Diagramm.

@rangeQuiz2($\hspace{1cm}$ $t_{max}$, 0.28, $s$)

@rangeQuiz2($\hspace{1cm}$ $x_{max}$, 0.4625, $m$)

@rangeQuiz2($\hspace{1cm}$ $y_{max}$, 0.385, $m$)



<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Im Maximum ist $v_y(t)=0$.

</details>

</div>

5. Zeichne in das y(x)-Diagramm die Flugbahn anhand der hier berechneten Daten. Nutze als Zeitschritte (0,05 s).

<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Berechne für Zeitschritte von 0,05s x(t) und y(t) und trage die Punkte in das Diagramm ein.

</details>

<details>

<summary> Lösung </summary>

![Loesung_x_y](https://diversewolken.ddns.net/nextcloud/index.php/s/DqKyz8DiaDCfgi5/download)

</details>

</div>