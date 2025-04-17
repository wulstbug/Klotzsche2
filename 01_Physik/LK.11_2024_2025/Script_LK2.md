<!--
author: Christian Golnik

language: de

import: https://raw.githubusercontent.com/LiaScript/CodeRunner/master/README.md

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
        [[?]] Achte auf die Richtung der Feldlinien im Aufgabentext. Vergleiche die Richtung mit der Richtungsvorgabe für Feldlinien (siehe 5.2)
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

<summary> Lösungsweg Newton'sche Gesetze / Kinematik </summary>

![Lsg_2.4](https://diversewolken.ddns.net/nextcloud/index.php/s/Xas4Gr5sMZYsLGP/download)

</details>

<details>

<summary> Lösungsweg Energieansatz </summary>

![Lsg_2.4](https://diversewolken.ddns.net/nextcloud/index.php/s/pXJdL873F8pX9bj/download)

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
     [[?]] Nutze die allgemeine Formel für die Kapazität ([1.4](#1.4.-die-kapazität)) und die spezielle Formel für die Kapazität des Plattenkondensators.
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

$$ \boxed{I = \dfrac{\mathrm{d}Q}{\mathrm{d}t}} $$
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

$$ T=18,4 s$$

Die Funktion $I(t)$ für die Entladekurve am Kondensator lautet

$$ I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t} $$ 

mit den Werten $R=1000\Omega$, $C=4600\cdot10^{-6}F$ und $I_0=\frac{U}{R}$. Das gesamte Integral für die Ladung $Q_{int}$ lautet:

$$ Q_{int} = \int_0^{T} \frac{U}{R} \cdot e^{-\frac{1}{R\cdot C}\cdot t} \mathrm{d}t $$ 

Bzw. mit Zahlenwerten für den CAS:

$$ Q_{int} = \int_0^{18,4} \frac{10}{1000} \cdot e^{-\frac{1}{1000 \cdot 0,0046}\cdot t} \,\,\mathrm{d}t $$

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


### 5.9.9. Auswertung der Messkurve

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

Gegeben: $R = 1000 \Omega$, $C=4600 \mu F$, $U=10V$

<br>

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

## Selbstständiges Arbeiten: Berechnungen am Kondensator

### Berechnungen am Kondensator

Die kreisförmigen Platten eines Kondensators besitzen einen Radius von **8,5 cm** und haben einen Abstand von **3,0 mm**. Der Raum zwischen den Platten ist mit einem der in Tabelle 1 genannten Dielektrika vollständig ausgefüllt.

__Tabelle 1: Dielektrika und Permittivität__


<!-- data-type="none" -->
| Dielektrikum | Gummi | Glas | Polystyrol |
|-------------|------|------|------------|
| relative Permittivität ($\varepsilon_r$) | 3,5  | 10  | 2,5 |

In einer Messreihe wird der Kondensator mit verschiedenen Spannungen _U_ aufgeladen. Für jede Spannung wird die auf dem Kondensator befindliche Ladung _Q_ gemessen. Tabelle 2 zeigt die zugehörigen Messwerte:


**Tabelle 2: Messwerte der Ladung _Q_ in Abhängigkeit der Spannung _U_**

<!-- data-type="none" -->
| _U_ in kV  | 0,5  | 1,0  | 2,0  | 3,0  | 4,0  |
|------------|------|------|------|------|------|
| _Q_ in nC | 83,0 | 168  | 325  | 510  | 655  |

__Aufgaben__

1. **Darstellung der Messwerte**
    - Stelle die Ladung _Q_ in Abhängigkeit von der Spannung _U_ in einem geeigneten Schaubild dar und begründe den Kurvenverlauf.

2. **Kapazitätsberechnung**
    - Ermittle unter Verwendung aller Messwerte die Kapazität des mit dem Dielektrikum gefüllten Kondensators.

3. **Bestimmung des Dielektrikums**
    - Bestimme das verwendete Dielektrikum.

4. **Veränderte Messung mit Glas**
    - In einem neuen Versuch ist der Kondensator vollständig mit Glas gefüllt. Der Abstand der Kondensatorplatten beträgt nun **6,0 mm**. Die oben stehende Messung wird mit den gleichen Spannungswerten wiederholt.
    - Ermittle, wie sich die Ladungen auf den Platten gegenüber Tabelle 2 verändern.

5. **Erklärung der Dielektrikum-Wirkung**
    - Erläutere, weshalb ein Dielektrikum die Kapazität eines Kondensators erhöht.

### Berechnungen am Kondensator (mit Loesungen)

Die kreisförmigen Platten eines Kondensators besitzen einen Radius von **8,5 cm** und haben einen Abstand von **3,0 mm**. Der Raum zwischen den Platten ist mit einem der in Tabelle 1 genannten Dielektrika vollständig ausgefüllt.

__Tabelle 1: Dielektrika und Permittivität__


<!-- data-type="none" -->
| Dielektrikum | Gummi | Glas | Polystyrol |
|-------------|------|------|------------|
| relative Permittivität ($\varepsilon_r$) | 3,5  | 10  | 2,5 |

In einer Messreihe wird der Kondensator mit verschiedenen Spannungen _U_ aufgeladen. Für jede Spannung wird die auf dem Kondensator befindliche Ladung _Q_ gemessen. Tabelle 2 zeigt die zugehörigen Messwerte:


**Tabelle 2: Messwerte der Ladung _Q_ in Abhängigkeit der Spannung _U_**

<!-- data-type="none" -->
| _U_ in kV  | 0,5  | 1,0  | 2,0  | 3,0  | 4,0  |
|------------|------|------|------|------|------|
| _Q_ in nC | 83,0 | 168  | 325  | 510  | 655  |

__Aufgaben__

1. **Darstellung der Messwerte**
    - Stelle die Ladung _Q_ in Abhängigkeit von der Spannung _U_ in einem geeigneten Schaubild dar und begründe den Kurvenverlauf.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Abi21_Loesung1](https://diversewolken.ddns.net/nextcloud/index.php/s/qnpT9nHgETS2E4o/download)

</details>

---

2. **Kapazitätsberechnung**
    - Ermittle unter Verwendung aller Messwerte die Kapazität des mit dem Dielektrikum gefüllten Kondensators.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Abi21_Loesung2](https://diversewolken.ddns.net/nextcloud/index.php/s/iTHMxL3ADM7oJCf/download)

</details>

---


3. **Bestimmung des Dielektrikums**
    - Bestimme das verwendete Dielektrikum.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Abi21_Loesung3](https://diversewolken.ddns.net/nextcloud/index.php/s/zfyWnpnadqBNwHD/download)

</details>

---


4. **Veränderte Messung mit Glas**
    - In einem neuen Versuch ist der Kondensator vollständig mit Glas gefüllt. Der Abstand der Kondensatorplatten beträgt nun **6,0 mm**. Die oben stehende Messung wird mit den gleichen Spannungswerten wiederholt.
    - Ermittle, wie sich die Ladungen auf den Platten gegenüber Tabelle 2 verändern.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Abi21_Loesung4](https://diversewolken.ddns.net/nextcloud/index.php/s/6ndABxptiNCyQdY/download)

</details>

---


5. **Erklärung der Dielektrikum-Wirkung**
    - Erläutere, weshalb ein Dielektrikum die Kapazität eines Kondensators erhöht.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Abi21_Loesung5](https://diversewolken.ddns.net/nextcloud/index.php/s/DiL85geCyAEjg5x/download)

</details>

---

### Experimentieren am Kondensator

Ermitteln Sie unter Nutzung des angegebenen Schaltplans experimentell die Kapazität des Kondensators.
Die Einstellungen am Stromversorgungsgerät dürfen nicht verändert werden. Die anliegende Spannung U wird Ihnen nicht mitgeteilt und darf nicht gemessen werden. Erfragen Sie beim Aufsicht führenden Lehrer den Widerstand des Ohm’schen Bau-
elements.

- Verbinden Sie Ihr Tablet mit dem Cassy-Messgerät (_Hilfe_-> [5.9.5 CassyVerbinden](#5.9.5.-anleitung-zur-verbindung-von-cassy-und-tablet)) @color(_Hinweis: Das Cassy-Messgerät ist bereits eingestellt. Parameter müssen nicht mehr geändert werden._, blue)

- ![Schaltplan_Exp](https://diversewolken.ddns.net/nextcloud/index.php/s/2QzYebzS4esXzrK/download) Laden Sie den Kondensator zunächst auf. Der Kondensator soll nun entladen und dabei die I(t)-Entladekurve aufgezeichnet werden.

1. Nehmen Sie eine Entladekurve I(t) des Kondensators auf.

2. Ermitteln Sie mit Hilfe des Cassy-Messgerätes die abgeflossene Ladung $Q_{exp}$ und notieren Sie diese (_Hilfe_ -> [5.9.9. Auswertung der Messwertkurve](#5.9.9.-auswertung-der-messkurve)).

3. Machen Sie von Ihrer Messung einen Screenshot. <br> @color(_Hinweis: Der experimentelle Teil ist beendet. Gehen Sie zu Ihrem Platz zurück._, blue)

4. Ermitteln Sie aus Ihren Messdaten die Ladespannung $U$ und die Kapazität des Kondesators $C$.

5. Ermittlen Sie aus Ihren Messwerten eine Entladezeit $T$, welche sinnvollerweise nicht unterschritten werden sollte, damit ein Großteil der Ladung vom Kondensator abgeflossen ist.

6. Ermitteln Sie die zum Zeitpunkt t=0 im Kondensator gespeicherte elektrische Energie an.

7. Die Kondensatorspannung wird für elektronische Schaltvorgänge genutzt. Ein Schaltvorgang wird ausgelöst, wenn der Kondensator entladen wird und die Kondensatorspannung den Wert $\frac{U}{2}$ unterschreitet. Ermitteln Sie rechnerisch diese Zeitdauer für die im Experiment untersuchten Kondensator-Widerstands-Kombination.


### Experimentieren am Kondensator (mit Lösung)

Ermitteln Sie unter Nutzung des angegebenen Schaltplans experimentell die Kapazität des Kondensators.
Die Einstellungen am Stromversorgungsgerät dürfen nicht verändert werden. Die anliegende Spannung U wird Ihnen nicht mitgeteilt und darf nicht gemessen werden. Erfragen Sie beim Aufsicht führenden Lehrer den Widerstand des Ohm’schen Bau-
elements.

- Verbinden Sie Ihr Tablet mit dem Cassy-Messgerät (_Hilfe_-> [5.9.5 CassyVerbinden](#5.9.5.-anleitung-zur-verbindung-von-cassy-und-tablet)) @color(_Hinweis: Das Cassy-Messgerät ist bereits eingestellt. Parameter müssen nicht mehr geändert werden._, blue)

- ![Schaltplan_Exp](https://diversewolken.ddns.net/nextcloud/index.php/s/2QzYebzS4esXzrK/download) Laden Sie den Kondensator zunächst auf. Der Kondensator soll nun entladen und dabei die I(t)-Entladekurve aufgezeichnet werden.

1. Nehmen Sie eine vollständige Entladekurve des Kondensators auf.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Exp_Loesung1](https://diversewolken.ddns.net/nextcloud/index.php/s/MSzKXixiaKNBnW2/download)

</details>

---

2. Ermitteln Sie mit Hilfe des Cassy-Messgerätes die abgeflossene Ladung $Q_{exp}$ und notieren Sie diese (_Hilfe_ -> [5.9.9. Auswertung der Messwertkurve](#5.9.9.-auswertung-der-messkurve)).

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Exp_Loesung2](https://diversewolken.ddns.net/nextcloud/index.php/s/5zJjPAZWHR4KpQb/download)

</details>

---

3. Machen Sie von Ihrer Messung einen Screenshot. <br> @color(_Hinweis: Der experimentelle Teil ist beendet. Gehen Sie zu Ihrem Platz zurück._, blue)

---

4. Ermitteln Sie aus Ihren Messdaten die Ladespannung $U$ und die Kapazität des Kondesators $C$.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Exp_Loesung4](https://diversewolken.ddns.net/nextcloud/index.php/s/2RNc35nfFdw24Mi/download)

</details>

---

5. Ermittlen Sie aus Ihren Messwerten eine Entladezeit $T$, welche sinnvollerweise nicht unterschritten werden sollte, damit ein Großteil der Ladung vom Kondensator abgeflossen ist.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Exp_Loesung5](https://diversewolken.ddns.net/nextcloud/index.php/s/NofXcH6GfgcZ5fX/download)

</details>

---

6. Ermitteln Sie die zum Zeitpunkt t=0 im Kondensator gespeicherte elektrische Energie an.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

$ E = \frac{1}{2}\cdot C \cdot U^2 \approx 0,14 J $

</details>

---

7. Die Kondensatorspannung wird für elektronische Schaltvorgänge genutzt. Ein Schaltvorgang wird ausgelöst, wenn der Kondensator entladen wird und die Kondensatorspannung den Wert $\frac{U}{2}$ unterschreitet. Ermitteln Sie rechnerisch diese Zeitdauer für die im Experiment untersuchten Kondensator-Widerstands-Kombination.

<details style="margin-left:10%;margin-right:10%">

<summary> Loesung </summary>

![Exp_Loesung7](https://diversewolken.ddns.net/nextcloud/index.php/s/xxe4r8EZD5HwQE3/download)

</details>

---


## 5.11 Potentielle Energie eines geladenen Teilchens im elektr. Feld

![TB_Herleitung_E_pot_el](https://diversewolken.ddns.net/nextcloud/index.php/s/TTfNQpdec65NNZC/download)

<details>

<summary> Lösungsweg zu 5.3 / Aufgabe 2 (Elektronenröhre) - Energieansatz </summary>

![Lsg_2.4E](https://diversewolken.ddns.net/nextcloud/index.php/s/pXJdL873F8pX9bj/download)

</details>

## 5.12 Das elektrische Potential und die elektrische Spannung

<p style="color:blue">

- nutze Duden S. 267/268 (oder Metzler S. 198)

- erarbeite dir (allein oder in Partnerarbeit) den Begriff __elektrisches Potential__

- übernimm dazu die Merkkästen in deine Aufzeichnungen

- zeichne in deinen Hefter Äquipotentiallinien an in einem Plattenkondensator und bei einem Radialfeld

- übernimm den Merksatz zum Begriff __elektrische Spannung__ (Duden S. 268)

</p>


## 5.13 Dielektrikum - Ein Medium (Material) im Plattenkondensator

{{1}}
********
> ![Dielektrikum1](https://diversewolken.ddns.net/nextcloud/index.php/s/LjstxnWtmJbaGJY/download)<!-- style="width:300px" --> Ein __Dielektrikum__ ist ein @color(nichtleitendes Material, orange), welches zwischen die Platten eines Plattenkondensators eingebracht wird. Dabei verändert sich die Kapazität des Kondensators. <br> Das Verhältnis aus Kapazität mit - ($C$) und Kapazität ohne ($C_0$) Dielektrikum nennt man Dielektrizitätszahl $\varepsilon_r$. <br> $$ \varepsilon_r = \dfrac{C}{C_0}$$
********

{{2}}
********
> ![ElementareDipole](https://diversewolken.ddns.net/nextcloud/index.php/s/XfwLBXEkJSMJPTL/download) Legt man an den Kondensator nun eine Spannung an, so richten sich die @color(elementaren Dipole, orange) innerhalb des Dielektrikums im elektrischen Feld des Kondensators aus (__Polarisierung__).
********

{{3}}
********
> ![Dielektrikum2](https://diversewolken.ddns.net/nextcloud/index.php/s/KwkZD7myWYGePT4/download)<!-- style="width:300px" -->  Innerhalb des Dielektrikums entsteht ein @color(inneres elektrisches Feld, darkgreen), welches dem @color(äußeren elektrischen Feld, blue) des Kondensators entgegen gerichtet ist und es schwächt.
********

{{4}}
********
> Die Kapazität eines __Plattenkondensators__ mit Dielektrikum, das den Plattenzwischenraum vollständig ausfüllt, beträgt
>
> $$ C = \varepsilon_r \varepsilon_0 \dfrac{A}{d}$$
********

### Aufgaben zu 5.12.

@color(Löse Metzler S. 221 / A1-4, blue)

---

Lösung 1.

<p style="margin-left:10%">

@rangeQuiz2($C$, 8e-12 , $F$)

</p>

---

Lösung 2.

<p style="margin-left:10%">

@rangeQuiz2(Quarzglas:, 3.75 , .)

@rangeQuiz2(Wasser:, 81 , .)

@rangeQuiz2(Glycerin:, 43 , .)

</p>

---

Lösung 3.

<details style="margin-left:10%">

<summary> Lösungsweg 3.a </summary>

![MetzlerS221_3](https://diversewolken.ddns.net/nextcloud/index.php/s/erNfkkbssMPTstf/download)

</details>

<details style="margin-left:10%">

<summary> Lösungsweg 3.b </summary>

![MetzlerS221_3](https://diversewolken.ddns.net/nextcloud/index.php/s/NnySNYYcrmz236c/download)

</details>

---

Lösung 4.

<details style="margin-left:10%">

<summary> Lösungsweg 4. </summary>

![MetzlerS221_4](https://diversewolken.ddns.net/nextcloud/index.php/s/6ycm4BFAzFiPeGt/download)

</details>

## 5.14 Fachpraktische Übung Fahrradlicht

![FahrradLicht](https://diversewolken.ddns.net/nextcloud/index.php/s/WjpAnRMmgnWJXpN/download) Zur Sicherheitsausrüstung jedes Fahrrads gehört ein Rücklicht, das seine Energie entweder von einem Dynamo oder von einer Batterie bzw. Akkumulator bekommt. Heutige Fahrradrücklichter enthalten oft anstelle einer Batterie
einen Kondensator. Wenn der Dynamo aufhört, elektrische
Energie zu liefern, leuchtet ein solches Rücklicht noch einige Zeit weiter.

__Schaltung__

![FahrradLichtSchaltung](https://diversewolken.ddns.net/nextcloud/index.php/s/rd4XonE8LgTLLJW/download)Der folgende Aufbau soll modelhaft eine solche Rücklichtschaltung untersuchen. <br> Dabei wird anstelle des Dynamos eine Spannungsquelle verwendet, welche mit Hilfe des Schalters von der Versorgung getrennt werden kann.

<p style="color:blue">

Machen Sie sich zunächst mit der Schaltung vertraut. Diskutieren Sie in Ihrer Gruppe, warum die LED bei geschlossenem Schalter leuchtet und warum Sie bei geöffnetem Schalter noch eine Weile weiter leuchtet.

</p>

### Aufgaben I

<p style="color:blue">

1. a) Beschreiben Sie die Vorgängen beim Anschließen eines Plattenkondensators an eine Spannungsquelle, zunächst ohne Dielektrikum Kondensator.

</p>

<details style="margin-left:10%">

<summary> Lösung 1.a) </summary>

- legt man an einen Plattenkkondensator eine Spannung an, so fließen elektrische Ladungen auf die Platten des Kondesators.

- da sich gleichnahmige Ladungen abstoßen, ist die Ladestromstärke zunächst hoch und sinkt dann exponentiell ab

</details>

---

<p style="color:blue">

1. b) Erläutern Sie, wie sich das Einfügen eines Dielektrikums zwischen den Platten auswirkt.

</p>

<details style="margin-left:10%">

<summary> Lösung 1.b) </summary>

- bei Verwendung eines Dielektrikums ruft das entstehende elektrische Feld eine Ladungsverschiebung im Dielektrikum hervor (Polarisation)

- es entsteht ein inneres elektrisches Feld, welches dem äußerden elektrischen Feld entgegen gerichtet ist und dieses schwächt. 

- durch die Verringerung der elektrischen Feldstärke im Inneren des Kondensators erhöht sich die auf den Platten speicherbare Ladung (bei gleicher Ladespannung) und somit erhöht sich auch die Kapazität.

</details>

---

<p style="color:blue">

1. c) Die Leuchtdiode (LED) im Rücklicht soll nach Ende der Fahrt noch für mindestens 1 Minute leuchten. Nehmen Sie __vereinfachend__ an, dass die LED vom Kondensator über 1 Minute mit einer konstanten Spannung von U = 2,5 V versorgt wird und dabei ein Strom der Stärke I = 0,2 mA fließt. <br> Berechnen Sie die elektrische Ladung, die durch die LED fließen muss und ermitteln Sie die mininmale Kapazität des Kondensators.

<p style="margin-left:10%">

@rangeQuiz2($Q$, 0.012 ,$C$)

@rangeQuiz2($C$, 4.8e-3 ,$F$)

</p>

</p>

<details style="margin-left:10%">

<summary> Lösung 1.c) </summary>

Bei einer @color(konstanten, red) Stromstärke von 0,2 mA während einer Zeit von 1 Minute, kann die Ladung ermittelt werden mit

$$ Q = I \cdot t = 0,2 \cdot 10^{-3} A \cdot 60 s = 0,012 C  $$

Die zugehörige Kapazität wäre dann

$$ C = \dfrac{Q}{U} = 4,8 \cdot 10^{-3} F $$

</details>

---

<p style="color:blue">

1. d) Begründen Sie, dass der vereinfachte Ansatz von Aufgabe c) auf einen realen Schaltkreis mit Kondensator nur sehr begrenzt angewendet werden kann. D.h. diskutieren Sie inwiefern die Annahme nicht der Realität entspricht.

</p>

<details style="margin-left:10%">

<summary> Lösung 1.d) </summary>

Beim Entladen eines Kondensators ist die Entladespannung zeitlich nicht konstant. Die Spannung sinkt mit zunehmend abgeflossener Ladung. Somit sinkt auch die Stromstärke beim Entladen des Kondensators.

</details>

### Experimenteller Teil

<p style="color:blue">

Sie erhalten von der Lehrkraft eine LED (rot), einen Kondensator, ein Cassy-Messgerät und einige ohmsche Widerstände. 

Erfragen Sie von der Lehrkraft die Ladespannung $U$.

Bauen Sie den Schaltkreis (5.14) auf. Wählen Sie zunächst einen der ohmschen Widerstände. 

@color(Lassen Sie sich den Schaltkreis abnehmen., red)

Schalten Sie probehalber die Spannungsversorgung bei geschlossenem Schalter ein. Öffnen Sie den Schalter und beobachten Sie das Leucht-Verhalten der LED.

---

__Abhängigkeit vom ohmschen Widerstand__

1. Beobachten Sie für verschiedene ohmsche Widerstände die Zeitdauer, wie lange die LED nachleuchtet, zunächst qualitativ. Formulieren Sie eine Aussage zum Einfluss des ohmschen Widerstands auf das Leuchtverhalten.

2. Die Leuchtdauer der LED soll nun in Abhängigkeit des ohmschen Widerstands quantitativ untersucht werden. Überlegen Sie zunächst, mit welcher physikalisch messbaren Größe, man die Leuchtdauer (d.h. das Erlöschen) der LED definieren könnte. Formulieren Sie Ihre Vermutung. <br> @color(_Hinweis: "Hinschauen wann Sie ausgeht" ist keine quantitative Messung._, orange)

3. Bauen Sie den Schaltkreis so um, dass eine quantitative Messung der Leuchtdauer ermöglich wird.

4. Nehmen Sie mit Ihrem Messaufbau für alle bereitgestellten ohmschen Widerstände die Leuchtdauer auf.

5. Zeichnen Sie ein Diagramm in welchem Sie die Leuchtdauer in Abhängigkeit des ohmschen Widerstands auftragen.

6. Interpretieren Sie das Diagramm und begründen Sie den Kurvenverlauf physikalisch.

</p>

### Aufgaben II

Ein Kondensator besteht aus zwei dünnen Metallfolien mit einer isolierenden Schicht (mit der Dielektrizitätszahl $\varepsilo_r_ = 9,6$ und der Dicke d = 0,70 μm) als Dielektrikum.

1. Berechnen Sie den benötigten Flächeninhalt pro Kondensatorplatte, um die Kapazität von $C=4,8\cdot10^{-3} F$ in einem Plattenkondensator mit diesem Dielektrikum zu erhalten.

<p style="margin-left:10%">

@rangeQuiz2($A$, 39.5 ,$m^2$)

</p>

2. Diskutieren Sie, welches Material als Dielektrikum sich eher eignen würde, damit sich für die Platten des Kondensators ein praktisch umsetzbarer Wert ergibt. Berechnen Sie eine mögliche Kondensatorfläche.

### Auswertung des Experiments

__Kriterium LED__

```text Kriterium

```
@LIA.eval()

<!-- 
    data-xlabel="R in Ω" 
    data-ylabel="t in s" 
    data-title="Leuchtdauer LED"
-->
| R in Ω| t in s |
| ---- | ---- | ---- |
| 100 | 0 |
| 220 | 0 |
| 470 | 0 |
| 1000 | 0 |
| 2200 | 0 |
| 10000 | 0 |

__Probleme für Realität:__

```text Probleme



```
@LIA.eval()

# LB6 - Magnetisches Feld

![MagnetischesFeld](https://www.mozaweb.com/de/mozaik3D/FOL/termeszet/foldi_magneses_mezo/960.jpg)

{{1}}
***********
> __Das magnetische Feld__ ist, ebenso wie das elektrische Feld, @color(ein Modell, red) um den Einfluss von @color(magnetischen Kräften im Raum um einen Magneten, blue) darzustellen.
***********


## 6.1 Vergleich von elektrischen und magnetischen Feldern

<p class="newspaper3">

__Name__

<p class="cb">

__Elektrisches Feld__


<p class="cb">

__Magnetisches Feld__

</p>

</p>

</p>

---

<p class="newspaper3">

_Ursache sind_

<p class="cb">

{1}{__elektrische Ladungen Q__}

<p class="cb">

{2}{__@color(Dauermagnete,red)__ und __@color(bewegte,red) elektrische Ladungen (elektrischer Strom)__}

</p>

</p>

</p>

---

<p class="newspaper3">

_Darstellung durch_

<p class="cb">
{{3}}
********
Elektrische Feldlinien

![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)
********
<p class="cb">
{{4}}
********
Magnetische Feldlinien

![WikimediaMagnetischesFeld](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0c/VFPt_cylindrical_magnet_thumb.svg/1280px-VFPt_cylindrical_magnet_thumb.svg.png)
********
</p>

</p>

</p>

---

<p class="newspaper3">

_Verdeutlicht wird die_

<p class="cb">

{5}{__Wirkung der elektrischen Kraft__ auf eine <span style="color:orange">positive Probeladung</span>.}

<p class="cb">

{6}{__Wirkung der magnetischen Kraft__ auf einen @color(anderen Magneten,orange) oder auf @color(eine bewegte Ladung, orange).}

</p>

</p>

</p>

---

<p class="newspaper3">

_Eigenschaften sind_

<p class="cb">
{{7}}
********
- Feldlinien verlaufen von @color($\oplus$, red) nach @color($\ominus$, blue)

<br>

- elektrischen Kräfte wirken __entlang (d.h. tangetial)__ der Feldlinien

- je dichter die Feldlinien, desto größer die Kraft
********

<p class="cb">

{{8}}
********
- Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, blue)

- magnetische Kräfte mit Hilfe der Feldlinien ableitbar (siehe __Lorentzkraft__)

- je dichter die Feldlinien, desto größer die Kraft

- Feldlinien sind @color(__immer__,red) geschlossen (kein Anfang oder Ende)

- sie verlaufen außerhalb des Magneten von @color(__N__,red)->@color(__S__, blue) und innerhalb von @color(__S__, blue)->@color(__N__,red)
********

</p>

</p>

</p>

---

{{9}}
********

@color(Selbstständiges Arbeiten, blue)

<p style="margin-left:5%">

<br>

@color(__Aufgabe:1.1__ Ergänze diese Übersicht zu magnetischen Feldern durch eine eigene Recherche. Zeichne dazu einige Arten von Magneten und die zugehörigen Felder in deinen Hefter., blue)

<br>

@color(__Aufgabe 1.2.__ Ergänze diese Übersicht mit zwei Beispielen für homogene magnetische Felder. Wiederhole die Definition von __homogen__., blue)

<br>

@color(__Aufgabe 1.3.__ Ergänze diese Übersicht mit Erklärungen zur anziehenden und abstoßenden Kraftwirkung zwischen Magneten., blue)

<br>

<bdi style="color:blue">__Aufgabe 1.4.__ Notiere Stichpunkte zum Erdmagnetfeld. Gehe dabei auf die Lage der magnetischen Pole, das Feldlinienbild und die Funktion als Schutzschild für die Erde ein.</bdi>

<br><br>

@color(Nutze hierfür z.B. folgende Quellen:, blue)

<br>

- [Arten von Magneten](https://www.abi-physik.de/buch/das-magnetfeld/dauer--und-elektromagnete/)

- [Homogene Felder](https://www.abi-physik.de/buch/das-magnetfeld/homogenes-magnetfeld/)

- LB Duden S. 277-279

</p>

---

********


{{10}}
********
!?[XeniusMagnetismusUnsichtbareKraft](https://www.youtube.com/watch?v=mlt9JcRpzYg)
********

{{11}}
********
<p class="newspaper3">

_Arten von Feldern_

<p class="cb">

homogenes Feld (im Plattenkondensator)

![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)


<p class="cb">

homogenes Feld (im Inneren eines Hufeisenmagneten)

![HomogenesFeld](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-spule.png)

homogenes Feld (im Inneren einer Spule)

![HomogenesFeldHufeisenmagnet](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-1.png)

</p>

</p>

</p>

---
********

### Aufgaben zur Überprüfung

1. Das Magnetfeld der Erde gleich dem eines/r .. <br>
_Hinweis: Die folgenden Formen der magnetischen Felder solltest du im Hefter haben._

<!-- data-solution-button="off" -->
[( )] Hufeisenmagneten
[(x)] Stabmagneten
[( )] Stromdurchflossenen Leites
[( )] Stromdurchflossenen Spule

---

2. Das hier gezeigte Magnetfeld gehört zu einem/r

![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)

<!-- data-solution-button="off" -->
[(x)] Hufeisenmagneten
[( )] Stabmagneten
[( )] Stromdurchflossenen Leiters
[( )] Stromdurchflossenen Spule

---

3. Welche der folgenden Aussagen über das Erdmagnetfeld ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Der magnetische Nordpol der Erde befindet sich nahe dem geografischen Südpol.
[[ ]] Das Erdmagnetfeld schützt die Erde vor kosmischer Strahlung.
[[x]] Die Stärke des Erdmagnetfelds ist überall auf der Erde gleich.
[[ ]] Die Polarität des Erdmagnetfelds kann sich im Laufe der Zeit umkehren.

---

4. Erkunden Sie, ob auch andere Planeten ein Magnetfeld besitzen.

---

5. Markieren Sie das Magnetfeld eines stromdurchflossenen Leiters.

<!-- data-solution-button="off" -->
[( )] ![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)
[( )] ![Stabmagnet](https://www.abi-physik.de/images/devpages/stabmagnet.png)
[(x)] ![Leiter](https://www.abi-physik.de/images/devpages/leiter.png)
[( )] ![Spule](https://www.abi-physik.de/images/devpages/spule.png)

---

6. Dauermagnete (Permanentmagnete) sind Stoffe, die ihre Umgebung dauerhaft magnetisch beeinflussen. Sie bestehen aus.. (_Vgl. LB S. 102_)

<!-- data-solution-button="off" -->
[[ ]] Magnesium
[[x]] Eisen
[[ ]] Aluminium
[[ ]] Zink
[[ ]] Kupfer
[[ ]] Zinn
[[x]] Cobalt
[[x]] Nickel

---

7. Der magnetische Nordpol der Erde befindet sich in der Nähe des

<!-- data-solution-button="off" -->
[( )] geographischen Nordpols
[(x)] geographischen Südpols
[( )] Nullmeridians
[( )] Äquators

---

8. Durch welche Anordnung könnten die abgebildeten Magnetfelder erzeugt worden sein.

![GK_Duden_S124_A20](https://diversewolken.ddns.net/nextcloud/index.php/s/gDybkgMkALZHmoq/download)

a)

<!-- data-solution-button="off" -->
[[ ]] Hufeisenmagneten
[[x]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

b)

<!-- data-solution-button="off" -->
[[x]] Hufeisenmagneten
[[ ]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

---

9. Welcher der folgenden Prozesse erzeugt kein Magnetfeld?

<!-- data-solution-button="off" -->
[[ ]] Ein elektrisch geladenes Teilchen bewegt sich mit konstanter Geschwindigkeit.
[[ ]] Ein stromdurchflossener Leiter.
[[x]] Ein statischer elektrischer Dipol.
[[ ]] Eine Spule mit wechselndem Strom.

---

10. Welche Aussage über Magnetfeldlinien ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Magnetfeldlinien sind geschlossene Kurven und haben keinen Anfang und kein Ende.
[[ ]] Magnetfeldlinien verlaufen außerhalb eines Magneten vom Nordpol zum Südpol.
[[x]] Magnetfeldlinien können sich in einem homogenen Magnetfeld überschneiden.
[[ ]] Die Dichte der Magnetfeldlinien gibt die Stärke des Magnetfeldes an.

11. Welche der folgenden Aussagen ist korrekt?

<!-- data-solution-button="off" -->
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist entlang der Leiterachse ausgerichtet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist radial nach außen gerichtet.
[[x]] Das Magnetfeld um einen stromdurchflossenen Leiter ist kreisförmig und konzentrisch um den Leiter angeordnet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter existiert nur, wenn der Strom sinusförmig wechselt.


## Demonstrationsexperiment: Kräfte auf bewegte elektrische Ladungen in Magnetfeldern

![FotoLorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/mLFceeEL2jP7BDC/download)

## 6.2. Hand-Regel zur Richtungsbestimmung der Lorentzkraft

!?[HandRegel](https://www.youtube.com/watch?v=snM3g4zWeNw)

__Bemerkungen zur Lorentzkraft:__

??[Lorentzkraft_LearningApps](https://learningapps.org/4454537)

_Bitte schau dir zunächst dieses kleine Quiz zur Richtungsbestimmung der Lorentz-Kraft an._

      [QuizZurLorentzkraftRichtung](https://www.leifiphysik.de/elektrizitaetslehre/bewegte-ladungen-feldern/aufgabe/quiz-zu-bewegten-ladungen-im-magnetfeld)

      _Hinweis: Die magnetischen Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, green)._

## 6.3 Berechnung des magnetischen Feldes - Die magnetische Flussdichte B

<p class="newspaper">

__Elektrisches Feld__

<p class="cb">

__Magnetisches Feld__

</p>

</p>

---

<p class="newspaper">

{{1}}
********

Die elektrische Feldstärke $E$ berechnet sich aus der Kraft $F$ auf eine elektrische Ladung $Q$.

$$ \boxed{E = \frac{F_{el}}{Q}} $$

- $F$: Elektrische Kraft [Newton, $N$]
- $Q$: Ladung im Feld [Coulomb, $C$]

> Hinweis: Das elektrische Feld ist eine vektorielle Größe $\vec{E}$, ebenso wie die Kraft $\vec{F_{el}}$. Kraft und Feld wirken entlang einer Linie.

********

<p class="cb">

{{2}}
********

Die __magnetische Flussdichte__ $B$ beschreibt die Stärke und Richtung des magnetischen Feldes in einem Punkt. Sie wird definiert durch die Kraft auf eine bewegte Ladung oder einen stromdurchflossenen Leiter:

$$ \boxed{B = \frac{F}{I \cdot l}}$$

- $F$: Magnetische Kraft [Newton, $N$]
- $I$: Stromstärke [Ampere, $A$]
- $l$: Leiterlänge [Meter, $m$]

> Hinweis: Die magnetische Flussdichte ist eine vektorielle Größe ($\vec{B}$), ebenso wie die Lorentzkraft $\vec{F_L}$. Die Richtungen von $\vec{B}$ bzw. $\vec{F}$ ergeben sich aus der Handregel.

********

</p>

</p>

---

{{3}}
********
<p class="newspaper">

__Einheit__: $$\Big[\dfrac{N}{C}=\dfrac{V}{m}\Big]$$

<p class="cb">

__Einheit__: [1 Tesla = 1 T]

$$\Big[T=\dfrac{N}{A \cdot m}\Big]$$

</p>

</p>

---
********


### 6.3.2 Übung: Berechnung der magnetischen Flussdichte

#### Aufgabe 6.3.1
Ein gerader Leiter mit einer Länge von 2 m wird von einem Strom von 5 A durchflossen. Er befindet sich in einem Magnetfeld mit einer Flussdichte $B$. Die magnetische Kraft auf den Leiter beträgt 0,5 N. Berechne $B$!

@rangeQuiz2(B, 0.05, T)

#### Aufgabe 6.3.2
Ein stromdurchflossener Leiter (Länge $ℓ = 1,5 \, m$, Stromstärke $I = 3 \, A$) befindet sich in einem Magnetfeld mit $B = 0,2 \, T$. Berechne die magnetische Kraft $F$ auf den Leiter.

@rangeQuiz2(F, 0.9, N)

#### Aufgabe 6.3.3
Ein Leiter der Länge $ℓ = 3 \, m$ und Stromstärke $I = 2 \, A$ erfährt eine magnetische Kraft von $F = 0,6 \, N$. Berechne die magnetische Flussdichte $B$.

@rangeQuiz2(B, 0.1, T)

#### Aufgabe 6.3.4 

__Analyse von Änderungen__

Ein stromdurchflossener Leiter befindet sich in einem Magnetfeld. Die Stromstärke $I$ wird verdoppelt, während die Leiterlänge $ℓ$ und die magnetische Flussdichte $B$ unverändert bleiben. Wie ändert sich die magnetische Kraft $F$?

<!-- data-solution-button="off" -->
[[ ]] Sie bleibt gleich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie halbiert sich.  
[[ ]] Sie vervierfacht sich. 

---

<!-- data-solution-button="off" -->
Die magnetische Flussdichte $B$ wird auf das Doppelte erhöht, während Stromstärke $I$ und Leiterlänge $ℓ$ konstant bleiben. Was passiert mit der magnetischen Kraft $F$?

[[ ]] Sie bleibt gleich.  
[[ ]] Sie halbiert sich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie vervierfacht sich.  

## 6.4. Berechnungen der magnetischen Flussdichte B in einer langen Spule

<p class="newspaper">

__Magnetisches Feld__

![FeldInSpule](https://diversewolken.ddns.net/nextcloud/index.php/s/z7CNJzqkxjf4bf7/download)

<p class="cb">

__Elektrisches Feld__

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

</p>

</p>

---



{{1}}
********

<p class="newspaper">

Die magnetische Flussdichte $B$ innerhalb einer __langen, stromdurchflossenen Spule__ wird durch folgende Formel beschrieben:

$$
\boxed{B = \mu_0 \cdot \mu_r \cdot \frac{N\cdot I}{ℓ}}
$$

- $B$: Magnetische Flussdichte [ Tesla, $T$]
- $\mu_0$: Magnetische Feldkonstante $\boxed{\mu_0 = 1,26 \cdot 10^{-6} \frac{V \cdot s}{A \cdot m}}$
- $\mu_r$: Magnetische Permeabilität des Mediums [einheitenlos -> FS S.54]
- $N$: Anzahl der Windungen der Spule
- $ℓ$: Länge der Spule [Meter, $m$]
- $I$: Stromstärke [Ampere, $A$]

<p class="cb">

{{2}}
********

Die elektrische Feldstärke E innerhalb eines Plattenkondensators wird durch folgende Formel beschrieben:

$$ \boxed{E = \dfrac{U}{d}} $$

- $U$: Spannung zwischen den Platten $\big[ V \big]$ 
- $d$: Abstand der Platten $\big[ m \big]$ 

********

</p>

</p>

********

### Aufgaben zur B-Feld Berechnung an Spulen

<bdi style="color:blue">__Löse die folgenden Aufgaben, indem du die gegebene Formel zur _langen Spule_ anwendest__.</bdi>

---

__Aufgabe 6.4.1 __ 

Eine Spule hat $N = 800$ Windungen und eine Länge von $ℓ = 0,4 \, m$. Sie wird von einem Strom mit $I = 3 \, A$ durchflossen. Die Spule ist luftgefüllt ($\mu_r = 1$). Berechne die magnetische Flussdichte $B$ im Inneren der Spule.  

@rangeQuiz2(B, 0.00754, T)

---

__Aufgabe 6.4.2__

Eine Spule mit $N = 500$ Windungen und $ℓ = 0,5 \, m$ erzeugt eine magnetische Flussdichte von $B = 2,51 \, mT$. Berechne die Stromstärke $I$, die durch die Spule fließt.  

@rangeQuiz2(I, 2, A)

__Aufgabe 6.4.3__  

Eine Spule hat $N = 1000$ Windungen und eine Länge von $ℓ = 1 \, m$. Der Strom beträgt $I = 4 \, A$. Wie verändert sich die magnetische Flussdichte $B$, wenn: 

1. Die Anzahl der Windungen $N$ verdoppelt wird?  
2. Der Strom $I$ halbiert wird?  
3. Die Länge der Spule $ℓ$ verdreifacht wird?

<!-- data-solution-button="off" -->
[[x]] 1. Verdoppelt sich, 2. halbiert sich, 3. verringert sich auf ein Drittel.  
[[ ]] 1. Verdoppelt sich, 2. bleibt gleich, 3. verringert sich auf die Hälfte.  
[[ ]] 1. Bleibt gleich, 2. halbiert sich, 3. verringert sich auf ein Viertel.  
[[ ]] 1. Verringert sich, 2. bleibt gleich, 3. bleibt gleich.

__Aufgabe 6.4.4__

Eine luftgefüllte Spule hat $N = 1000$ Windungen, $ℓ = 0,8 \, m$ und $I = 2 \, A$. Im Innenraum der Spule wird ein Material mit einer unbekannten relativen Permeabilität $\mu_r$ ersetzt, wodurch die magnetische Flussdichte $B$ auf $1,7 \, T$ ansteigt. Berechne $\mu_r$.  

@rangeQuiz2($\mu_r$, 539.7, -)

Um welchen ferromagnetischen Stoff könnte es sich handeln?

<!-- data-solution-button="off" -->
[[Eisen]]

__Aufgabe 6.4.5__

Die magnetische Flussdichte $B$ in einer luftgefüllten Spule beträgt $1,26 \, mT$. Die Spule hat $N = 400$ Windungen und eine Länge von $ℓ = 0,5 \, m$. Berechne den Strom $I$, der durch die Spule fließt?  

@rangeQuiz2(I, 1.25, A)


### Übungen zum magnetischen Feld allgemein

__Grundwissen Magnetismus__

??[LueckentextMagnetismus](https://learningapps.org/1319776)

__Grundwissen magnetisches Feld__

??[LueckentextMagnetfeld](https://learningapps.org/35523603)

__Fragen zu magnetischen Experimenten__

??[MagnetischeExperimente](https://www.leifiphysik.de/elektrizitaetslehre/permanentmagnetismus/aufgabe/quiz-zu-magnetischen-eigenschaften)


#### Hinweise zur LK

![DreiFingerRegel](https://diversewolken.ddns.net/nextcloud/index.php/s/mnjjesXkkPMEGc8/download)

---

Übungen zur [Elektronenröhre](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#16) und [Wolkenkondensator](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#19).

---

Übungen zur [Berechnung an Kondensatoren](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#42) und zum Kondensator in realen Schaltkreisen [1](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#50) und [2](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#52)


## 6.5 Materie im magnetischen und elektrischen Feld

<p class="newspaper">

__Magnetisches Feld__

<p class="cb">

__Elektrisches Feld__

</p>

</p>

{{1}}
*******
---

Wird ein __Stoff (d.h. Materie)__ in ein magnetisches oder elektrisches Feld eingefügt, so verändert der Stoff die Stärke des Feldes, beschrieben durch 

<p class="newspaper">

die @color(magnetische Permeabilität $\mu_r$, orange) (-> FS. S 54).

<p class="cb">

die @color(Dielektrizitätszahl $\varepsilon_r$, orange) (-> FS. S 54).

</p>

</p>

---
*******

{{2}}
*******
__Beispiele:__

<p class="newspaper">

Cobalt: $\mu_r \approx 80-200$

Eisen: $\mu_r \approx 250-680$

Nickel: $\mu_r \approx 280-2500$

<p class="cb">

Glas: $\varepsilon_r \approx 5-16$

Bariumtitanat: $\varepsilon_r \approx 100-1000$

Wasser: $\varepsilon_r \approx 81$

</p>

</p>
*******
---

{{3}}
*******
__In beiden Beispielen__ richten sich elementare Strukturen des Material im umliegenden Feld aus.

<p class="newspaper">

@color(Elementar,red)@color(magnete,green) richten sich aus (__Magnetisierung__)

![ElementarMagnete](https://diversewolken.ddns.net/nextcloud/index.php/s/7H9rDQfp9fsAixS/download)

<p class="cb">

@color(Elementare,red) @color(Dipole, green) richten sich aus (__Polarisierung__)

![ElementareDipole](https://diversewolken.ddns.net/nextcloud/index.php/s/XfwLBXEkJSMJPTL/download)

</p>

</p>
*******
---

{{4}}
*******
__Unterschied:__

Während ferromagnetische Stoffe (Eisen, Cobalt, Nickel) das magnetische Feld __verstärken__, wird das elektrische Feld durch ein Dielektrikum (z.B. Glas, Wasser) __geschwächt/gedämpft__.
*******

### Aufgaben zum magnetischen Feld

1. Eine Spule ist 9cm lang, hat 1500 Windungen und wird von einem Strom der Stärke 1,52 A durchflossen. Im Innern der Spule wird die magnetische Flussdichte 2,54 T gemessen.<br> Weise rechnerisch nach, dass sich im Innern der Spule nicht ausschließlich Luft befindet.

<details style="margin-left:10%">

<summary> Hilfe: Hinweis Zur Lösung</summary>

Ermitteln Sie die magnetische Flussdichte im Inneren der Spule unter der Annahme, dass diese mit Luft gefüllt ist. Vergleichen Sie Ihr Ergebnis mit der Angabe aus der Aufgabe und schlussfolgern Sie auf das vorhandene $\mu_r$.

</details>

<details style="margin-left:10%">

<summary> Rechenweg </summary>

![Abi21_Lsg2.1_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/4dsX4QKj4FgWz6q/download)

</details>

<details style="margin-left:10%">

<summary> Begründung </summary>

![Abi21_Lsg2.1_Begründung](https://diversewolken.ddns.net/nextcloud/index.php/s/som5GarSYN8yHPR/download)

</details>

<details style="margin-left:10%">

<summary> Alternativer Lösungsweg </summary>

Stelle die Formel für $B$ nach $\mu_r$ um, nutze für für B=2,54T und zeige, dass $\mu_r > 1$ gilt.

Hier ist: $\mu_r \approx 85$ 

</details>


---

2. Eine andere Spule hat 50 Windungen, ist 20 cm lang und ist ausschließlich mit Luft gefüllt. Die Flussdichte im Inneren der Spule beträgt 0,63 mT. Gib die Stromstärke an. <br> Die Spule wird nun auf 40 cm gedehnt, dabei ändert sich die Flussdichte im Inneren der Spule, Stromstärke und Windungszahl bleiben konstant.<br> Zeiche den Graphen $B = B(ℓ)$ für das Intervall 20cm bis 40cm.

@rangeQuiz2($\hspace{1cm}$ $I$, 2, $A$)

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zur Stromstärke</summary>

Nutzen Sie die Formel zur Berechnung der magnetischen Flussdichte und ermitteln Sie den fehlenden Wert der elektrischen Stromstärke.

</details>

<details style="margin-left:10%">

<summary> Rechenweg Stromstärke </summary>

![Abi21_Lsg2.2_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/Xd5nS692Wwd97cD/download)

</details>

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zum Graph</summary>

Nutze Sie die Formel für die magnetische Flussdichte, ermittlen Sie die Funktion $B(ℓ)$, setzen Sie die gegebenen Werten ein und erstellen Sie eine Datentabelle | $ℓ$ | $B(ℓ)$ | für den Bereich 20cm bis 40 cm.

</details>

<details style="margin-left:10%">

<summary> Berechnungen für den Graph $B(ℓ)$ </summary>

![Abi21_Lsg2.2_Berechnung_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/mddY9WFHAT59ofx/download)

</details>

<details style="margin-left:10%">

<summary> Datentabelle und Graph $B(ℓ)$ </summary>

<p class="newspaper">

<!-- data-type="none" -->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |

<p class="cb">

<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="ℓ in m"
     data-ylabel="B in mT"
-->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |


</p>

</p>

</details>

---

3. Es wird eine lange Spule der Länge $l = 21cm$ betrachtet. Fließt durch die Spule eine Stromstärke von 2A so erhällt man eine magnetische Flussdicht von $30\,mT$. Fügt man in die Spule einen ferromagnetischen Kern, so erhöht sich die magnetische Flussdichte auf den Wert $2,4\,T$.

3. 1. Nennen Sie ein Material aus welchem der ferromagnetische Kern bestehen könnte. Begründen Sie Ihre Aussage. 

     <!-- data-solution-button="off" -->
     [[ Cobalt ]]

<details style="margin-left:10%">

<summary> Begründung </summary>

Ohne Ferromagnetikum ist die magnetische Flussdichte $0,03 T$ und mit Ferromagnetikum erhöht sich die Flussdichte um das 80-fache auf $2,4 T$. Der Wert für $\mu_r$ muss demzufolge 80 betragen und dafür kommt aus der FS S. 54 nur Cobalt in Frage.

</details>

3. 2. Ermitteln Sie die Anzahl der Windungen der Spule.

     <!-- data-solution-button="off" -->
     [[ 2500 ]]

<details style="margin-left:10%">

<summary> Lösung </summary>

Formel für magnetische Flussdichte im Inneren einer Spule nutzen und nach $N$ auflösen.

</details>

3. 3. __Partnerarbeit__ Geben Sie zwei Möglichkeiten an, mit der man die magnetische Flussdichte der Spule(inklusive Kern) verdoppeln kann.

<details style="margin-left:10%">

<summary> Möglichkeiten </summary>

- Stromstärke verdoppeln
- Windungszahl verdoppeln
- Länge der Spule halbieren
- Ferromagnetikum mit $\mu_r=2$ gibt es laut Tabelle nicht

</details>

3. 4. __Partnerarbeit__ Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht.

<details style="margin-left:10%">

<summary> Lösungen </summary>

Ein ferromagnetischer Stoff hat mikroskopische magnetische Elemente, genannt @color(Elementarmagnete, red). Diese sind im Normalzustand des Ferromagnetikums @color(ungeordnet, red). Unter dem Einluss eines @color(äußeren Feldes, red) ordnen sich Elementarmagnete mit Ihren Polen entlang der Feldlinien des äußeren Feldes, man nennt das @color(Magnetisierung, red). <br>
Die geordneten Elementarmagnete verstärken mit ihren ausgerichteten Elementarmagneten das äußere Feld

</details>

### KI-Aufgabe zu ferromagnetischen Stoffen

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Prompt Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Ferromagnetikum-Aufgabe:__<br> Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht.
<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Gib mir keine Hinweise und nicht die Lösung, sondern warte auf meine Aussagen. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist. Ich habe folgende Aufgabe bekommen: Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht. Bitte warte auf meine Antwort und bewerte diese.</span>
</div>

<script input="submit" style="margin-left:10%"  default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)


# LB 7 - Geladene Teilchen in statischen elektrischen und magnetischen Feldern

{{1}}
**********
> Die Bewegung elektrisch geladener Teilchen beschreiben wir mit den Methoden der __Kinematik__ [@color(__LB 3__, red)] auf Basis der wirkenden Kräfte (__elektrische Kraft__ $F_{el}$ [@color(__LB 5__,red)] und __Lorentzkraft__ $F_L$ [@color(__LB 6__,red)]). Dabei betrachten wir die Teilchen als __Punktmassen__, welche den __Newton'schen Gesetzen__ [@color(__LB 2__, red)] folgen. __Energie__betrachtungen, z.B. zur kinetischen Energie, [@color(__LB 1__, red)] sind gültig. 
**********

![ProtonCollisionCern](https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg)

## 7.1. Geladene Teilchen im elektrischen Feld

<p class="newspaper">

__Bewegung im Längsfeld__

> Elektrische Kraft auf Teilchen (hier @color(Elektronen, darkgreen) ) wirkt __entlang der Bewegungsrichtung__

<p class="cb">

__Bewegung im Querfeld__

> Elektrische Kraft auf Teilchen (hier @color(Elektronen, darkgreen) ) wirkt __senkrecht zur Bewegungsrichtung__

</p>

</p>

---

<p class="newspaper">

__Elektronenkanone__

![Elektronenkanone](https://diversewolken.ddns.net/nextcloud/index.php/s/cC5JWAYmimFKmrC/download)

<p class="cb">

__Ablenkröhre__

![Ablenkröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/HaNg8rpJnyZj7F5/download)

</p>

</p>

### 7.1.1. Beschleunigung im Längsfeld - Elektronenkanone

@timer(35,00)

__Aufbau einer Elektronenkanone__

??[VirtuelleExperiment_Elektronenkanone_Aufbau](https://virtuelle-experimente.de/kanone/klassisch/aufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de CC BY-NC-SA 3.0 DE")

<p style="color:blue">

__Aufgaben:__

1. Wähle im linken Menü _Simulation_

1. 1. Verändere die Heizspannung $U_{Heiz}$ und beobachte den Effekt auf das Experiment.

1. 2. Verändere die Beschleunigungsspannung $U_b$ und beobachte den Effekt auf das Experiment.

2. Klicke auf _weiter_ oder im linken Menü auf _Beschleunigung_.

2. 1. Die Elektronenkanone ist in eine @color(Beschleunigungszone, green) und eine @color(Flugzone, pink) aufgeteilt.

2. 2. Zeichne unter der Überschrift (siehe oben) eine Skizze der Elektronenkanone in deinen Hefter. 

2. 3. Schau dir die Herleitung der Beschleunigungsarbeit ($W_{el}$) bzw. der Geschwindigkeit der Elektronen nach der Beschleunigung an. Übernimm grundlegende Elemente der Herleitung für $v_{end}$ und die finale Formel in deinen Hefter.

2. 3. Klicke nun auf _weiter_ oder _Flugphase_. Lies dir die Anweiungen durch. Es genügt, wenn du im Hefter folgende Bemerkung unter die Herleitung notierst.

<p style="color:black">
> Wenn die Elektronen die Anode verlassen haben, bewegen Sie sich in Flugrichtung (x-Richtung) geradlinig-gleichförmig mit der Geschwindigkeit $v_{end}.$
</p>

3. Klicke nun im oberen Menü auf den Punkt _Übungen_.

3. 1. Löse _Übung Aufbau_ (Menü links)

3. 2. Löse den Lückentext.

3. 3. (_Optional_) Löse das Quiz.

3. 4. Bearbeite die Rechenaufgaben. 

      __Aufgabe 1:__ Als __Partnerübung__, d.h. eine Person stellt die Frage und liest die Lösung, die andere Person beantwortet die Frage.

      __Aufgabe 2:__ Als __Einzelarbeit__ mit Lösungsüberprüfung und Diskussion des Lösungswegs in der Gruppe.

</p>



#### KI-Aufgabe: Beschleunigung elektrischer Ladungen im Längsfeld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem Elektronen beschleunigt werden können. <br> 2. Nenne und begründe die Art der Bewegung der Elektronen. <br> 3. Gib an, wie die Intensität des Elektronenstrahls (d.h. die Anzahl an Elektronen pro Sekunde) beeinflusst werden kann. <br> 4. Gib an, wie die Endgeschwindigkeit der Elektronen beeinflusst werden kann.

<p style="margin-left:10%">

<summary> __Prompt__ </summary>

<span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem Elektronen beschleunigt werden können. <br> 2. Nenne und begründe die Art der Bewegung der Elektronen. <br> 3. Gib an, wie die Intensität des Elektronenstrahls (d.h. die Anzahl an Elektronen pro Sekunde) beeinflusst werden kann. <br> 4. Gib an, wie die Endgeschwindigkeit der Elektronen beeinflusst werden kann. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Grundkurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
    
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)


alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)

### 7.1.2. Ablenkung Querfeld - Ablenkröhre

@timer(35, 00)

__Aufbau einer Elektronen-Ablenkröhre__

??[VirtuelleExperiment_ElektronenAblenkrhre](https://virtuelle-experimente.de/e-feld/hypothesen/versuchsaufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de CC BY-NC-SA 3.0 DE")

<p style="color:blue">

__Aufgaben:__

1. Klicke auf Zusammenfassung (linkes Menü)

1. 1. Übernimm folgenden Merksatz in deinen Hefter

<p style="color:black">
> Bewegen sich Elektronen senkrecht zu den Feldlinien durch das homogene elektrische Feld eines Plattenkondensators, werden sie aufgrund der elektrischen Kraft abgelenkt.
</p>

1. 2. Übernimm eine Skizze des Aufbaus in deinen Hefter

1. 3. Übernimm die beiden Erkenntnisse in deinen Hefter

<p style="color:black">

> Je größer die Plattenspannung $U_P$ am Kondensator desto stärker ist die Ablenkung der Elektronen
>
> Je kleiner die Beschleunigungsspannung der Elektronen (und somit deren Geschwindigkeit), desto stärker ist die Ablenkung
>
> Die Bahnform der Elektronen ist eine __Parabel__ mit der Gleichung
>
> $$\boxed{y(x) = \dfrac{U_p}{4 \cdot d \cdot U_b} \cdot x^2}$$
>
> Die parabelförmige Bewegung ist eine __Superposition__ (Überlagerung) aus einer gleichförmigen Bewegung (in x-Richtung) und einer gleichmäßig beschleunigten Bewegung in (y-Richtung). Es gelten die __Bewegungsgleichungen__:

<p class="newspaper">

> $x(t) = v_{0x} \cdot t$ 
>
> $v_x(t) = v_{0x} $
>
> $a_x(t) = 0 $

<p class="cb">

> $y(t) = \frac{1}{2} \cdot a_y \cdot t^2$
>
> $v_y(t) =  a_y \cdot t$
> 
> $a_y(t) \overset{\mathrm{2.NG}}{=} \frac{F_{el}}{m} = \frac{E_{el}\cdot q}{m} = \frac{U_p \cdot q}{d \cdot m} $

</p>

</p>

</p>

2. Wechsle zu den _Übungen_ (oberes Menü) und bearbeite:

2. 1. Übung Fachbegriffe

2. 2. _Optional:_ Übung Anschluss

2. 3. Mulitple Choice kurze Version

2. 4. Abituraufgaben

      - Aufgabe 2

      - Aufgabe 5 (a, b, d)

</p>

#### KI-Aufgabe: Beschleunigung elektrischer Ladungen im Querfeld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten die Bewegung eines geladenen Teilchens im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen (Querfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem eine solche Ablenkung erfolgen kann. <br> 2. Beschreibe die Art der Bewegung der elektrischen Ladungen. Gehe auf den Begriff Superposition ein. <br> 3. Gib qualitativ an, welcher Bahnform die geladenen Teilchen folgen. <br> 4. Gib an, wie die Stärke der Ablenkung der geladenen Teilchen beeinflusst werden kann.

<p style="margin-left:10%">

>__Prompt__
>
><span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen:<br> Erkläre mit eigenen Worten die Bewegung eines geladenen Teilchens im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen (Querfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem eine solche Ablenkung erfolgen kann. <br> 2. Beschreibe die Art der Bewegung der elektrischen Ladungen. Gehe auf den Begriff Superposition ein. <br> 3. Gib qualitativ an, welcher Bahnform die geladenen Teilchen folgen. <br> 4. Gib an, wie die Stärke der Ablenkung der geladenen Teilchen beeinflusst werden kann. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Grundkurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>

</p>
    
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>


---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)


alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)

## Entwicklung Leistungen 11Ph2

{{0-2}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend |
| ---- | ---- | ---- |
| LK1 | 7.9 | 7.88 |
| KA1 | 6.3 | 8.2 |
| EX1 | 11.9| 8.52 |
| KA2 | 7.7 | 8.84 |
| LK2 | 8.8 | 9.16 |
*********

{{2}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend |
| ---- | ---- | ---- |
| LK1 | 7.9 | 7.88 |
| KA1 | 6.3 | 8.2 |
| EX1 | 11.9| 8.52 |
| KA2 | 7.7 | 8.84 |
| LK2 | 8.8 | 9.16 |
| KA3 |   | 9.5 |
*********

{{1}}
*******
> Trend: $$\boxed{f(n) = 0.32\cdot n + 7.56}$$
*******

## Aktuelle Informationen

> Aufgrung der aktuellen politischen Lage, haben Deutschland und einige Nachbarländer beschlossen, @color(internationale Klassenfahrten nicht mehr zu genehmigen, red).

- Kursfahrt wurde vom _Landesamt für Schule und Bildung_ storniert

- Schweiz fällt daher aus

{{1}}
*******
> Ich habe in __Chemnitz__ Ersatz gefunden

<p class="newspaper3">

__Schullandheim im Chemnitzer Küchenwald__

![Chemnitzer Schullandheim](https://www.kjf-online.de/files/kjf/arbeitsbereiche/erholung-bildung/schullandheim-chemnitz/Impressionen/IMG_5706.JPG)

![Chemnitzer Schullandheim2](https://www.kjf-online.de/assets/images/c/SLH1-8270065b.jpg)

<p class="cb">

__Karl Marx Monument__

![Nischel](https://travelnating.com/wp-content/uploads/2023/01/Karl-Marx-Monument-in-Chemnitz.jpg)

__Neues Rathaus (mit Stadtratsbesuch)__

![Neue Rathaus](https://travelnating.com/wp-content/uploads/2023/01/Neues-Rathaus-Chemnitz.jpg)

<p class="cb">

__Industriemuseum Chemnitz__

![IndustrieMuseum](https://travelnating.com/wp-content/uploads/2023/01/Industriemuseum-Chemnitz.jpg)

__Küchenwald Parkeisenbahn__

![Parkeisenbahn](https://img.dampfbahn-route.de/rubrik_xl/1920x1080/bahn_37_2.jpg)

</p>

</p>

</p>
*******

{{2}}
*******
> Vorteil: Es wird nicht so teuer
*******

## 7.1.3. Der Millikan-Versuch

_Tafelbildvideo zum Millikan-Versuch:_

!?[Millikan-Experiment](https://www.youtube.com/watch?v=XMfYHag7Liw)

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Millikan](https://diversewolken.ddns.net/nextcloud/index.php/s/ocNCHdfqgfNNt44/download)

</details>

---

__Erklärung:__

Robert Millikan führte einen berühmten Versuch durch, um die Elementarladung $q_e$ zu bestimmen. Dabei wurden geladene Öltröpfchen in einem homogenen elektrischen Feld zwischen zwei Platten zum Schweben gebracht, indem sich die elektrische Kraft und die Gewichtskraft gegenseitig kompensieren. 


[IQB-Aufgabe-Milikan-Versuch](https://www.iqb.hu-berlin.de/appsrc/taskpool/data/taskpools/getTaskFile?id=p03%5Emillikan%5Ef4498)

### IQB-Aufgabe Milikan-Versuch

1. __Aufgabenstellung:__  [Milikan-Aufgabenstellung](https://diversewolken.ddns.net/nextcloud/index.php/s/EzY4gat6pjTXD7b/download)

2. __Hilfestellung:__ [Milikan-Hilfestellung](https://diversewolken.ddns.net/nextcloud/index.php/s/cizYee289ftPDQi/download)

3. __Zusätzliches Material:__ [Milikan-Material](https://diversewolken.ddns.net/nextcloud/index.php/s/dAa869L72S2dLzo/download)

#### KI-Aufgabe: Erkläre den Milikan-Versuch


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten den Milikan-Versuch <br> 1. Erkläre das Ziel, mit welchem der Versuch durchgeführt wurde. <br> 2. Erkläre den Versuchsaufbau <br> 3. Beschreibe, was bei den Messungen als Ergebnisse heraus gekommen sind. <br> 4. Erkläre, wie man die Ergebnisse interpretieren konnte.

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten den Milikan-Versuch <br> 1. Erkläre das Ziel, mit welchem der Versuch durchgeführt wurde. <br> 2. Erkläre den Versuchsaufbau <br> 3. Beschreibe, was bei den Messungen als Ergebnisse heraus gekommen sind. <br> 4. Erkläre, wie man die Ergebnisse interpretieren konnte. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungskurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
</div>
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)

## 3. Übungen zur Kombination aus statischen E- und B-Feld

@color(Löse aus den folgenden Aufgaben die __Grundlagen__ und wähle __eine__ der beiden Aufgaben I oder II., blue)

_Hinweis: Es gibt einige Aufgaben die als **Partnerübung** gekennzeichnet sich. Hier empfiehlt es sichin einer kleinen Gruppe zu arbeiten._ <br>

@color(-> Eine Person stellt die Frage und schaut sich die Lösung an. Die andere Person beantwortet die Frage und wird unterstützt., blue)

### Grundlagen

1. Notiere die Ladung des Elektrons, die Masse eines Protons, die Ladung und Masse eines Alpha-Teilchens

<p style="margin-left:10%">

<details>

<summary> Hinweis zur Lösung </summary>

Nutze die Formelsammlung unter der Rubrik: _Tabellierte Werte_

</details>

---

@rangeQuiz2($q_e$, -1.602e-19 , $C$)

@rangeQuiz2($m_p$, 1.67e-27, $kg$)

@rangeQuiz2($q_\alpha$, 3.204e-19 , $C$)

@rangeQuiz2($m_\alpha$, 6.64e-27, $kg$)

</p>

2. __Partnerübung__ 

2. 1. Definiere den Begriff homogenes Feld.

<details style="margin-left:10%">

<summary> Lösung </summary>

Ein homogenes Feld hat an jedem Ort (d.h. an jeder Stelle im Raum) den gleichen Wert (z.B. Feldstärke).

</details>

2. 2. Definiere den Begriff statisches Feld.

<details style="margin-left:10%">

<summary> Lösung </summary>

Ein statisches Feld ist zeitlich konstant, d.h. es verändert sich mit der Zeit nicht.

</details>


### Übungsaufgabe I

1. ![Geschwindigkeitsfilter](https://diversewolken.ddns.net/nextcloud/index.php/s/PfptPJcdpDkjDNX/download) (85) Elektronen treten aus einer Glühkathode K aus und werden durch ein Feld zwischen ihr und der Anode A (Spannung zwischen K und A beträgt U = 500,0 V) zu letzterer hin beschleunigt. Durch die Öffnung C in der Anode treten Elektronen in den Raum ein, in dem zwei Felder wirken:

- ein elektrisches Feld mit der elektrischen Feldstärke E = konst. > 0, dessen Feldlinien parallel zur Zeichenebene verlaufen (in der Skizze weggelassen), und 

- ein magnetisches Feld mit der magnetischen Flussdichte B = 0,012 T, dessen Feldlinien senkrecht aus der Zeichenebene heraus verlaufen (in der Skizze punktförmig dargestellt).

1. 1. Ermittle die Geschwindigkeit $v_1$ derjenigen Elektronen, die an der Oberfläche der Kathode keine kinetische Energie hatten, wenn Sie an der Öffnung C ankommen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($v_1$, 13.3e6 ,$\frac{m}{s}$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Hier kann man die kinetische Energie, die die Elektronen dazu gewinnen gleich der potentiellen Energie der Ladung im elektrischen Feld gleichsetzen.

<details style="margin-left:10%">

<summary> __Hinweis zu Formeln__ </summary>

Die kinetische Energie findet sich in der Formelsammlung. Die potentielle elektrische Energie wurde in Lernbereich II (elektrisches Feld) hergeleitet.

<details style="margin-left:10%">

<summary> _pot. elektr. Energie_ </summary>

$E_{pot.,el.} = E_{el} \cdot q \cdot d \overset{E_{el}=\frac{U}{d}}{=} U \cdot q$

</details>

</details>

</details>

<details>

<summary> __Lösung__ </summary>

![85_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/r9LweMS7dLMSWPk/download)

</details>

</p>

---

1. 2. Ermittle die Geschwindigkeit $v_2$ solcher Elektronen an der Öffnung C, welche die Katodenoberfläche in Richtung C mit der kinetischen Energie $E_{kin} = 3,2 \cdot 10^{-17} Ws$ verlassen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($v_2$, 15.7e6 ,$\frac{m}{s}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Ähnlich zu a) muss hier zur potentiellen elektrischen Energie der Ladung noch die kinetische Energie der Anfangsgeschwindigkeit addiert werden. Dann wieder Energien gleichsetzen und auflösen.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![85_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/SGpjarRsK859zkA/download)

</details>

</p> 

---

1. 3. __Partnerübung:__ Die Elektronen treten nach der Öffnung C in den Bereich elektrisches/magnetisches Feld ein. Begründen Sie, dass die Kräfte, die auf ein bewegtes Elektron unter dem Einfluss beider Felder wirken, unterschiedliche Richtungen haben.

<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Auf die Elektronen wirken sowohl die elektrische Kraft, als auch die magnetische Kraft (_Lorentzkraft_). Überprüfen Sie für beide Kräfte die Kraftrichtung.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

- die Kraft des elektrischen Feldes wirkt aufgrund der negativen Ladung des Elektrons und der Polung des Kondensators nach unten. 
- das magnetische Feld wirkt senkrecht zur Geschwindigkeit des Elektrons (_Lorentzkraft_), die Richtung wird mit der
linken-Hand-Regel bestimmt und zeigt nach oben.

</details>

</p>

---

1. 4. Stellen Sie eine Gleichung zur Berechnung des Betrages (des Wertes) der Gesamtkraft auf, wenn bekannt ist, dass sich die Einzelkräfte in der Richtung unterscheiden. (Die Gewichtskraft wird vernachlässigt).


<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Ermitteln Sie mit Hilfe der Formelsammlung die Formel für die elektrische Kraft innerhalb eines Plattenkondensators und Formel für die Lorentzkraft.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$F_{ges} = F_{el} - F_L $

$F_{ges} = E_{el} \cdot q - q \cdot v \cdot B $

</details>

</p>

---

1. 5. Berechnen Sie die notwendige elektrische Feldstärke, damit die Elektronen, die an der Oberfläche der Kathode keine kinetische Energie hatten, die Anordnung geradlinig durchfliegen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($E_{el}$, 159.1e3 ,$\frac{V}{m}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Überlegen Sie, unter welcher Bedingung die Elektronen keine Ablenkung erfahren (d.h. geradlinig weiter fliegen).

<details style="margin-left:10%">

<summary> __Hinweise zu Kräften__ </summary>

Keine Ablenkung erfolgt, wenn die Gesamtkraft (siehe 1.4.) gleich Null ist. Setzen Sie diese Gleichung gleich Null und ermitteln Sie daraus den Wert für $E_{el}$.

</details>

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$0 = F_{el} - F_L $

$ E_{el} \cdot q = q \cdot v \cdot B \Big| :q$

$ E_{el} = v \cdot B $

$ E_{el} = 13,3\cdot10^{6} \frac{m}{s} \cdot 0,012 T \hspace{0.5cm} \Big[ \frac{m\cdot V\cdot s}{s\cdot m^2} \Big]$

$ E_{el} = 159,1 \cdot 10^{3} \frac{V}{m} $

Alle Elektronen mit der oben berechneten Geschwindigkeit fliegen geradlinig durch die gekreuzten Felder hindurch. Alle anderen werden nach oben oder unten abgelenkt.

Damit wirkt eine solche Anordnung als Geschwindigkeitsfilter für geladene Teilchen und wird z.B. beim Massenspektrographen 
eingesetzt. Die Masse der Teilchen spielt dabei keine Rolle.

</details>

</p>

## 7.2. Geschwindigkeitsfilter für geladene Teilchen - E-B-Kombination

![TB_Geschwindigkeitsfilter](https://diversewolken.ddns.net/nextcloud/index.php/s/9LkfYcrrJTKZJFF/download)

### Übungsaufgabe Querfeldablenkung - E-B-Kombination

![Nr262_ElektronenbahnImElektrischenFeld.png](https://diversewolken.ddns.net/nextcloud/index.php/s/MMoMF6oKAeALQHs/download) Aus einer Elektronenquelle treten die Elektronen mit einer Geschwindigkeit $v_0$ senkrecht in das homogene elektrische Feld eines
Plattenkondensators der Breite 8,0 cm und der
Länge 10,0 cm ein. An den Plattenkondensator wird eine Spannung
von 12 kV angelegt.

2. 1. __Partnerübung*:__ Nennen Sie die Art der Flugbahn der Elektronen. Leiten Sie eine Gleichung für die Elektronenbahn im Feld her.

<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösungfindung__ </summary>

Auf die Elektronen wirkt die elektrische Kraft immer senkrecht zur den Kondensatorplatten, hier senkrecht nach oben. Das elektrische Feld ist homogen, demzufolge ist die elektrische Kraft konstant.

Dieser Effekt ist ähnlich dem horizontalen Wurf eines Körpers (nur nach oben statt nach unten). 

</details>

<details style="margin-left:10%">

<summary> __Hinweise zur Bahnform__ </summary>

In horizontaler Richtung (x-Richtung) wirkt keine Kraft auf das Elektron. Nach dem 1. Newton'schen Gesetz ist die Bewegung in x-Richtung daher __gleichförmig__.

In vertikaler Richtung (y-Richtung) wirkt auf das Elektron die konstante elektrische Kraft. Daher führt es in dieser Richtung nach dem zweiten Newton'schen Gesetz eine __gleichmäßig beschleunigte Bewegung__ aus.

</details>

<details style="margin-left:10%">

<summary> __Hinweise zu Bewegungsgleichungen__ </summary>

In horizontaler Richtung (x-Richtung): 

$x(t) = v_0 \cdot t$

In vertikaler Richtung (y-Richtung): 

$y(t) = \frac{1}{2} \cdot a \cdot t^2 $ wobei $a=\frac{F_{el}}{m}$

Ermitteln Sie nun die Wurfparabel $y(x)$. Stellen Sie dazu $x(t)$ nach der Größe $t$ um und setzen Sie diese in die Gleichung $y(t)$ ein.

</details>

<details style="margin-left:10%">

<summary> __Lösungsweg__ </summary>

Bewegungsgleichungen:

$x(t) = v_0 \cdot t$

$y(t) = \frac{1}{2} \cdot \frac{F_{el}}{m_e} \cdot t^2 $

Stelle $x(t)$ nach $t$ um: 

$t = \frac{x}{v_0}$

Setze $t$ in $y(t)$ ein, es ergibt sich die Wurfparabel y(x):

$ y(x) = \frac{1}{2} \cdot \frac{F_{el}}{m_e} \cdot \frac{x^2}{v_0^2}$

Die elektrische Kraft $F_{el}= \frac{U}{b} \cdot q_e$, wobei b der Plattenabstand des Kondensators ist. Setzt man das noch in y(x) ein, so ergibt sich

$ y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e} \cdot \frac{x^2}{v_0^2}$

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$ \boxed{y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot v_0^2} \cdot x^2}$

Dies ist die Gleichung für eine Parabel. Die Größen im Bruch sind alle gegeben, es gilt y~x2.

</details>

</p>

---

2. 2. Ermitteln Sie die Eintrittsgeschwindigkeit $v_0$, bei welcher die Elektronen genau den hinteren Rand der Platte erreichen. 


<p style="margin-left:10%">

@rangeQuiz2($v_0$, 5.74e7 , $\frac{m}{s}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösungfindung__ </summary>

Nutzen Sie die Lösung aus 2.1. Verwenden Sie die Bahnform. Legen Sie ein _geeignetes_ Koordinatensystem fest und überprüfen Sie, welche Korrdinaten die obere rechte Ecke des Kondensators hat.

</details>

<details style="margin-left:10%">

<summary> __Hinweise zum Koordinatensystem__ </summary>

Ein geeignetes Koordinatensystem wäre mit dem Ursprung am Eintrittsort des Elektrons in den Plattenkondensator (in der Abbildung der rote Punkt).

Die rechte obere Ecke des Kondensators wäre dann bei x=10cm und y=4cm.

</details>

<details style="margin-left:10%">

<summary> __Lösungsweg: Hinweise zur Nutzung der Gleichung y(x) __ </summary>

Die obere rechte Ecke des Kondensators besitzt die Koordinate (0,1 m | 0,04 m). Für die Bahngleichung (Wurfparabel) des Elektrons gilt:

$y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot v_0^2} \cdot x^2$

Mit $y=0,04m$ und $x=0,1m$. Stellt man die Gleichung nach $v_0$ um, so ergibt sich:

$v_0 = \sqrt{\frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot y}}\cdot x$

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

geg.: 

<p style="margin-left:10%">

$x=0,1m$

$y=0,04m$

$U=12\cdot10^3 V$

$|q_e|=1,602\cdot10^{-19}C$

$m_e=9,11\cdot10^{-31}kg$

$b=0,08 m$

</p>

ges.: $v_0$

Lsg.: _(Herleitung siehe Lösungsweg)_

$ v_0 = \sqrt{\frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot y}}\cdot x$

$v_0 = 5,74 \cdot 10^7 \frac{m}{s}$

</details>

</p>


---

2. 3. __Partnerübung:__ Beschreiben Sie die Bewegung der Elektronen, wenn die Geschwindigkeit $v_0$ größer als der in 2.2. ermittelte Wert ist.


<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Ist $v_0$ größer, fliegen sie über die Kondensatorplatten hinweg. Durch die größere Geschwindigkeit ist weniger Zeit, sie zu der Platte _hin zu lenken_. Stellt man die Bahnkurve nach x um, ist x~v2. Eine größere Geschwindigkeit bedeutet bei gleichem y, also Plattenabstand, ein größeres x.

</details>

---

Zwischen den Kondensatorplatten soll dem elektrischen Feld ein homogenes Magnetfeld so überlagert werden, dass die Elektronen der Geschwindigkeit $1,8\cdot 10^7 \frac{m}{s}$ die Anordnung unabgelenkt durchfliegen.

2. 4. __Partnerübung:__ Ermitteln Sie die Orientierung des Magnetfeldes. Begründen Sie Ihre Aussage.

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Überprüfen Sie die Richtung der elektrischen Kraft. Die Lorentzkraft muss der elektrischen Kraft entgegen gerichtet sein.

Überlegen Sie, welche Hand man für die Bestimmung der Lorentzkraft auf Elektronen nutzen muss.

Nutzen Sie die Drei-Finger-Regel um die Richtung des magnetischen Feldes zu bestimmen.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Die elektrische Kraft auf die Elektronen wirkt nach oben. Demzufolge muss die Lorentzkraft nach unten wirken. Nutzt man die Drei-Finger-Regel mit der linken Hand (Daumen=Elektronenbewegung; Zeigefinger=Magnetfeld; Mittelfinger=Kraftrichtung [nach unten]) so ergibt sich, dass das Magnetfeld in die Tafelebene hinein zeigen muss.

</details>

---

2. 5. __Partnerübung:__ Zeigen Sie, dass der Betrag der magnetischen Flussdichte 8,3 mT sein muss.

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Stellen Sie die Gleichung für die elektrische Kraft und die Lorentzkraft auf. Setzen Sie beide Kräfte gleich. Stellen Sie die Gleichung nach der magnetischen Flussdichte $B$ um.

</details>

<details style="margin-left:10%">

<summary> __Kräftegleichungen__ </summary>

Für die elektrische Kraft gilt:

<p style="margin-left:10%">

$F_{el} = E_{el} \cdot q_e$

Die elektrische Feldstärke $E_{el}$ in einem Plattenkondensator errechnet man mit 

$E_{el} = \frac{U}{d}$ mit d .. Plattenabstand.

Daher ist

$F_{el} = \frac{U}{d} \cdot q_e$

</p>

Für die Lorentzkraft $F_L$ gilt:

<p style="margin-left:10%">

$F_L = q_e \cdot v \cdot B$

</p>

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Setzt man die elektrische Kraft gleich der Lorentzkraft so ergibt sich

$F_{el} = F_L$

$ \frac{U}{d} \cdot q_e = q_e \cdot v \cdot B$

Diese Gleichung muss noch nach B umgestellt werden.

$\boxed{B= \frac{U}{v\cdot d}}$

Setzt man die gegebenen Wert $U=12\cdot10^3 V$, $v=1,8\cdot10^7\frac{m}{s}$ und $d=0,08m$ ein, so ergibt sich

$B = 0,0083 T$

</details>

---


2. 6. Erklären Sie, in welche Richtung Elektronen mit einer kleineren Geschwindigkeit unmittelbar nach dem Einschuss in den Feldbereich abgelenkt werden.

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Wenn die Elektronen langsamer fliegen, ändert sich die elektrische Kraft nicht. Die magnetische Kraft (_Lorentzkraft_) wird jedoch geringer, so dass die Elektronen nach oben abgelenkt werden.

</details>

---

Nun wird die Ablenkspannung ausgeschaltet, so dass nur noch das magnetische Feld vorhanden ist.

2. 7. *Ermitteln Sie die minimale Eintrittsgeschwindigkeit der Elektronen in das magnetische Feld, damit Sie den Feldbereich wieder verlassen, ohne auf eine Kondensatorplatte zu treffen.<br>_Hinweis: Hier müssen zur Vollständigkeit zwei Fälle betrachtet werden._

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![262_Lsg_f](https://diversewolken.ddns.net/nextcloud/index.php/s/qNeT5R6rQDm5DQ7/download)

</details>


## 7.3. Bewegung geladener Teilchen im homogenen Magnetfeld

![TB_HomogenesMagnetfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/jJYF7kSL4p6rQrb/download)

### Übungsaufgaben - Geladene Teilchen im homogenen Magnetfeld

1. Aufgabe 2 a+b+c aus: [Abituraufgabe-2-abc](https://virtuelle-experimente.de/b-feld/uebungen/aufgaben.php)

2. ![Kreisbahn](https://diversewolken.ddns.net/nextcloud/index.php/s/yZwLi4z7RWqTDkG/download) Geladene Teilchen bewegen sich im zeitlich konstanten homogenen Magnetfeld senkrecht zu den Feldlinien auf einer Kreisbahn. 

2. 1. Entscheiden Sie, ob es sich um ein positiv oder negativ geladenes Ion handelt. (1BE)

<p style="margin-left:10%">

[[negativ]]

</p>

2. 2. Übernehmen Sie diese Abbildung und tragen Sie am Punkt P der Bahn die Vektoren der Bahngeschwindigkeit und der wirkenden Lorentzkraft an. Begründen Sie, dass sich der Betrag der Bahngeschwindigkeit durch diese Kraft nicht ändert. (3BE)

<p style="margin-left:10%">

<details>

<summary> Hinweis </summary>

Überprüfe die Handregel und die Richtung der Lorentzkraft mit Hilfe von __1.2.__

</details>

<details>

<summary> Lösung Zeichnung </summary>

![Abi13_2_Lsg](https://diversewolken.ddns.net/nextcloud/index.php/s/SbMnFEaMHdqcEPn/download)

</details>

<details>

<summary> Lösung Begründung </summary>

Die Lorentzkraft @color($F_L$,purple) wirkt immer senkrecht zur Bewegungsrichtung. Eine Kraft, die auf einen Körper senkrecht zur Bewegungsrichtung wirkt, ändert nur die Richtung der Geschwindigkeit, nicht aber der Betrag (d.h. den Wert). Der Körper bewegt sich auf einer Kreisbahn.

</details>

</p>

2. 3. Ein einfach geladenes Ion der Masse $4,98\cdot 10^{−27} kg$ bewegt sich in einem Magnetfeld der Flussdichte $0,045 T$ auf einer Bahn mit dem Radius $0,15 m$. Berechnen Sie dessen Bahngeschwindigkeit. (3 BE)

<p style="margin-left:10%">

@rangeQuiz2($v$, 216867.5, $\frac{m}{s}$)

<details>

<summary> Hinweis 1 </summary>

Eine Information zur Ladung des Ions steckt im Text.

</details>

<details>

<summary> Hinweis 2 </summary>

Das Ion ist einfach geladen.

</details>

<details>

<summary> Hinweis 3 </summary>

Die Ladung des Ions beträgt eine Elementarladung.

</details>

<details>

<summary> Hinweis 4 </summary>

Nutzen Sie die hergeleitete Formel zur Berechnung des Bahnradius.

</details>

<details>

<summary> Lösung </summary>

<p class="newspaper">

geg.: 

<p style="margin-left:10%">

$B = 0,045 T$

$m = 4,98 \cdot 10^{-27} kg$

$r = 0,15 m$

$q = 1e = 1,6\cdot10{-19} C$

</p>

ges.: $v$

<p class="cb">

Lsg.:

<p style="margin-left:10%">

$r = \dfrac{v}{B\cdot \frac{q}{m}} \hspace{0.5cm}\Big | \cdot \Big(B\cdot \frac{q}{m}\Big)$

$v = \dfrac{r \cdot B \cdot q}{m}$

$v = 216867,5 \frac{m}{s} \approx 2,17\cdot 10^5 \frac{m}{s}$

</p>

</p>

</p>


</details>

</p>

### KI-Aufgabe: Bewegung eines Elektrons im B-Feld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung im B-Feld-Aufgabe:__<br> 

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">
Ich habe folgende 4 Aufgaben bekommen: <br> 1. Erkläre, warum sich ein geladenes Teilchen in einem homogenen Magnetfeld auf einer Kreisbahn bewegt.<br> 1. Gib begründet qualitativ an, wie sich der Kreisbahnradius mit zunehmender Geschwindigkeit verändert.<br> 2. Wiederhole Aufgabe. mit veränderter magnetischer Flussdichte.<br>3. Hat man Ionen identischer Geschwindigkeit und Ladung, kann man mit Hilfe eines homogenen Magnetfeldes einen Massenspektrograph, d.h. eine Trennung der Teilchen nach ihrer Masse erreichen. Erkläre, wie das funktionieren könnte.<br>
Stelle mir nacheinander die 4 Aufgaben. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungskurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln. Schätze meine Ergebnisse zusammenfassend ein.</span>
</div>
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


## Entwicklung Leistungen 11Ph2

{{0-1}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend(alt) |
| ---- | ---- | ---- |
| LK1 | 7.9 | 7.88 |
| KA1 | 6.3 | 8.2 |
| EX1 | 11.9| 8.52 |
| KA2 | 7.7 | 8.84 |
| LK2 | 8.8 | 9.16 |
| KA3 | 8.7 | 9.5 |
*********

{{1}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend(alt) | Trend(neu) |
| ---- | ---- | ---- | ---- |
| LK1 | 7.9 | 7.88 | 8.03 |
| KA1 | 6.3 | 8.2 | 8.2 |
| EX1 | 11.9| 8.52 | 8.4 |
| KA2 | 7.7 | 8.84 | 8.7 |
| LK2 | 8.8 | 9.16 | 8.9 |
| KA3 | 8.7  | 9.5 | 9.1 |
| KA4 |  | | 9.3 | 
*********

![Ergebnisse_KA3](https://diversewolken.ddns.net/nextcloud/index.php/s/8srboQ4cKEFebQ3/download)

## 7.4. e/m-Versuch mit Helmhotz-Spulen

![e_m_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/dtPMS5294W8Qi4q/download)

![e_m_TB2](https://diversewolken.ddns.net/nextcloud/index.php/s/MoMFPxGn8zjD4iL/download)

![e_m_TB3](https://diversewolken.ddns.net/nextcloud/index.php/s/ct7BCE29PDo546B/download)

![e_m_TB4](https://diversewolken.ddns.net/nextcloud/index.php/s/xM2z7xkdFfQXdes/download)

### Fehlerrechnung am e/m-Versuch

![Fehler_e_m1](https://diversewolken.ddns.net/nextcloud/index.php/s/3dMAx9wr4MTJxGQ/download)

![Fehler_e_m2](https://diversewolken.ddns.net/nextcloud/index.php/s/wyRd2H84Cr8w2J6/download)

### Lösung Übungsaufgabe Mikrotron

<p class="newspaper">

a) Die Lorentzkraft wirkt immer @color(senkrecht, red) zur Bewegungsrichtung der Elektronen, daher wirkt sie als Radialkraft (Zentripetalkraft) einer Kreisbewegung.

b) Im Uhrzeigersinn

c) $ r = \frac{m \cdot v}{B \cdot q} = 0,022 m$

d) Zuwachs der kinetischen Energie ist pro Umlauf

$$ E_{kin} = U \cdot e = 2,92 \cdot 10^{-17} J$$

Damit ergibt sich nach 10 Umläufen eine kinetische Energie von

$$ E_{kin-10} = U \cdot e = 2,92 \cdot 10^{-16} J$$

Die zugehörige Geschwindigkeit beträgt

$$ v = \sqrt{\frac{2\cdot E_{kin-10}}{m_e}} = 2,53 \cdot 10^7 \frac{m}{s}$$

und der Radius ist

$$ r = 7,1 cm$$

@color(Der Platzbedarf ist somit 14.2 cm., red)

<p class="cb">

e) Für die Umlaufzeit gilt:  $T_n = \frac{u_n}{v_n}$, wobei $u_n$ der Umfang der n-ten Bahn und $v_n$ die Geschwindigkeit der n-ten Bahn ist.

Für $u_n$ gilt: $u_n = 2 \pi r_n = 2 \pi \frac{m \cdot v_n}{B \cdot q}$

Für $v_n$ gilt: $v_n = \sqrt{\frac{2 \cdot U \cdot e \cdot n}{m}}$

Das heißt für $T_n$ gilt:

$$ T_n = \frac{u_n}{v_n} = \frac{2\pi \frac{1}{B} \sqrt{\frac{n \cdot 2\cdot U\cdot m}{e}}}{\sqrt{\frac{n\cdot 2 \cdot U \cdot e}{m}}} = \frac{2\pi m}{e\cdot B}$$

</p>

</p>

## 7.5. Anwendung - Geladene Teilchen in elektrischen und magnetischen Feldern

> __Aufgabe:__ Erstelle in einer kleinen Gruppe innerhalb der nächsten 45 Minuten eine kurze Präsentation zu einem dieser Themen. Jede Präsentation sollte nicht mehr als 5 min dauern.

<p class="newspaper">

__Mögliche Themen:__



<details>

<summary> Linearbeschleuniger [Johannes, Florian]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUOUY0MVlTR1FUWE5NM003TEM3V1BXMlZVNy4u)

</details>

<details>

<summary> Zyklotron [Gustav, Valentin W]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUMjQyS0dNOUNSUDRYQThXTEk3SklONUJXMi4u)

</details>

<details>

<summary> Synchrotron [Egor, Hannah]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUQkZVREtXSVZMVFQwVjVRV1NWNkwzQTVIOS4u)

</details>

<details>

<summary> Massenspektrometer [Oleg Torben] </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUMUk0M0NSQzQxMlFBOVBRUjBHVFBMQ0kyTS4u)

</details>

<details>

<summary> magnetische Flaschen (Plasmaphysik) [Theo, Max]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdURFhGRk9JTzJBUUZIWEtXTE1MMjQzODUxMS4u)

</details>

<details>

<summary> Elektronenmikroskopie [Christopher, Theo]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdURDZPNzNLMUtHR1EzMUdJMDZNT1IySFhUNC4u)

</details>

<details>

<summary> Ionenantriebe (Raumfahrt) [Valentin G, Till]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUQzlDMDJONjNGOVdQU1pRTFFOSkNTM1BNOC4u)

</details>

<details>

<summary> Protonentherapie [Fynn]  </summary>

[qr-code](https://forms.office.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUQzJHN082TjBSUTlDSUNKQ1A4UjJPMFo4WC4u)

</details>


<p class="cb">

__Inhalt:__

- kurze Einführung -> _Worum handelt es sich?_

- Anwendungsbereiche / Anwendungsbeispiele

- Erklärung der grundlegenden Physik: Teilchenbewegung in Feldern

- interessante Details / aktuelle Informationen

</p>

</p>