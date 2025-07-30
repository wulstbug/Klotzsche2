<!--
author: Christian Golnik

language: de

logo: https://img.welt.de/img/wirtschaft/webwelt/mobile218083858/8146580597-ci23x11-w2000/Out-Of-The-Blue.jpg

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

### 5.2.2 Berechnung des elektrischen Feldes

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

## 5.4. Die Kapazität

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


5. 6. 1. [LEIFI-Quiz zur Kondensatorformel](https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/aufgabe/quiz-zur-kondensatorformel)


## 5.7 Elektronische Schaltkreise mit Kondensatoren

### Einführungsvideo zu Mobile-Cassy 2

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

### 5.7.1 Experiment: Vorübung zur Schulung mit Cassy

### 5.7.2 Automatische Messwerterfassung mit Cassy:

## 5.8 Lade und Entladevorgang eines Kondensators

### 5.8.1 Theoretische Beschreibung des Lade- und Entladevorgangs an einem Kondensator

### 5.8.2 Der Zusammenhang von geflossener Ladung $Q$, Zeit $t$ und momentaner Stromstärke $I(t)$

## 5.9 Experiment Entladevorgang eines Kondensators

### 5.9.1. Vorbetrachtungen zum Versuch

### 5.9.2. Berechnung: Laden des Kondensators

### 5.9.3. Ermittlung einer sinnvollen Messzeit $T$

### 5.9.4. Berechnung: Integral der Entladekurve $I(t)$

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

### 5.9.8. Aufnahme der Entladekurve

### 5.9.9. Auswertung der Messkurve $I(t)$

### 5.9.10. Übersicht: Vergleich aller Ergebnisse

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

### Experimentieren am Kondensator (mit Lösung)

## 5.11 Potentielle Energie eines geladenen Teilchens im elektr. Feld

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

Ein Kondensator besteht aus zwei dünnen Metallfolien mit einer isolierenden Schicht (mit der Dielektrizitätszahl $\varepsilon_r = 9,6$ und der Dicke d = 0,70 μm) als Dielektrikum.

1. Berechnen Sie den benötigten Flächeninhalt pro Kondensatorplatte, um die Kapazität von $C=4,8\cdot10^{-3} F$ in einem Plattenkondensator mit diesem Dielektrikum zu erhalten.

<p style="margin-left:10%">

@rangeQuiz2($A$, 39.5 ,$m^2$)

</p>

2. Diskutieren Sie, welches Material als Dielektrikum sich eher eignen würde, damit sich für die Platten des Kondensators ein praktisch umsetzbarer Wert ergibt. Berechnen Sie eine mögliche Kondensatorfläche.