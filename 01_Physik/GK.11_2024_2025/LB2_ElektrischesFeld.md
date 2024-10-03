
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

.blue {
    color:blue
}

.green {
    color:darkgreen
}

.red {
    color:darkgreen
}
@end

@color
<div style="color:@1">@0</div>
@end

@onload
window.LIA.settings.font_size = 2
@end

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Grundkurs Physik 2024/2025 - LB II: Das elektrische Feld

![Blitzeinschläge](https://img.welt.de/img/wirtschaft/webwelt/mobile218083858/8146580597-ci23x11-w2000/Out-Of-The-Blue.jpg)

## 1.1 Grundlagen Elektrizität

### 1.1.1 Atomaufbau

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
<span style="color:orange">*Schau dir zur Veranschaulichung noch einmal die verschiedenen Atom-Modelle (LB S. 93) an.*</span>
![ModelleAtomaufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/Mw2YQeHk4bA3aaL/download)

************

### 1.1.2 Elektrisch geladene Atome und Körper

<span style="color:orange">*Ergänze und übernimm diese Wiederholung.*</span>

> Ein neutrales (nicht geladenes) Atom besitzt die [[ gleiche ]] Anzahl an Elektronen und Protonen. Ist die Anzahl der geladenen Elementarteilchen nicht gleich, so wird es als [[ Ion ]] bezeichnet. Das gleiche gilt für elektrisch geladene Körper. Negativ geladene Körper enthalten mehr [[ Elektronen ]] als Protonen und bei positiv geladenen Körpern ist es umgekehrt.

Negativ geladene Ionen nennt man [[ Anionen ]].

Positiv geladene Ionen nennt man [[ Kationen ]]

Beispiele:

Kohlenstoff mit 7 Elektronen ist elektrisch einfach [[ negativ ]] geladen. 

Germanium mit 34 Elektronen ist elektrisch [[ zwei ]]-fach [[ negativ ]] geladen.

__Übung:__

<iframe src="https://learningapps.org/watch?app=21709772" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### Physikalische Beschreibung der elektrischen Ladung

<span style="color:orange">*Nutze LB S. 88. Ergänze und übernimm dieses Tafelbild.*</span>

> Definition: Die elektrische Ladung eines Körpers gibt an, wie groß sein Elektronenüberschuss oder sein Elektronenmangel ist.
>
> __Formelzeichen: [[ Q ]]__
>
> __Einheit: 1 [[ C ]] ( [[ Coulomb ]] )__

Ein Elektron besitzt die kleinst mögliche Ladungsmenge, man nennt das eine __[[ Elementarladung ]] ($e$)__.

> $$ 1\,e = 1,602\cdot10^{-19} C $$

Die Anzahl $N$ der überzähligen Elementarladungen $e$ ergibt demnach die elektrische Ladung $Q$ eines Körpers. 

> $$Q = N \cdot e $$

### 1.2.3 Kräfte zwischen elektrisch geladenen Körpern

> Zwischen geladenen Körpern wirken elektrische Kräfte. Dabei stoßen sich gleichnamig geladene Körper ab, wohingegen sich ungleichnamig geladene Körper anziehen.

<span style="color:orange"> _Ergänze mit Hilfe des LBs die wirkenden Kräfte Kraftpfeile. Übernimm die Zeichnung in deinen Hefter._</span>
![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/Bwpb4qQF7jRzHYk/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

<details>

<summary> Lösung </summary>

![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/3bj6ESWb8DdS5m3/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

</details>

## 1.2 Das elektrische Feld

Im Raumbereich um einen __geladenen Körper__ wirkt auf einen anderen geladen Körper eine elektrische __Kraft__ ([Simulation elektrischer Kräfte](https://www.geogebra.org/classic/vbw299uv?embed)).

{{1}}
***********
> Um die Kraftwirkung im gesamten Raum zu __illustrieren__ wird der Begriff <span style="color:orange">elektrisches Feld</span> eingeführt.
***********

{{2}}
***********
> Das __elektrische Feld__ verdeutlicht die Kraftwirkung auf eine <span style="color:orange">positive Probeladung</span>, dargestellt durch so genannte <span style="color:orange">Feldlinien.</span> 
***********


{{3}}
***********
__Beispiele für elektrische Felder:__

| Radialfeld<br>(_inhomogen_) |  Dipolfeld<br>(_inhomogen_) | Homogenes Feld |
| {4}{![Radialfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/3r6ngsjZkRr4RD6/download)} | {5}{![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)} | {6}{![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)} |
| {4}{einzelne Punktladung} | {5}{zwei ungleichnamige Punktladungen} | {6}{Plattenkondensator} |

***********

{{7}}
***********
__Es gelten folgende Vereinbahrungen:__

- Feldlinien verlaufen von <span style="color:red">__Plus__</span> nach <span style="color:darkgreen">__Minus__</span>.

- die Richtung der Feldlinie gibt die Kraftrichtung auf eine <span style="color:red">__positive Probeladung__</span> an

- je dichter die Feldlinien in einem bestimmten Gebiet, desto größer ist die dort wirkende Kraft

- in einem __homogenen Feld__ (z.B. innerhalb eines Plattenkondensators) ist der Betrag der wirkenden Kraft überall gleich

- elektrische Feldlinien beginnen/enden senkrecht an einer Oberfläche
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

### Kurze Wiederholung zum elektrischen Feld

<p style="color:orange"> Bitte schau dir folgendes Video an. Bis zur Minute 3:00 ist es Wiederholung, dann folgenden Fakten zum elektrischen Feld, welche wir noch nicht besprochen haben. Du kannst es dir zur Information ansehen, musst du aber nicht. </p>

!?[ElektischesFeld](https://www.youtube.com/watch?v=EN6dTZH-HDs)

### 1.2.1 Berechnung des elektrischen Feldes

Die Stärke des elektrischen Feldes $\vec{E}$ berechnet sich aus der Kraft $\vec{F}$ auf eine elektrische Ladung $Q$.

> $$ \vec{E} = \frac{\vec{F}}{Q} $$
>
> <div style="color:orange">_Hinweis: Die Pfeile über $\vec{E}$ und $\vec{F}$ bedeuten, dass es sich um Vektoren mit einer Richtung und einem Wert (auch Betrag genannt) handelt. Kräfte haben wir bereits als Vektoren gezeichnet._ </div>
>
> Einheit: $$\Big[\dfrac{N}{C}\Big]$$
>
> $\hspace{1cm}$  <div style="color:orange">_Hinweis: $N$ (Newton) ist die Einheit der Kraft und $C$ (Coulomb) ist die Einheit der elektrischen Ladung._ </div>

### Aufgaben zum elektrischen Feld (1)

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

1. 3. Die Ladung des Tischtennisballs beträgt $Q = 0,1\cdot10^{-3} C =  5 mC $. Ermittle den Wert der Kraft $\vec{F}$, mit welche auf den TT-Ball wirkt.<br>(_Hinweis: Zwischen Zahl und Einheit bitte kein Leerzeichen._)

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

### Aufgaben zum elektrischen Feld (2)


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


