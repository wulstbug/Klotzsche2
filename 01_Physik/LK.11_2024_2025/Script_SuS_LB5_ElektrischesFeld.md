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
    .newspaper3 {
        column-count: 3;
        column-gap: 20px;
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

# LB5 - Elektrisches Feld

![Blitzeinschläge](https://img.welt.de/img/wirtschaft/webwelt/mobile218083858/8146580597-ci23x11-w2000/Out-Of-The-Blue.jpg)

## 5.1 Grundlagen Elektrizität

### 5.1.1 Atomaufbau

<span style="color:orange">*Ergänze und übernimm diese Wiederholung.*</span>

> Das Atom wird in zwei Grundstrukturen unterteilt

<!-- style="display: block; width: 100%; margin-left: auto;margin-right: auto;" -->
``` ascii
                  Atom
                    |
               .----o-----.             
              /            \             
             /              \           
            /                \          
           v                  v          
```
| [[ Atomkern  ]] | [[ Atomhülle ]] |
| :--: | :--: |




> Darin enthalten sind die Elementarteilchen mit ihren jeweiligen elektrischen Ladungszuständen

| Atomkern | elektrische Ladung |  Atomhülle |
|:--:|:--:|:--:|
| | ![Elektron](https://diversewolken.ddns.net/nextcloud/index.php/s/Bnw2kL8nFrErwXP/download)<span class="green">[[ negativ ]]</span> | <span class="green">[[ Elektron ]]</span> |
| <span class="red"> [[ Proton ]]</span> | ![Proton](https://diversewolken.ddns.net/nextcloud/index.php/s/fs9TTTmjnwRDNm5/download)<span class="red">[[ positiv ]]</span> | |
| [[ Neutron ]] | ![Neutron](https://diversewolken.ddns.net/nextcloud/index.php/s/YJnsjw6546zn55P/download)neutral | |

Beispiele: 

Das Kohlenstoffatom besitzt [[ 6 ]] Protonen im Kern, wohingegen ein Aluminiumatom [[ 13 ]] Protonen enthält. Die Protonenzahl wird durch die [[ Ordnungszahl ]] festgelegt.

{{1}}
************
<span style="color:orange">*Schau dir zur Veranschaulichung noch einmal die verschiedenen Atom-Modelle an. Diese Modelle müssen nicht übernommen werden.*</span>
![ModelleAtomaufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/Mw2YQeHk4bA3aaL/download)

************

### 5.1.2 Die elektrische Ladung

> Definition: Die elektrische Ladung eines Körpers gibt an, wie groß sein Elektronenüberschuss oder sein Elektronenmangel ist.
>
> __Formelzeichen: [[ Q ]]__
>
> __Einheit: 1 [[ C ]] ( [[ Coulomb ]] )__

Ein Elektron besitzt die kleinst mögliche Ladungsmenge, man nennt das eine __[[ Elementarladung ]] ($e$)__.

> $$ 1\,e = 1,602\cdot10^{-19} C $$

Die Anzahl $N$ der überzähligen Elementarladungen $e$ ergibt demnach die elektrische Ladung $Q$ eines Körpers. 

> $$Q = N \cdot e $$


__Elektrisch geladene Atome und Körper__

<span style="color:orange">*Ergänze und übernimm diese Wiederholung.*</span>

> Ein neutrales (nicht geladenes) Atom besitzt die [[ gleiche ]] Anzahl an Elektronen und Protonen. Ist die Anzahl der postiv und negativ geladenen Elementarteilchen nicht identisch, so ist es elektisch geladen und wird als [[ Ion ]] bezeichnet. Das gleiche gilt für elektrisch geladene Körper. Negativ geladene Körper enthalten mehr [[ Elektronen ]] als Protonen und bei positiv geladenen Körpern ist es umgekehrt.

Negativ geladene Ionen nennt man [[ Anionen ]].

Positiv geladene Ionen nennt man [[ Kationen ]]

Beispiele:

Kohlenstoff mit 7 Elektronen ist elektrisch einfach [[ negativ ]] geladen. 

Germanium mit 34 Elektronen ist elektrisch [[ zwei ]]-fach [[ negativ ]] geladen.

__Übung:__

<iframe src="https://learningapps.org/watch?app=21709772" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>


### 5.1.3 Qualitative Beschreibung der Kräfte zwischen elektrisch geladenen Körpern

> Zwischen zwei elektrisch geladenen Körpern K1 und K2 wirken elektrische Kräfte $\vec{F_{el}}$. 
>
> Die Richtung der Kraftvektoren ist __entlang__ der Verbindungslinie beider Körper.
>
> Je nach Vorzeichen der Ladung sind die Kräfte anziehend oder abstoßend.

<span style="color:orange"> _Ergänze die wirkenden Kräfte als Kraftpfeile. Übernimm die Zeichnung in deinen Hefter._</span>
![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/Bwpb4qQF7jRzHYk/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

<details>

<summary> Lösung </summary>

![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/3bj6ESWb8DdS5m3/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

</details>

### 5.1.4 Berechnen der Kräfte zwischen elektrisch geladenen Körpern (quantitativ)

> Der Betrag der elektrischen Kraft $ F_{el}$ zwischen zwei elektrisch geladenen Körper $K1$ und $K2$ mit den Ladungen $Q_1$ bzw. $Q_2$, welche sich im Abstand r zueinander befinden, ist definiert als:
>
> __Coulomb'sches Gesetz:__
>
> | $$ \boxed{F_{el} = \frac{1}{4\cdot \pi \cdot \varepsilon_0} \cdot \frac{Q_1 \cdot Q_2}{r^2}} $$ | ![Kraefte](https://diversewolken.ddns.net/nextcloud/index.php/s/4zwL8NcGmoGwmAW/download) |
>
> $\hspace{1cm}$ $\varepsilon_0$ ... elektrische Feldkonstante $\boxed{\varepsilon_0 = 8,854 \cdot 10^{-12}\,\dfrac{A\cdot s}{V \cdot m}}$

#### Aufgabe zu 5.1

Der Atomkern eines Heliumatoms (ohne Elektronen) wird als $\alpha$-Teilchen bezeichnet. In der folgenden Aufgabe befinden sich zwei $\alpha$-Teilchen ruhend im Vakuum im Abstand von 5 µm.

1. Geben Sie die elektrische Ladung des $\alpha$-Teilchens in der Einheit Coulomb an.

@rangeQuiz2($\hspace{1cm}$ $Q_{\alpha}$, 3.204e-19 ,$C$)

<details style="margin-left:10%">

<summary> Hinweis </summary>

Überprüfe die Anzahl der Ladungsträger in einem Heliumkern.

</details>

---

2. Ermitteln Sie die Masse eines $\alpha$-Teilchens.

@rangeQuiz2($\hspace{1cm}$ $m_{\alpha}$, 6.644e-27 ,$kg$)

<details style="margin-left:10%">

<summary> Hinweis </summary>

Überprüfe die Masse des Teilchens in der Formelsammlung.

</details>

---

3. Nennen Sie die Art des Ions bei einem $\alpha$-Teilchen.

<div style="margin-left:10%">
[[ Kation ]]
</div>

---

4. Geben Sie den Abstand der beiden Teilchen in der Einheit Meter an.

@rangeQuiz2($\hspace{1cm}$ $r$, 5e-6 ,$m$)

---

5. Nennen Sie die Art der Kraftwirkung zwischen den $\alpha$-Teilchen.

<div style="margin-left:10%">
[( )] keine Kraftwirkung
[( )] anziehende Kraftwirkung
[(x)] abstoßende Kraftwirkung
</div>

---

6. Berechnen Sie den Betrag der elektrischen Kraft, die auf jedes $\alpha$-Teilchen wirkt.

@rangeQuiz2( $\hspace{1cm}$ $F_{el}$, 3.68E-17 , $N$)

<details style="margin-left:10%">

<summary> Hinweis </summary>

Nutze die Formel für die elektrische Kraft zwischen zwei Ladungen.

</details>

---

7. Beschreiben Sie wie sich die $\alpha$-Teilchen bewegen.

<details style="margin-left:10%">

<summary> Antwort </summary>

Durch die abstoßende Kraftwirkung werden die Teilchen voneinander weg beschleunigt.

</details>

---

8. Aufgrund der wirkenden elektrischen Kräfte werden die $\alpha$-Teilchen beschleunigt. Entscheiden Sie, ob es sich dabei um eine gleichmäßig beschleunigte Bewegung handelt. Begründen Sie Ihre Entscheidung.

<details style="margin-left:10%">

<summary> Hinweis </summary>

Überprüfe, ob sich die beschleunigende Kraft während der Bewegung ändert.

</details>


<details style="margin-left:10%">

<summary> Lösung </summary>

Es ist keine gleichmäßig beschleunigte Bewegung, da sich die beschleunigende Kraft mit zunehmendem Abstand (die Teilchen bewegen sich von einander weg) verringert.

</details>

---

9. Ermitteln Sie den Wert der Beschleunigung für die $\alpha$-Teilchen im Abstand $r=5\,\mu m$.

@rangeQuiz2($\hspace{1cm}$ a, 5.541E9 , $\dfrac{m}{s^2}$)

<details style="margin-left:10%">

<summary> Hinweis </summary>

Nutzen Sie das 2. Newton'sche Gesetz zur Ermittlung der Beschleunigung.

</details>

<details style="margin-left:10%">

<summary> Lösung </summary>

-> 2. Newton'sches Gesetz

$$ a = \frac{F}{m} $$

$$ F_{el} = 3,69 \cdot 10^{-17} N\,\mathrm{(siehe\,5.)}$$

Die Masse des $\alpha$-Teilchens beträgt

$$ m_\alpha = 6,64 \cdot 10^{-27} kg $$

</details>


### Einschub: Einheitenvorsätze und 10er-Potenzen

@color(vgl. FS S. 50, orange)

![TB_Einheitenvorzeichen](https://diversewolken.ddns.net/nextcloud/index.php/s/iSnpGbWo5yCkJG9/download)

[GSI_SCRIPT_ELEHRE](https://web-docs.gsi.de/~wolle/TELEKOLLEG/ELEKTRIK/elektrik.html)

## 5.2 Das elektrische Feld

![DasElektrischeFeld](https://web-docs.gsi.de/~wolle/TELEKOLLEG/ELEKTRIK/E-FELD/e-1.jpg)



### 5.2.1 Definition und elektrische Feldlinien

Im Raumbereich um einen __geladenen Körper__ wirkt auf einen anderen geladen Körper eine elektrische __Kraft__ ([Simulation elektrischer Kräfte](https://www.geogebra.org/classic/vbw299uv?embed)).

{{1}}
***********
> Um die Kraftwirkung im gesamten Raum zu __illustrieren__ wird der Begriff <span style="color:orange">elektrisches Feld</span> eingeführt.
***********

{{2}}
***********
> Das __elektrische Feld__ verdeutlicht die Kraftwirkung auf eine <span style="color:orange">positive Probeladung</span>, dargestellt durch <span style="color:orange">Feldlinien.</span> 
***********


{{3}}
***********
__Beispiele für elektrische Felder:__

| Radialfeld<br>(_inhomogenes Feld_) |  Dipolfeld<br>(_inhomogenes Feld_) | Plattenkondensator<br> (homogenes Feld) |
| {4}{![Radialfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/3r6ngsjZkRr4RD6/download)} | {5}{![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)} | {6}{![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)} |
| {4}{einzelne Punktladung} | {5}{zwei ungleichnamige Punktladungen} | {6}{Plattenkondensator} |

***********

{{7}}
***********
__Es gelten folgende Vereinbahrungen:__

- Feldlinien verlaufen von <span style="color:red">__Plus__</span> nach <span style="color:darkgreen">__Minus__</span>.

- die Richtung der Feldlinie gibt die __Kraftrichtung__ auf eine <span style="color:red">__positive Probeladung__</span> an

- je dichter die Feldlinien in einem bestimmten Gebiet, desto größer ist die dort wirkende Kraft

- in einem __homogenen Feld__ (z.B. innerhalb eines Plattenkondensators) ist der Betrag der wirkenden Kraft überall gleich

- elektrische Feldlinien beginnen/enden __senkrecht__ an/auf einer Oberfläche
***********

{{8}}
***********
> __Quellen und Senken elektrischer Felder:__
>
> Elektrische Feldlinien beginnen an positiven Ladungen <span style="color:red">__(Quelle)__</span> und enden an negativen Ladungen <span style="color:darkgreen">__(Senke)__</span>
***********

#### Video zum elektrischen Feld

<p style="color:orange"> Bitte schau dir folgendes Video an. Bis zur Minute 3:00 ist es Wiederholung, dann folgenden Fakten zum elektrischen Feld, welche wir noch nicht besprochen haben. Du kannst es dir zur Information ansehen, musst du aber nicht. </p>

!?[ElektischesFeld](https://www.youtube.com/watch?v=EN6dTZH-HDs)

### 5.2.2 Berechnung des elektrischen Feldes

Die Stärke des elektrischen Feldes $\vec{E}$ berechnet sich aus der Kraft $\vec{F}$ auf eine elektrische Ladung $Q$.

> $$ \vec{E} = \frac{\vec{F_{el}}}{Q} $$
>
> <div style="color:orange">_Hinweis: Die Pfeile über $\vec{E}$ und $\vec{F}$ bedeuten, dass es sich um Vektoren mit einer Richtung und einem Wert (auch Betrag genannt) handelt. Kräfte haben wir bereits als Vektoren gezeichnet._ </div> <br>
>
> Einheit: $$\Big[\dfrac{N}{C} = \dfrac{V}{m}\Big]$$
>
> $\hspace{1cm}$  <div style="color:orange">_Hinweis: $N$ (Newton) ist die Einheit der Kraft und $C$ (Coulomb) ist die Einheit der elektrischen Ladung._ </div>

### Aufgaben zu 5.2

<div style="color:orange">_Hinweis: Löse folgende Augaben. Du kannst auf das Glühlampensymbol klicken, wenn du Tipps benötigst, auch mehrfach._ </div>

1. Die Erde bestitz in zur Oberfläche gerichtetes elektrisches Feld, das an der Oberfläche eine Stärke von $ 130 \dfrac{N}{C} $ besitzt.

1. 1. Welches Vorzeichen hat die demzufolge die Ladung der Erde.

        <!-- data-solution-button="off" -->
        [( )] positiv
        [(X)] negativ
        [( )] kann man nicht sagen
        [[?]] Achte auf die Richtung der Feldlinien im Aufgabentext. Vergleiche die Richtung mit der Richtungsvorgabe für Feldlinien (siehe 1.2)
        [[?]] Feldlinien beginnen bei positiven und enden bei negativen Ladungen

---


1. 2. Eine Tischtennisball mit einer metallischen Oberfläche sei elektrisch negativ aufgeladen. Entscheide, ob der Tischtennisball von der Erde abgestoßen oder angezogen wird.

        <!-- data-solution-button="off" -->
        [( )] angezogen
        [(X)] abgestoßen
        [[?]] Die Erde ist, wie in 1.1. überlegt negativ geladen. Überprüfe die Kraftwirkung auf den negativ geladenen Tischtennisball.

---

1. 3. Die Ladung des Tischtennisballs beträgt $Q = 0,1\cdot10^{-3} C =  0,1 mC $. Ermittle den Wert der Kraft $\vec{F_{el}}$, mit welche auf den TT-Ball wirkt.<br>(_Hinweis: Zwischen Zahl und Einheit bitte kein Leerzeichen._)

        [[ 0,013N ]]
        [[?]] Die Formel zur Berechnung der Kraft findest du in Abschnitt 1.2.1.
        [[?]] Stelle die Formel $\vec{E} = \frac{\vec{F}}{Q} $ nach $\vec{F}$ um.

---

1. 4. *Der Ball hat eine Masse von 5g. Ermittle die Ladung Q, die er haben müsste, damit er über dem Erdboden schweben könnte.<br>_Gib die Antwort in der Einheit mC (Millicoulomb) an. Runde auf 2 Kommastellen._

        [[ 0,38mC ]]
        [[?]] Wenn der Ball schweben soll, muss Gewichtskraft $F_g$ und abstoßende elektrische Kraft $F_{el}$ gleich groß sein.
        [[?]] Es gilt: $F_g = m \cdot g$ und $F_{el} = E \cdot Q$.
        [[?]] Umgestellt nach $Q$: $Q=\frac{m \cdot g}{E}$
        [[?]] Lösung $Q = 0,0003773 C \approx 0,38mC$

---

2. Entscheide für die folgenden Felder, um welche Art von Feld es sich handelt.

2. 1. ![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)

        <!-- data-solution-button="off" -->
        [( )] Radialfeld
        [(X)] Dipolfeld
        [( )] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.

---

2. 2. ![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)

        <!-- data-solution-button="off" -->
        [( )] Radialfeld
        [( )] Dipolfeld
        [(X)] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.

---

2. 3. ![Radialfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/3r6ngsjZkRr4RD6/download)

        <!-- data-solution-button="off" -->
        [(X)] Radialfeld
        [( )] Dipolfeld
        [( )] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.


3. Zeichne das elektrische Feld einer positiv geladenen Punktladung, welche zentral vor einer negativ geladenen Kondensatorplatte positioniert ist. Bei Fragen nutze folgende Hinweise.

<details style="margin-left:10%">

<summary> Hinweis: Anordnung der Ladungen </summary>

![Aufgabe_1_L1](https://diversewolken.ddns.net/nextcloud/index.php/s/3mH8ApKdxxj52dJ/download)

</details>

<details style="margin-left:10%">

<summary> Hinweis: Lage der Feldlinien </summary>

![Aufgabe_1_L2](https://diversewolken.ddns.net/nextcloud/index.php/s/DF6TktoF9Xgyg5A/download)

</details>

4. An den acht Ecken eines Würfels mit der Kantenlänge 1 mm ist jeweils ein Proton angeheftet (es ist fest). Ermittle die Feldstärke im Mittelpunkte des Würfels.

<details style="margin-left:10%">

<summary> Hinweis </summary>

Stell dir vor im Mittelpunkt des Würfels würde ein Elektron sitzen.
Überlege dir zunächst die Kraftrichtung, die eins der Protonen auf das Elektron ausübt. Addiere dann die Kraftwirkung des gegenüberliegenden Protons dazu, usw.

</details>

<details style="margin-left:10%">

<summary> Lösung </summary>

Die Feldstärke im Mittelpunkt des Würfels wäre Null, denn die Kräfte auf eine Probeladung heben sich jeweils von den gegenüberliegenden Ecken auf. Somit wirkt auf eine Ladung (z.B. ein Elektron) im Mittelpunkt in der Summe keine Kraft und somit ist auch das elektrische Feld Null.

</details>

5.(*) Leite die Formel für das elektrische Feld einer Punktladung her. 

<details style="margin-left-left:10%">

<summary> Hinweis </summary>

Nutze die allgemeine Gleichung für das das elektrische Feld und setze für die Kraft den Wert der elektrischen Kraft zwischen zwei Ladungen ein.

</details>

### Wie entsteht das elektrische Feld mehrerer Punktladungen

__Kraftwirkung im Radialfeld und im homogenen Feld__

[LEIFI_EFeldlinien](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/grundwissen/elektrisches-feld-und-feldliniendarstellung)

__Überlagerung elektrischer Felder__

[LEIFI_ÜberlagerungenElektrischerFelder](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/grundwissen/ueberlagerung-elektrischer-felder)

__Feldlinienbild mehrerer Ladungen__

??[LEIFI-SIMULATION_FELDLINIEN](https://www.didaktikonline.physik.uni-muenchen.de/programme/e_feld/E_Feld_leifi.html)

### Weitere Aufgaben zu 5.2

@color(__Löse Aufgabe 6. & 7. sowie 8. oder 9.__, blue)

<br>

<br>

6. @color(Quiz zur elektrischen Kraft [_leichte Aufgabe_], darkgreen)

     [Quiz](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/aufgabe/quiz-zur-elektrischen-kraft)

7. @color(Kraft zwischen zwei Ladungen [_leichte Aufgabe_], darkgreen)

     [Aufgabe-zwei-Ladungen](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/aufgabe/kraft-zwischen-zwei-ladungen)

8. @color(Pendel im homogenen elektrischen Feld [mittelschwere Aufgabe], orange)

     _Themen:_ homogenes elektrisches Feld, Kraftvektoren, Kraftzerlegung, Kräftegleichgewicht

     __Fokus: a), b)__

     [Aufgabe-Pendel-Homogenes-Feld](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/aufgabe/auslenkung-im-homogenen-elektrischen-feld)

9. @color(Geladenes Doppelpende [mittelschwere Aufgabe], orange)

     _Themen:_ elektrische Ladung, Kräfte zwischen elektrischen Ladungen, Kraftvektoren, Kräftegleichgewicht

     __Fokus: a)__

     [Aufgabe-Geladenes-Doppelpendel](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/aufgabe/doppelpendel)


## 5.3. Der Kondensator

__Definition:__ Ein Kondenstator ist ein Bauelement zur __Speicherung von elektrischer Ladung__. Er besteht aus zwei leitenden Schichten, die durch einen Isolator (@color(Dielektrikum,orange)) voneinander getrennt sind, darkgrey).

Einfachste Bauform: @color(__Plattenkondensator__, orange) 


![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

{{1}}
*******
__Eigenschaften eines Plattenkondensators:__

- auf den beiden Platten eines Plattenkondensators werden __elektrische Ladungen $Q$__ gespeichert
*******

{{2}}
*******
- __das elektrische Feld__ zwischen den Platten ist @color(homogen, orange), d.h. es hat an jedem Punkt dieselbe Feldstärke $\vec{E}$
*******

{{3}}
*******
- __die Feldlinien__ zeigen von der @color(positiven, red) Platte zur @color(negativen, blue) Platte
*******

{{4}}
*******
- __die elektrische Feldstärke__ $\vec{E}$ innerhalb eines Plattenkondensators berechnet sich mit
*******

{{5}}
*******
> $$ \boxed{\vec{E} = \dfrac{U}{d}} $$
>
> $\hspace{1cm}$ $U$ ... Spannung zwischen den Platten $\big[ V \big]$ 
>
> $\hspace{1cm}$ $d$ ... Abstand der Platten $\big[ m \big]$ 

- wird in das elektrische Feld eine elektrische Ladung eingebracht, so wirkt auf die Ladung eine elektrische Kraft die mit $\vec{F_{el}}=\vec{E}\cdot q$ berechnet werden kann
*******

### Aufgaben zu 5.3

1. __Elektrisches Feld und elektrische Ladung__ <br> Der Kern eines Helium-Atoms enthält vier Elementarteilchen: zwei Protonen und zwei Neutronen. <br> Man nennt diesen Kern α-Teilchen (Elektronen sind hier nicht enthalten).

1.1. Geben Sie die elektrische Ladung $q_α$ und die Masse $m_α$ eines solchen Alpha-Teilchens an.

<p style="margin-left:10%">

@rangeQuiz2($q_{\alpha}$, 3.204e-19 , $C$)

@rangeQuiz2($m_{\alpha}$, 6.645e-27 , $kg$)

</p>

---

1.2. Zeichnen Sie das elektrische Feld eines einzelnen Alpha-Teilchens. Sie können das Alpha-Teilchen als Kugel betrachten, die Elementarteilchen müssen nicht extra gezeichnet werden.

<details style="margin-left:10%">

<summary> Lösung </summary>

-> siehe Radialfeld

</details>

---

1.3. Notieren Sie die Art des elektrischen Feldes. Begründen Sie Ihre Aussage anhand 4.2.

<p style="margin-left:10%">

Feldform: [[ Radialfeld ]]

Feldart: [[ inhomogen ]]

</p>

---
2. __Elektronenröhre__ <br> Elektronenröhren sind sehr nützliche elektronische Bauelemente, welche entscheidend für die Entwicklung der ersten Computer Waren. Eine Elektronenröhre ähnelt einem einem kleinen Plattenkondensator, welcher sich Inneren einer evakuierten Glaskugel befindet. Abb.1 zeigt eine stark vereinfachte seitliche Skizze. Dabei ist der negative Pol der Spannungsquelle an die Kathode angeschlossen und der positive Teil an die Anode. ![Elektronenröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/27yGykN3XxZ27gJ/download "Abb.1: Schema Elektronenröhre") 

2.1. Zeichnen Sie die elektrischen Feldlinien in die Skizze ein.

2.2. Erläutern Sie qualitativ, was mit einem Elektron geschieht, welches zwischen Kathode und Anode befindet.

2.3. Ermitteln Sie den Wert der elektrischen Feldstärke zwischen Kathode und Anode. 

@rangeQuiz2($\hspace{1cm}$  $E_{el}$, 40000, $\frac{V}{m}$)

2.4. Im Betrieb wird die Kathode geheizt und Elektronen treten mit ca. 2∙10⁶ m/s aus der Kathode aus. Ermitteln Sie die Geschwindigkeit, welche ein Elektron an der Anode besitzt.

@rangeQuiz2($\hspace{1cm}$  $v$, 8.61e6, $\frac{m}{s}$)

<details>

<summary> Hilfestellung zur Lösung </summary>

Stellen Sie die Bewegungsgleichung für das Elektron auf. Ermitteln Sie aus dem zweiten Newton'schen Gesetz die Beschleunigung.

</details>

<details>

<summary> Lösungsweg1 </summary>

![Lsg_2.4](https://diversewolken.ddns.net/nextcloud/index.php/s/Xas4Gr5sMZYsLGP/download)

</details>

### 5.3.1 Demonstrationsexperiment - Metallischer TT-Ball zwischen Kondensatorplatten

![TB_TT_Ball_Kondensator1](https://diversewolken.ddns.net/nextcloud/index.php/s/CHp3Z5AZi6FnyFy/download)

![TB_TT_Ball_Kondensator2](https://diversewolken.ddns.net/nextcloud/index.php/s/RFGE7nr44G3qjEs/download)

![TB_TT_Ball_Kondensator3](https://diversewolken.ddns.net/nextcloud/index.php/s/axm4xbD5AwT4ock/download)

<details>

<summary> Foto vom Aufbau </summary>

![Foto_TT_Ball_Kondesator](https://diversewolken.ddns.net/nextcloud/index.php/s/XGmC5NgE4zEo3T7/download)

</details>

## 5.4. Die Kapazität

__Definition:__ Die @color(Kapazität, orange) eines Kondensators beschreibt seine Fähigkeit eine __Ladungsmenge Q__ zu speichern, wenn eine bestimmte __Spannung U__ angelegt wird.

{{1}}
*********
> __Formel:__ 
>
> $$ \boxed{ C = \dfrac{Q}{U} } $$
>
> $\hspace{1cm}$ $C$ ... Kapazität  
>
> $\hspace{1cm}$ $Q$ ... im Kondensator gespeicherte Ladung $\big[ C \big]$ 
>
> $\hspace{1cm}$ @color(_Hinweis: Im folgenden werden wir den Buchstaben **Q** für die Ladung auf dem Kondensator und den Buchstaben **q** für die Ladung eines Teilchens im elektrischen Feld verwenden_, orange)
>
> $\hspace{1cm}$ $U$ ... angelegte Spannung $\big[ V \big]$ 
*********

{{2}}
*********
> __Einheit der Kapazität:__  $$\textbf{1 Farad = 1 F}$$
>
> $$\Big[ F = \dfrac{C}{V} \Big] $$
*********

{{3}}
*********
> _Für die einfachste Bauform eines Kondensators [siehe 5.3](#5.3.-der-kondensator) kann man die Kapazität wie folgt berechnen:_
> 
> __Kapazität eines @color(Plattenkondensators, orange):__
>
> $$ \boxed{ C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} } $$
>
> <p style="text-align:center">[Formelsammlung](https://www.iqb.hu-berlin.de/abitur/abitur/dokumente/naturwissenschaften/N_Mathematischna.pdf) (S.28+54)</p>
*********

{{4}}
*********
> $\hspace{1cm}$ $C$ ... Kapazität  
>
> $\hspace{1cm}$ $\varepsilon_0$ ... elektrische Feldkonstante $\boxed{\varepsilon_0 = 8,854 \cdot 10^{-12}\,\dfrac{A\cdot s}{V \cdot m}}$
>
> $\hspace{1cm}$ $\varepsilon_r$ ... Dielektrizitätszahl [Einheitenlos] @color( - Luft/Vakuum: $\varepsilon_r=1$,blue)
>
> $\hspace{1cm}$ $A$ ... Flächeninhalt der Platte $[m^2]$
>
> $\hspace{1cm}$ $d$ ... Abstand der Platten $[m]$
*********

{{5}}
*********
__Beispiel:__ _Ermittle die Kapazität des Plattenkondensators auf dem Lehrertisch. Komm dazu in kleiner Gruppe nach vorn und bestimme die notwendigen Werte._
*********

{{6}}
*********
<p class="newspaper">

geg.:

<div style="text-indent:10%">

$A$ = <bdi style="color:orange"> $28\,cm \cdot 28\,cm = 0,28 \cdot 0,28\,m^2 = 0,0784 m^2$</bdi>

$d$  <bdi style="color:orange"> $\approx 1,5\,cm = 0,015 m$ </bdi>

$\varepsilon_r$ = <bdi style="color:orange"> $ = 1$ </bdi>

</div>

ges.:

<div style="text-indent:10%">

$C$

</div>

<p class="cb">

Lsg.:

<div style="text-indent:10%">

$C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} $

$C \approx $  <bdi style="color:orange"> $ 4,6 \cdot 10^{-11} F $ = $ 46\,pF$  </bdi>

<bdi style="color:orange">Lösungen $ C = 2 \cdot 10^{-11}\,F$ bis $ 8 \cdot 10^{-11}\,F $ sind akzeptabel</bdi>

Beispiel: Taschenrechner:

![GTR](https://diversewolken.ddns.net/nextcloud/index.php/s/939gMiCMEoNn7bL/download)<!-- style="width:80%" -->

</div>

</p>

</p>

*********

### Aufgabe zu 5.3/5.4

3. __Wolkenkondensator__ ![Wolkenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/F3xsbZknJ3PPqme/download) Eine positiv geladene Wolke in 400 m Höhe bildet zusammen mit dem Erdboden einen Plattenkondensator (Fläche einer „Platte“ 8,0 km²). Läd sich die elektrisch Wolke auf, so entsteht zwischen Wolke und Erdboden ein elektrisches Feld. Die elektrische Feldstärke ist in dieser Aufgabe 1,2∙10⁵ V/m, was so hoch ist, dass eine Entladung durch die Luft (Blitz) unmittelbar bevorsteht.

---

3.1. Zeigen Sie, dass die Spannung zwischen der Wolke und dem Boden etwa 50 Millionen Volt beträgt. Bestimmen Sie den genauen Wert.

@rangeQuiz2($ \hspace{1cm}$ $U$, 48e6, $V$)

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_3_1](https://diversewolken.ddns.net/nextcloud/index.php/s/WCbLJTRp7Z22fG7/download)

</details>

---

3.2. Ermitteln Sie die Ladung, die sich in den Wolken befindet.

@rangeQuiz2($ \hspace{1cm}$ $Q$, 8.5 , $C$)

<details style="margin-left:10%">

<summary>Zwischenergebnisse</summary>

@rangeQuiz2( $C$ , 1.77e-7, $F$)

</details>

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_3_2](https://diversewolken.ddns.net/nextcloud/index.php/s/od6j7Cpr8a5bPRX/download)

</details>

---

3.3. Ermittle die Ladung $q$, die ein kugelförmiges Wassertröpfchen mit 2,0 mm Durchmesser haben müsste, wenn es vor Entladung der Wolke zwischen dieser und der Erde bei Windstille gerade schweben würde? <br> (Der Auftrieb in Luft ist zu vernachlässigen.)

@rangeQuiz2($ \hspace{1cm}$ $q$, 3.42E-10 , $C$)

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_3_3](https://diversewolken.ddns.net/nextcloud/index.php/s/a3nHxzzENECm5GX/download)

</details>

---

3.4. Wie lange würde die Entladung der Wolke dauern, wenn die mittlere Stromstärke des Blitzes 4,0 kA betragen würde?

@rangeQuiz2($ \hspace{1cm}$ $t$, 2.1e-3 , $s$)

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_3_4](https://diversewolken.ddns.net/nextcloud/index.php/s/HLGPAkXt3TwCE5H/download)

</details>

---

3.5. Noch bevor es zu einer Entladung kommt, drückt ein Fallwind die Wolke auf eine niedrigere Höhe herab. Die Ladung der Wolke bleibe dabei konstant. <br> Wie ändert sich qualitativ die elektrische Feldstärke zwischen Wolke und Erde? Wird eine Entladung der Wolke dadurch wahrscheinlicher? <br> Geben Sie eine kurze Begründung.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_3_5](https://diversewolken.ddns.net/nextcloud/index.php/s/4ZegS5AXFdZgXwY/download)

</details>


## 5.5 Energie im elektrischen Feld

> Im elektrischen Feld eines Kondensators ist Energie gespeichert und wird als __elektrische Feldenergie $E_{Feld}$__  bezeichnet.
>
> $$ \boxed{E_{Feld} = \frac{1}{2}\cdot Q \cdot U} $$
>
> $$ \boxed{E_{Feld} = \frac{1}{2}\cdot C \cdot U^2} $$
>
> $\hspace{1cm}$ $C$ ... Kapazität des Kondensators $\big[ F \big]$
>
> $\hspace{1cm}$ $Q$ ... im dem Kondensator gespeicherte Ladung $\big[ C \big]$
>
> $\hspace{1cm}$ $U$ ... am Kondensator anliegende Spannung $\big[ V \big]$

### Aufgabe 5: Feldenergie im Kondensator

5.1. Ergänze folgende Aussage: Um die Feldenergie eines Kondensators zu erhöhen kann man:

     <!-- data-solution-button="off" -->
     [[ ]] die Spannung verringern
     [[X]] die Spannung erhöhen
     [[X]] ein Dielektrikum zwischen die Platten des Kondensators einbringen
     [[ ]] ein Dielektrikum zwischen den Platten des Kondensators entfernen
     [[ ]] die elektrische Feldenergie ist eine Konstante und kann nicht verändert werden
     [[?]] Nutze die zweite Formel für die Feldenergie. Überprüfe ob eine Veränderung von Spannung und Kapazität die elektrische Feldenergie vergrößert oder verkleinert. Überprüfe auch die Formel zur Berechnung der Kapazität und den Einfluss eines Dielektrikums.

5. 2. Ergänze folgende Aussage: Wird bei einem Kondensator mit einer festen Kapazität die Spannung verdoppelt so

     <!-- data-solution-button="off" -->
     [(X)] verdoppelt sich die Feldenergie
     [( )] vervierfacht sich die Feldenergie
     [( )] bleibt die Feldenergie gleich
     [( )] halbiert sich die Feldenergie
     [( )] viertelt sich die Feldenergie
     [[?]] Nutze die zweite Formel für die Feldenergie. Wähle Beispielwerte für die Spannung und Kapazität. Verdopple die Spannung und überprüfe den Einfluss auf das Ergebnis

5. 3. Wahr oder falsch? Bringt man die Platten eines Kondensators näher zusammen, steigt die Kapazität.

     <!-- data-solution-button="off" -->
     [(X)] wahr
     [( )] falsch

5. 4. Wahr oder falsch? Verkleinert man die Plattenfläche eines Kondensators so steigt die Kapazität.

     <!-- data-solution-button="off" -->
     [( )] wahr
     [(X)] falsch

5. 5. An einem Plattenkondensator ($A$ ... Flächeninhalt der Platte, $d$ ... Abstand der Platten, Luft zwischen den Platten), soll eine feste Spannung $U$ angelegt werden. Markiere die Formel zur Berechnung der Ladung $Q$ auf den Platten.

     <!-- data-solution-button="off" -->
     [( )] $Q = \dfrac{\varepsilon_0 \cdot \varepsilon_r \cdot A}{d \cdot U} $
     [( )] $Q = \varepsilon_0 \cdot \varepsilon_r \cdot A \cdot d \cdot U $
     [( )] $Q = \dfrac{d \cdot U}{\varepsilon_0 \cdot \varepsilon_r \cdot A} $
     [( )] $Q = \dfrac{d}{\varepsilon_0 \cdot \varepsilon_r \cdot A \cdot U} $
     [(X)] $Q = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} \cdot U $     
     [[?]] Nutze die allgemeine Formel für die Kapazität ([5.4](#5.4.-die-kapazität)) und die spezielle Formel für die Kapazität des Plattenkondensators.
     [[?]] Setze beide Formeln gleich und stelle sie nach der Ladung $Q$ um

5. 6. Ein Plattenkondensator der zwischen den Platten mit Luft gefüllt ist hat eine Kapazität von 1 nF. Dann wird ein Stoff zwischen die Platten geschoben und die Kapazität erhöht sich auf den Wert 2,3 nF. Benenne den Stoff, der zwischen die Platten geschoben wurde.

     <!-- data-solution-button="off" -->
     [[ Paraffin ]]
     [[?]] Überprüfe in der Formel zur Berechnung der Kapazität eines Plattenkondensators [-> 1.4], welche physikalische Größe sich auf ein Material bezieht.
     [[?]] Das Material zwischen den Platten wird durch die Dielektizitätszahl $\varepsilon_r$ repräsentiert. Nutze die Formelsammlung für die Dielektrizitätszahl verschiedener Materialen.
     [[?]] Die Dielektrizitätszahl verschiedener Materialien wird in der Formelsammlung auf Seite 54 aufgeführt. Überprüfe, welches Material eine Dielektrizitätszahl von 4 besitzt.


5. 7. [LEIFI-Quiz zur Kondensatorformel](https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/aufgabe/quiz-zur-kondensatorformel)


## 5.6.1 Sim1 Elektronische Schaltkreise mit Kondesatoren

??[PhET-Kondensator1](https://phet.colorado.edu/sims/html/capacitor-lab-basics/latest/capacitor-lab-basics_all.html?locale=de)


## 5.6.2 Sim2 Elektronische Schaltkreise mit Kondensatoren

??[PhET-Kondensator2](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac/latest/circuit-construction-kit-ac_all.html?locale=de)


## 5.7 Elektronische Schaltkreise mit Kondensatoren

@color(_Hinweis: Für die folgenden Unterrichtseinheiten werden wir mit dem Formelzeichen $Q$ immer die Ladung auf den Platten des Kondensators bezeichnen._,darkgrey) 

<br>

__Wiederholung:__ Schließen wir den Kondensator an eine Gleichspannungsquelle (Spannung $U-$) an, so fließen elektrische Ladungen auf den Kondensator. Im Kondensator wird die Ladungsmenge $Q$ gespeichert.



<p class="newspaper">

{{1}}
***********

__Ladung $Q$__

<p style="margin-left:5%">

Die Ladung $Q$ beschreibt Anzahl überzähliger Elemtarladungen $e$.

_Einheit: 1C (1 Coulomb)_

$$ \boxed{1 e = 1,6 \cdot 10^{-19} C} \,\,\,\mathrm{oder}\,\,\, \boxed{1C = 6,24 \cdot 10^{18} e}$$

</p>

---

***********

{{2}}
***************

__Spannung $U$__


<p style="margin-left:5%">

Die Spannung $U$ beschreibt den @color(das Potential bzw. den Antrieb für das Fließen von Ladungsträgern, orange). 
Je größer die Spannung, desto größer ist die gespeicherte Ladung.

_Einheit: 1V (1 Volt)_

</p>

---

***************

{{3}}
***************

__Stromstärke $I$__

<p style="margin-left:5%">

Die Stromstärke $I$ beschreibt <bdi style="color:orange">die Menge der elektrischen Ladungen $Q$, die pro Sekunde durch einen Leiterquerschnitt fließen</bdi>.

_Einheit: 1A (1 Ampere)_

_Eine Stromstärke von 1A bedeutet, dass pro Sekunde eine Ladung von 1 C fließt._

$$ \Big[ A = \frac{C}{s} \Big] $$

</p>

--- 

***************

{{4}}
***************

__Gespeicherte Energie $E_{Feld}$__

<p style="margin-left:5%">

Die im Kondensator (im elektrischen Feld) gespeicherte Energie $E_{Feld}$ wird berechnet mit

$$ E_{Feld} = \frac{1}{2}\cdot Q \cdot U $$

$$ E_{Feld} = \frac{1}{2}\cdot C \cdot U^2 $$

_Einheit: 1J (1Joule)_

</p>

***************



<p class="cb">

__Schaltplan zum Laden des Kondensators__

![Schaltkreis_Kondensator1](https://diversewolken.ddns.net/nextcloud/index.php/s/ARdjFMxTDoDoAWz/download)

</p>

</p>

### Einführungsvideo zu Mobile-Cassy 2

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

### 5.7.1 Experiment: Vorübung zur Schulung mit Cassy

__Aufgabenstellung:__ Nimm mit die U-I-Kennlinie für einen ohmschen Widerstand ($R=512\Omega$) auf. Variiere die Spannung in Schritten von 1 V im Intervall 0 - 10 V.


<p style="color:blue">

__Durchführung:__ _(muss nicht notiert werden)_ 

1. Übernimm Überschrift und Aufgabenstellung auf eine neue Seite.

2. Übernimm den Schaltplan und die zugehörige Tabelle für die Messwerte.

3. Stelle das Cassy-Messgerät anhand der Erklärungen ein.

4. Variiere die Spannung an der Spannungsquelle von 0..10V in Schritten von 1 V. Notiere Spannung und Stromstärke an Cassy-Messgerät.

5. Zeichne eine U-I-Kennlinie: Zeichne dazu ein Diagramm (x-Achse: U in V | y-Achse: I in A).

6. Öffne die nächste Seite: @color(_5.7.2 Automatische Messwert-Erfassung mit Cassy_,darkgreen). Folge den Anweisungen und wiederhole die Messung mit einer Automatischen Messwert-Aufname.

</p>

<p class="newspaper">

__Schaltkreis:__

![Schaltkreis_Exp1](https://diversewolken.ddns.net/nextcloud/index.php/s/rAwYZqysffqknd6/download)

{{0-1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | |
| 1 | |
| 2 | |
| .. | |
| 9 | |
| 10 | |
************

{{1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | 0,002 |
| 1 | 0,004 |
| 2 | 0,006 |
| 3 | 0,008 |
| ..| .. |
| 9 | 0,018 |
| 10 | 0,02 |
************

<p class="cb">

__Diagramm Kennlinie:__

{{0-1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/Z9at8rKH75N4Agt/download)
*************

{{1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/ztd7ScndfNAYNqM/download)
*************

<details  style="color:blue">

<summary>__Einstellen des Cassy-Messgerätes:__</summary>

_(muss nicht notiert werden)_

1. Schließe den blauen Anschluss (_I_) an den Minuspol der Spannungsquelle. Der schwarze Anschluss wird an den Widerstand angeschlossen.

2. Schalte das Cassy-Messgerät ein. Im oberen linken Bereich des Fensters sind die messbaren Größen dargestellt. Deaktiviere mit [Cursor-Rad + OK] die Spannung und aktiviere die Stromstärke.

![VGl-Cassy1](https://diversewolken.ddns.net/nextcloud/index.php/s/e7eaHcHB4YkGf95/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Klicke auf das Symbol für Stromstärke (I) und stelle für den (Mess-)Bereich [-0,03A .. 0,03A] ein. Wechsle zurück Anzeige der Stromstärke. Achte auf: __Nullpunkt links__.

![VGl-Cassy2](https://diversewolken.ddns.net/nextcloud/index.php/s/JiSJbjqy3SkS2CN/download)<!-- style="max-width:80%;margin-left:10%" -->

</details>

</p>

</p>

### 5.7.2 Automatische Messwerterfassung mit Cassy:

In dieser Messreihe wird die Kennlinie vom Cassy-Messgerät automatisch aufgenommen.

1. Schalte die Spannungsquelle ab.

2. Verbinde mit einem weiteren Kabel den @color(roten Pol __U__, red) des Cassy-Gerätes mit einem Kontakt hinter dem Widerstand.

![VGl-Cassy3](https://diversewolken.ddns.net/nextcloud/index.php/s/LxJxpcGsAmAeJJt/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Erweitere deine angezeigten Messwerte auf Spannung U und Stromstärke I. Achte auf __Bereich 0V .. 10V__ und __Nullpunkt links__.

![VGl-Cassy4](https://diversewolken.ddns.net/nextcloud/index.php/s/sXkCT7eGYWyrCYX/download)<!-- style="max-width:80%;margin-left:10%" -->

4. Wechsle zur Anzeige von Spannung und Stromstärke. Schalte die Spannungsquelle ein und vergleiche drei Messwertpaare der angezeigten Daten mit den Daten deiner Messwerttabelle (oben). <br> @color(Stimmen sie überein, red) nimmt Cassy nun korrekt Spannung und Stromstärke auf.

5. Stelle die Spannung an der Spannungsquelle auf 0 V.

6. Wähle nun oben rechts den __Diagramm Modus__. Stelle für die x-Achse die Spannung und für die y-Achse die Stromstärke ein. 

![VGl-Cassy5](https://diversewolken.ddns.net/nextcloud/index.php/s/4nJbMTEEjwz3SJd/download)<!-- style="max-width:80%;margin-left:10%" -->

7. Starte die automatische Messwerterfassung -> Wechsel auf Uhr oben links. 

![VGl-Cassy6](https://diversewolken.ddns.net/nextcloud/index.php/s/cHFbdz2ZQJGFTsE/download)<!-- style="max-width:80%;margin-left:10%" -->

8. Drehe die Spannung an der Spannungsquelle langsam von 0 V -> 10 V und beobache die dargestellten Messwerte. Vergleiche deine Darstellung mit dem hier gezeigten Erwartungsbild.

![VGl-Cassy7](https://diversewolken.ddns.net/nextcloud/index.php/s/f93rWiDbtDkR6Jj/download)<!-- style="max-width:80%;margin-left:10%" -->

9. @color(Dieses Diagramm und dein Messwertdiagramm sollten übereinstimmen., red)


## 5.8 Lade und Entladevorgang eines Kondensators

@uhr

<p style="color:blue; margin-right:200px">

Ziel der folgenden Einheit ist die __theoretische, simulierte und experimentelle__ Untersuchung des Ladevorgangs an einem Kondensator.

{{1}}
********
1. __Theorie:__ Schaltplan, physikalische Größen, theoretische Beschreibung
********

{{2}}
********
2. __Simulation:__ Konstruktion des Schaltplans in einer Simulation, Untersuchung der Entladekurve und Einfluss der physikalischen Größen.
********

{{3}}
********
3. __Experiment:__ Aufbau der Schaltung. Messung der relevanten Daten und deren Verarbeitung mit Tablet oder Laptop.
********

{{4}}
********
4. __Auswertung:__ Auswertung der Messungen. Vergleich der experimentelle Daten mit theoretischen und simulierten Ergebnissen.
********

</p>


### 5.8.1 Theoretische Beschreibung des Lade- und Entladevorgangs an einem Kondensator

__Schaltplan:__ Lade- und Entladevorgang eines Kondensators

<p class="newspaper3">

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/TGLpw4dssYj6WQ3/download)

<p class="cb">

@color(__Aufladen des Kondensators__, darkgreen)

- wird der Ladekreis geschlossen, so fließen elektrische Ladungen von den Polen auf die Platten des Kondensators <br> @color(-> die Ladung $Q$ auf den Kondensatorplatten wird größer, orange)

- für den zeitlichen Verlauf von Spannung $U(t)$ und Stromstärke $I(t)$ gilt: <br> <br> $ \boxed{U(t) = U_0 \cdot \Big[ 1-e^{-\frac{1}{R\cdot C}\cdot t} \Big] }$ <br> <br>  $\boxed{ I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t}} $ <br> <br>  $ \boxed{I_0 = \dfrac{U_0}{R}} $

- $U_0$ .. Ladespannung

<p style="margin-left:15%">
![Ladekurven](https://diversewolken.ddns.net/nextcloud/index.php/s/fdwCnPzcogDqriE/download)<!--style="max-width:70%" -->
</p>

<p class="cb">

@color(__Entladen des Kondensators__, purple)

- wird der Entladekreis geschlossen, so wirkt der Kondensator wie eine kurzzeitige Spannungsquelle <br> @color(-> mit sinkender Ladungszahl sinken Spannung und Stromstärke, orange)

- für den zeitlichen Verlauf von Spannung $U(t)$ und Stromstärke $I(t)$ gilt: <br> <br> $ \boxed{U(t) = U_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t}} $ <br> <br> $ \boxed{I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t}} $ <br> <br> $ \boxed{I_0 = \dfrac{U_0}{R}}$

- $U_0$ .. Spannung am Kondensator zum Zeitpunkt t=0

<p style="margin-left:15%">
![EntLadekurven](https://diversewolken.ddns.net/nextcloud/index.php/s/xBsiTSYozHKMNs4/download)<!--style="max-width:70%" -->
</p>

</p>

</p>

</p>

### 5.8.2 Der Zusammenhang von geflossener Ladung $Q$, Zeit $t$ und momentaner Stromstärke $I(t)$

<p class="newspaper3">

__Grundlage__

{{1}}
**********
_Stromstärke ist definiert als geflossene Ladung je Zeitintervall._
**********

{{2}}
**********
Die momentane Stromstärke $I(t)$ zum Zeitpunkt $t$ ergibt sich aus der geflossenen Ladungsmenge $\mathrm{d}Q$ im Zeitintervall $\mathrm{d}t$.

$$ \boxed{I(t) = \dfrac{\mathrm{d}Q}{\mathrm{d}t}} $$
**********

<p class="cb">

__Darstellung im $I(t)$-Diagramm__

{{3-4}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/Q9MwZdw5ZxwfrcN/download)<!-- style="max-width:80%; margin:5%"-->
*****

{{4}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/GSN44xxcqTH4HH6/download)<!-- style="max-width:80%; margin:5%"-->

Die Fläche unter dem $I(t)$-Diagramm entspricht der im Zeitinverall $T$ geflossenen Ladung $Q$

*****

<p class="cb">

__Theoretische Beschreibung:__


{{5}}
*****
Die im Zeitintervall $T$ geflossene Ladung $Q$ ergibt sich aus dem Integral:

$$ \boxed{ \red{Q_{int}} = \int_0^{\red{T}}{I(t) \mathrm{d}t}} $$
*****


</p>

</p>

</p>

## 5.9 Experiment Entladevorgang eines Kondensators


__Experimentierüberblick__

_Lernziele:_

- Versuchsablauf in Vorbetrachtungen bearbeiten

- sinnvolle Messzeit $T$ für Kombination aus $R$ und $C$ bestimmen

- Cassy mit Tablet verbinden

- Messparameter einstellen lernen (__ohne Trigger__)

- Entladekurve im Cassy automatisiert aufnehmen

- im Zeitintervall T geflossene Ladung bestimmen

- Vergleich der geflossenen Ladung mit theoretischer Berechnung

_Experimentelle Bauelemente:_

- Kondensator $C = 4600 \mu F$, Ohmscher Widerstand $R = 1 k\Omega$

_Anleitungen:_

- Anleitung für Verbindung von Tablet und Cassy

- Anleitung zur Steuerung von Cassy

- Anleitung zum Aufbauen des Versuchs

- Anleitung zur experimentellen Auswertung

- Anleitung zur theoretischen Auswertung


### 5.9.1. Vorbetrachtungen zum Versuch

<p class="newspaper">

__Schaltplan:__

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/JqJRbJpBMJXNwTq/download)

<p class="cb">

__Ladekreis__ 

Der Kondensator wird in dieser Schaltung direkt über die Spannungsquelle und @color(ohne ohmschen Widerstand, red) aufgeladen.

@color(-> siehe Abschnitt _Laden des Kondesators_, orange)
<br>

__Entladekreis:__

Wird der Entladekreis geschlossen, fließt die auf dem Kondensator gespeicherte Ladung $Q$ über den ohmschen Widerstand $R$ ab. Dabei wird mit der elektronischen Messwerterfassung _Cassy_ der Entladestrom $I(t)$ aufgenommen. Die gesamte Messzeit wird mit $T$ bezeichnet (s.u.).

@color(-> siehe Abschnitt _Ermittlung einer sinvollen Messzeit T_, orange)
<br>


{{1}}
*****
__Ermittlung der Ladung $\,Q$:__

Die vom Kondensator abgeflossene Ladung $Q$ entspricht im @color(Zeit-Stromstärke-Diagramm, blue) der <bdi style="color:red"> __Fläche unter dem Graphen $I(t)$__</bdi>.
*****

{{1-2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/Q9MwZdw5ZxwfrcN/download)<!-- style="max-width:80%; margin:5%"-->
*****

{{2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/GSN44xxcqTH4HH6/download)<!-- style="max-width:80%; margin:5%"-->

<bdi style="color:orange">->siehe Abschnitt _Auswertung der Messkurve $I(t)$_</bdi>
<br>

*****

</p>

</p>

### 5.9.2. Berechnung: Laden des Kondensators

@color(Ergänzen Sie hier die fehlenden Werte und notieren Sie sich die grundlegenden Fakten, blue)

_Vorüberlegung:_

Der Kondensator soll zunächst mit der Ladespannung

$$ U = 10 V $$ 

aufgeladen werden. Mit Hilfe der gegebenen Kapazität $C$, lässt sich die Ladung auf dem Kondensator $Q_{lad}$ berechenen.

<br>

<p style="margin-left:10%">

@rangeQuiz2($Q_{lad}$, 0.046 ,$C$)

<details>

<summary> Lösung </summary>

$Q_{lad} = C \cdot U = 4600 \cdot 10^{-6} \cdot 10 V = 0,046 C$



</details>

</p>

### 5.9.3. Ermittlung einer sinnvollen Messzeit $T$

Für die Kombination aus Kondensator (Kapazität $C$) und ohmscher Widerstand (Widerstand $R$) kann eine Zeitkonstante $\tau$ ermittelt werden: 

$$ \boxed{\tau = R \cdot C} $$

Als Messdauer $T$ für die elektronische Erfassung wird eine Gesamtzeit von @color($4\tau$,red) empfohlen. Nach dieser Zeit sind ca. $98,2\%$  der Gesamtladung Q abgeflossen.

$$ \Rightarrow \boxed{T = 4 \cdot \tau} $$



@color(Aufgabe: Ermitteln und notieren Sie für die vorliegende Kombination aus $R$ und $C$ die Zeitkonstante $\tau$ und daraus eine sinnvolle Entladezeit $T$, blue)

<br>

<br>

<p style="margin-left:10%">

@rangeQuiz2($\tau$,4.6,$s$)

@rangeQuiz2($T$, 18.4, $s$)

<details>

<summary> Lösung </summary>

Für das vorliegende Experiment gilt $R=1000\Omega$ und $C=4600\mu F$.

Demzufolge ergibt sich für die Zeitkonstante $\tau = R \cdot C$

$\tau = 1000 \Omega \cdot 4600 \cdot 10^{-6} F = 4,6 s \hspace{1cm}\Big[ \orange{\Omega} \cdot \green{F} \overset{5.4}{=} \orange{\dfrac{V}{A}} \cdot \green{\dfrac{C}{V}} \overset{C = A\cdot s}{=} s \Big]$

Als Faustregel ergibt sich eine sinnvolle Entladezeit $T=4\cdot\tau$ und somit:

$\boxed{ T = 4 \cdot 4,6s = 18,4 s}$

Damit $98,2\%$ der Ladung vom Kondensator abgeflossen sind, sollte eine Messzeit von $T=18,2s$ genutzt werden.

</details>

</p>

### 5.9.4. Berechnung: Integral der Entladekurve $I(t)$

Die im Zeitintervall $T$ geflossene Ladung $Q$ ergibt sich aus dem Integral:

$$ Q_{int} = \int_0^{T}{I(t) \mathrm{d}t} $$

Ermitteln Sie mit Hilfe des CAS das Integral für die Entladekurve mit Ihrer Messzeit $T$ und den gegebenen experimentellen Werten für $C$ und $R$.

<p style="margin-left:10%">

@rangeQuiz2($Q_{int}$, 0.0452 ,$\ C$)

<details>

<summary> Hinweis 1 </summary>

Um das Integral $ Q_{int} = \int_0^{T}{I(t) \mathrm{d}t} $ mit dem CAS zu berechnen muss sowohl die Messzeit $T$ (siehe vorheriger Abschnitt) und die Funktion $I(t)$ (siehe 5.8.1) bekannt sein. Setzen Sie in $I(t)$ die Werte für $U$,$R$ und $C$ ein und berechnen Sie mit dem CAS $Q_{int}$.
</details>

<details>

<summary> Hinweis 2 </summary>

Eine sinnvolle Messzeit aus dem vorherigen Abschnitt lautet 

$$ T=18,6 s$$

Die Funktion $I(t)$ für die Entladekurve am Kondensator lautet

$$ I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t} $$ 

mit den Werten $R=1000\Omega$, $C=4600\cdot10^{-6}F$ und $I_0=\frac{U}{R}$. Das gesamte Integral für die Ladung $Q_{int}$ lautet:

$$ Q_{int} = \int_0^{T} \frac{U}{R} \cdot e^{-\frac{1}{R\cdot C}\cdot t} \mathrm{d}t $$ 

Bzw. mit Zahlenwerten für den CAS:

$$ Q_{int} = \int_0^{18,6} \frac{10}{1000} \cdot e^{-\frac{1}{1000 \cdot 0,0046}\cdot t} \,\,\mathrm{d}t $$

</details>

<details>

<summary> Lösung im CAS </summary>

Geben Sie folgendes in den CAS ein:

![IntegralLadung_CAS](https://diversewolken.ddns.net/nextcloud/index.php/s/Eaf4zSJBqERerZd/download)

Als Ergebnis ergibt sich:

$\boxed{Q_{int} = 0,0452\,C}$

</details>

</p>

### 5.9.5. Anleitung zur Verbindung von Cassy und Tablet

__Grundlage:__ Jedes __Mobile Cassy 2__-Messgerät (im Folgenden mit _Cassy_ bezeichnet) kann mit Hilfe einer W-Lan Verbindung über das Tablet ferngestuert werden. Dabei können Messparameter eingestellt, Messungen gestartet und Messdaten abgespeichert werden. Hier wird das Tablet mit dem Cassy verbunden.

__Arbeitsablauf:__

- nach Einschalten von _Cassy_ baut das Gerät selbstständig eine W-Lan Verbinung auf

- wechseln Sie auf dem Cassy zum Menu Einstellungen (oben rechts) 

- wählen Sie QR-Code anzeigen, wechseln Sie zu AP_Daten und scannen Sie den angezeigten QR-Code mit dem Tablet -> das Tablet wird sich mit dem Cassy verbinden

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/cbw8JJBd7AAetEz/download)<!-- style="max-width:300px; margin-left:20%"-->

- wenn ihr Tablet mit dem _Cassy_-WLan verbunden ist, öffnen Sie einen neuen Tab im Safari-Webbrowser und öffnen Sie folgende Adresse [http://10.10.10.1](http://10.10.10.1)

![Cassy-WLan](https://diversewolken.ddns.net/nextcloud/index.php/s/zgynA6RKTTEaM4Y/download)<!-- style="max-width:80%; margin:5%"-->

- zu sehen ist die Live-Anzeige des Spannungssensors <br>-> aktivieren Sie am Cassy die Stromstärkemessung und deaktivieren Sie die Spannungsmessung <br> -> Überprüfen Sie die Veränderung auf Ihrem Tablet

![Cassy-WLan2](https://diversewolken.ddns.net/nextcloud/index.php/s/8ZjcN5DZqk6frXw/download)<!-- style="max-width:80%; margin:5%"-->

### 5.9.6. Einstellen der Messparameter am Cassy

__Grundlage:__ Hier werden die Messparameter eingestellt

__Arbeitsablauf:__

- wechseln Sie auf der linken Seite zu Einstellungen

- hier müssen Sie den Messbereich für die Stromstärke einstellen __0,03 A__ und den Nullpunkt (des Diagramms) auf __links__ setzen(_Hinweis: diese Einstellung kann auch im Cassy direkt vorgenommen werden_)

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/KQLjMB5CoYRR34o/download)<!-- style="max-width:80%; margin:5%"-->

- <bdi style="color:red">_Hinweis:_ Da zunächst ohne Trigger [automatischer Auslöser] gearbeitet wird, belassen Sie die _Messzeit_ auf manuell </bdi>

- wechseln Sie auf der linken Seite zu ***Diagramm*** und vergleichen Sie Ihre Anzeige

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9APdepf3in8wQ86/download)<!-- style="max-width:80%; margin:5%"-->

### 5.9.7. Aufbau der Messchaltung

$ \red{\boxed{\mathrm{Es\ muss\ keine\ Gewalt\ angewendet\ werden.}}}$

__Grundlage:__ Für diesen Versuch ist der Schaltplan in den Vorbetrachtungen des Versuchs gezeichnet. 

__Materialien:__ Sie erhalten einen Kondensator mit der Kapazität $4600 \mu F$ und einen ohmschen Widerstand mit $1000 \Omega$.

---

<H4>Schaltung: </H4>

__Ladekreis:__

- die Pole der Spannungsquelle werden über den Wechselschalter direkt an den Kondensator angeschlossen

<p style="margin-left:5%">

$ \red{\boxed{\mathrm{ACHTUNG:\ + Platte\ des\ Kondensators\ mit\ \oplus der\ Spannungs-Quelle\ verbinden}}}$

<details>

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_1](https://diversewolken.ddns.net/nextcloud/index.php/s/SMpRaWdBfXBPDSW/download)<!-- style="max-width:80%; margin:5%"-->

</details>

</p>

---

Entladekreis:

- der Widerstand wird in Reihe zum Kondensator angeschlossen

- in Reihe zum Widerstand folgt das _Cassy_

- achten Sie beim Anschluss des _Cassy_, dass der blaue Anschluss in Richtung $\ominus$-Pol der Spannungsquelle und der schwarze Anschluss in Richtung des $\oplus$-Pols der Spannungsquelle zeigt

<details style="margin-left:5%">

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_2](https://diversewolken.ddns.net/nextcloud/index.php/s/m2KAErdZKRTMFi5/download)<!-- style="max-width:80%; margin:5%"-->

</details>

- lassen Sie sich die Schaltung von der Lehrkraft abnehmen

### 5.9.8. Aufnahme der Entladekurve

$ \red{\boxed{\mathrm{Die Schaltung\ muss\ abgenommen\ worden\ sein.}}}$

__Grundlage:__ Hier wird der Kondensator zunächst geladen. Dann wird die automatische Messung mit dem _Cassy_ gestartet und die Entladekurve wird aufgezeichnet.

- legen Sie den Wechselschalter in die Ladeposition

- schalten Sie die Spannungsquelle ein und wählen eine Spannung von 10 V

- starten Sie anschließend die Messung auf dem _Cassy_ indem Sie oben auf __"Messzeit nicht vorgegeben"__ klicken, legen Sie anschließend den Schalter um

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/dDiiE3cYDgGqM3W/download)<!-- style="max-width:80%; margin:5%"-->

- stoppen Sie die Messung nach etwa $T=4\tau$ (4 charaktieristischen Zeiteinheiten)

- <bdi style="color:red">_Hinweis:_ Die Entladung (und somit die Messzeit $T$) beginnt erst, wenn sie den Schalter auf Entladen umlegen.</bdi>


### 5.9.9. Auswertung der Messkurve $I(t)$

__Grundlage:__ Hier werden die Messdaten ausgewertet.

__Ermittlung der geflossenen Ladung:__

- wählen Sie unter Auswertungen (unterhalb des Diagramms) den Menupunkt _"Fläche zur x-Achse"_

- angezeigt wird die geflossene Ladung in der Einheit $A\cdot s = C$ 

- notieren Sie diesen experimentell ermittelten Messwert als geflossene Ladung $Q_{exp}$ und

- $ \red{\boxed{\mathrm{Erstellen\ Sie\ einen\ Screeshot\ von\ Ihrer\ Messung\ INKLUSIVE\ Auswertung.}}}$

![Cassy_-_Auswertung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/BXHx8eeCy8oXBSD/download)<!-- style="max-width:80%; margin:5%"-->

### 5.9.10. Übersicht: Vergleich aller Ergebnisse

@color(Notieren und ergänzen Sie diese Übersicht als Ergebnis im Hefter, blue)

<br>

Gegeben: $R = 1000 \Omega$, $C=4600 \mu F$

<p class="newspaper3">

__Experimentelle Auswertung:__

Mit Hilfe von Cassy wurde im Zeitintervall

$$ T = \boxed{..^{\,}}\,s $$

die geflossene Ladung $Q_{exp}$ ermittelt.

<p class="cb">

__Aufladen des Kondesators:__

Der Kondensator wurde mit der Ladung 

$$ Q_{lad} = \dfrac{\boxed{..^{\,}}}{\boxed{..^{\,}}} $$

aufgeladen. 

<p class="cb">

__Numerische Emittlung (Integral):__

Aus der Entladekurve

$$Q_{int} = \int_{0}^{T} I_0 \cdot e^{-\frac{1}{R\cdot C}t}\,\,\mathrm{d}t$$

ergibt sich mittels Integral auf dem CAS geflossene Ladung $Q_{int}$ zu

</p>

</p>

</p>


<p class="newspaper3">

$$ Q_{exp} = \boxed{..^{\,}}\,C $$

<p class="cb">

$$ Q_{lad} = \boxed{..^{\,}}\,C $$

<p class="cb">

$$Q_{int} = \boxed{..^{\,}} \, C $$

</p>

</p>

</p>

<br>

@color(Diskutieren Sie diese Werte und die relativen d.h. prozentualen Abweichungen voneinander., blue)