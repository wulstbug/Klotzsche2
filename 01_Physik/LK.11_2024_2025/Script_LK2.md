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

# Physik LK 2024/2025 - Teil 2

@uhr

__E-Lehre, Magnetismus, Elektro-Magnetismus__

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

<details style="margin-left:10%">

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

@rangeQuiz2($q_{\alpha}$, 0, $C$)

@rangeQuiz2($m_{\alpha}$, 0, $kg$)

</p>

---

1.2. Zeichnen Sie das elektrische Feld eines einzelnen Alpha-Teilchens. Sie können das Alpha-Teilchen als Kugel betrachten, die Elementarteilchen müssen nicht extra gezeichnet werden.

<details style="margin-left:10%">

<summary> Lösung </summary>

</details>

---

1.3. Notieren Sie die Art des elektrischen Feldes. Begründen Sie Ihre Aussage anhand 4.2.

<p style="margin-left:10%">

Feldform: [[ Radialfeld ]]

Feldart: [[ homogen ]]

</p>

---

2. __Elektronenröhre__ <br> Elektronenröhren sind sehr nützliche elektronische Bauelemente, welche entscheidend für die Entwicklung der ersten Computer Waren. Eine Elektronenröhre ähnelt einem einem kleinen Plattenkondensator, welcher sich Inneren einer evakuierten Glaskugel befindet. Abb.1 zeigt eine stark vereinfachte seitliche Skizze. Dabei ist der negative Pol der Spannungsquelle an die Kathode angeschlossen und der positive Teil an die Anode. ![Elektronenröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/27yGykN3XxZ27gJ/download "Abb.1: Schema Elektronenröhre") 

2.1. Zeichnen Sie die elektrischen Feldlinien in die Skizze ein.

2.2. Erläutern Sie qualitativ, was mit einem Elektron geschieht, welches zwischen Kathode und Anode befindet.

2.3. Ermitteln Sie den Wert der elektrischen Feldstärke zwischen Kathode und Anode. 

2.4. Im Betrieb wird die Kathode geheizt und Elektronen treten mit ca. 2∙10⁶ m/s aus der Kathode aus. Ermitteln Sie die Geschwindigkeit, welche ein Elektron an der Anode besitzt.

2.5. Im Betrieb wird die Kathode geheizt und Elektronen treten mit ca. 2∙10⁶ m/s aus der Kathode aus. Ermitteln Sie die Geschwindigkeit, welche ein Elektron an der Anode besitzt.


## 1.4. Die Kapazität

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
> _Für die einfachste Bauform eines Kondensators [siehe 1.3](#13-der-kondensator) kann man die Kapazität wie folgt berechnen:_
> 
> __Kapazität eines @color(Plattenkondensators, orange):__
>
> $$ \boxed{ C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} } $$
>
> <p style="text-align:center">[IQB-Formelsammlung](https://www.iqb.hu-berlin.de/abitur/abitur/dokumente/naturwissenschaften/N_Mathematischna.pdf) (S.28+54)</p>
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

<p class="newspaper">

geg.:

<div style="text-indent:10%">

$A$ = <bdi style="color:orange"> $28\,cm \cdot 28\,cm = 0,28 \cdot 0,28\,m^2 = 0,0784 m^2$</bdi>

$d$  <bdi style="color:orange"> $\approx 1,5\,cm = 0,015 m$ </bdi>

$\varepsilon_r$ = <bdi style="color:orange"> $ = 1$ </bdi>

</div>

<p class="cb">

ges.:

<div style="text-indent:10%">

$C$

</div>

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

3. __Wolkenkondensator__ ![Wolkenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/F3xsbZknJ3PPqme/download) Eine positiv geladene Wolke in 400 m Höhe bildet zusammen mit dem Erdboden einen Plattenkondensator (Fläche einer „Platte“ 8,0 km²). Läd sich die elektrisch Wolke auf, so entsteht zwischen Wolke und Erdboden ein elektrisches Feld. Die elektrische Feldstärke ist in dieser Aufgabe 1,2∙105 V/m, was so hoch ist, dass eine Entladung durch die Luft (Blitz) unmittelbar bevorsteht.

3.1. Zeigen Sie, dass die Spannung zwischen der Wolke und dem Boden etwa 50 Millionen Volt beträgt.

3.2. Zeigen Sie, dass sich auf der Wolke eine Ladung von 8,5 C befindet.

3.3. Ermittle die Ladung, die ein kugelförmiges Wassertröpfchen mit 2,0 mm Durchmesser haben müsste, wenn es vor Entladung der Wolke zwischen dieser und der Erde bei Windstille gerade schweben würde? <br> (Der Auftrieb in Luft ist zu vernachlässigen.)

3.3. Ermitteln Sie die Ladung Q, welche sich in den Wolken befindet.

3.4. Wie lange würde die Entladung der Wolke dauern, wenn die mittlere Stromstärke des Blitzes 4,0 kA betragen würde?

3.5. Noch bevor es zu einer Entladung kommt, drückt ein Fallwind die Wolke auf eine niedrigere Höhe herab. Die Ladung der Wolke bleibe dabei konstant. <br> Wie ändert sich qualitativ die elektrische Feldstärke zwischen Wolke und Erde? Wird eine Entladung der Wolke dadurch wahrscheinlicher? <br> Geben Sie eine kurze Begründung.