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

$$ F_{el} = 3,68 \cdot 10^{-17} N\,\mathrm{(siehe\,5.)}$$

Die Masse des $\alpha$-Teilchens beträgt

$$ m_\alpha = 6,64 \cdot 10^{-27} kg $$

</details>

## 5.2 Das elektrische Feld

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

{{9}}
***********
<span style="color:orange">_Aufgabe: Zeichne das elektrische Feld einer positiv geladenen Punktladung, welche zentral vor einer negativ geladenen Kondensatorplatte positioniert ist. Bei Fragen nutze folgende Hinweise._</span>

<details>

<summary> Hinweis: Anordnung der Ladungen </summary>

![Aufgabe_1_L1](https://diversewolken.ddns.net/nextcloud/index.php/s/3mH8ApKdxxj52dJ/download)

</details>

<details>

<summary> Hinweis: Lage der Feldlinien </summary>

![Aufgabe_1_L2](https://diversewolken.ddns.net/nextcloud/index.php/s/DF6TktoF9Xgyg5A/download)

</details>
***********
