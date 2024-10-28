
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
<bdi style="color:@1">@0</bdi>
@end

@onload
window.LIA.settings.font_size = 2
@end

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Grundkurs Physik 2024/2025 - LB II: Das elektrische Feld

@color(__Checkliste zur Klausur__,red)

__Grundlagen Elektrizität [1.1]:__

- Kennen des Atomaufbaus, Elementarteilchen, Ladungszustände

- Kennen des Begriffs Elektrische Ladung, Kraftwirkungen auf elektrisch geladene Körper [Aufgabe 2]

__Grundlagen Elektrizität [1.2]:__

- Kennen des Begriffs und der Bedeutung des elektrischen Feldes

- Berechnung des elektrischen Feldes als Kraft auf Probeladung 

- Kennen von Eigenschaften elektrischer Felder und Arten von elektrischen Feldern 

__Kondensator [1.3/1.4]:__

- Kennen des Begriffs und Nutzen von Kondensatoren, Plattenkondensator als spezielle Bauform

- Berechnung des elektrischen Feldes eines Plattenkondensators und dessen Eigenschaften

- Kennen des Begriffs Kapazität als Fähigkeit Ladung zu Speichern, Berechnung allgemein und bei Plattenkondensator [-> Aufgabe 1]

- Kraftwirkung auf elektrische Ladungen im Feld eines Kondensators [-> Aufgabe 3/4]

__Energie im elektrischen Feld [1.5]:__

- Berechnung der Feldenergie

- Abhängigkeiten der im Kondensator gespeicherten Energie und der Kapazität des Kondensators [-> Aufgabe 5]

- Potentielle Energie einer Probeladung im elektrischen Feld eines Kondensators

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

### 1.1.3 Kräfte zwischen elektrisch geladenen Körpern

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


## 1.3. Der Kondensator

__Definition:__ Ein Kondenstator ist ein Bauelement zur __Speicherung von elektrischer Ladung__. Er besteht aus zwei leitenden Schichten, die durch einen Isolator (@color(Dielektrikum,orange)) voneinander getrennt sind @color([Vlg. LB S. 80], darkgrey).

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
- __das elektrische Feld__ $\vec{E}$ eines Plattenkondensators berechnet sich mit
*******

{{5}}
*******
> $$ \boxed{\vec{E} = \dfrac{U}{d}} $$
>
> $\hspace{1cm}$ $U$ ... Spannung zwischen den Platten $\big[ V \big]$ 
>
> $\hspace{1cm}$ $d$ ... Abstand der Platten $\big[ m \big]$ 

- wird in das elektrische Feld eine elektrische Ladung eingebracht, so wirkt auf die Ladung eine elektrische Kraft die mit $\vec{F}=\vec{E}\cdot q$ berechnet werden kann
*******

### Aufgabe 1. - Plattenkondensator

An einem Plattenkondensator beträgt die Spannung 1,5 kV und der Plattenabstand 3,2cm. 

Bestimme die Kraft, die auf einen Körper mit einer Ladung von 20 nC wirkt <br> @color(Hinweis: $nC=10^{-9}C$ [Nano-Coulomb], grey) <br> @color(Lösung: siehe Lehrbuch S.97, grey)


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

$A$ = .. $m^2$

$d$ = .. $m$

$\varepsilon_r$ = .. 

</div>

<p class="cb">

ges.:

<div style="text-indent:10%">

$C$

</div>

Lsg.:

<div style="text-indent:10%">

$C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} $

$C = .. F$ 

</div>

</p>

</p>

*********


### Aufgabe 2. Elektrische Ladung

__Löse LB. S. 122 6/8__  [Nutze hierfür __1.1 Grundlagen Elekrizität__](#1.1-grundlagen-elektrizität)

<div style="text-indent:10%">

Überprüfe deine Lösungen

<details>

<summary> Lösung S.122/6 </summary>

$N=\frac{0,1 C}{1,602\cdot10^{-19}C}\approx6,242 \cdot 10^{17} \textbf{Elektronen}$

</details>

<details>

<summary> Lösung S.122/8  </summary>

a) negativ

b) $Q = N \cdot e = 3,1\cdot10^{10} \cdot 1,602\cdot10^{-19} C = 4,966\cdot10^{-9} C \approx 5 nC $

</details>

</div>

### Aufgabe 3. Spannung am Kondensator*

__Bestimme die Spannung, die am Kondensator aus Aufgabe 1 [siehe 1.3 Der Kondensator](#1.3.-der-kondensator) anliegen muss, damit auf ein Elektron eine Kraft von 5 nN wirkt.__

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

Nutze Lösung der [Aufgabe 1.](#aufgabe-1.-plattenkondensator) und stelle die Formel nach U um.

> $1nN = 1 \cdot 10^{-9} N$

Ladung des Elektrons:

> $q=-1,602 \cdot 10^{-19}C$ (Nutze IQB-Formelsammlung -> Naturkonstanten S.50/51)

</details>

<details>

<summary> Lösung </summary>

![BildDerLösung](https://diversewolken.ddns.net/nextcloud/index.php/s/mtM5TLiakAzrisa/download)<!-- style="width:80%"-->

</details>

</div>

### Aufgabe 4. Geladenes Teilchen im Plattenkondensator

__Ein Plattenkondensator hat eine Querschnittsfläche der Platten von $50\,cm^2$. Der Abstand der Platten beträgt $2\,cm$. Der Kondensator ist horizontal aufgestellt, d.h. eine Platten unten, eine Platte oben. Zwischen den Platten sei Vakuum.__

4. 1. Bestimme die Kapazität dieses Kondensators.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.1. </summary>

Nutze die Formel zur Berechnung der Kapazität C eines Plattenkondensators. Achte auf die Umrechnungen von Fläche und Länge.

</details>

<details>

<summary> Lösung 4.1. </summary>

![Lsg_1.3_A4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/EKTW7ncRr3oSJcJ/download)<!-- style="width:80%"-->

</details>

</div>

4. 2. Zwischen den Platten befindet sich ein einzelnes Proton. Der Kondensator soll so geladen sein, dass das Proton zwischen den Platten schwebt. Zeichne dazu eine Skizze und gib die Pole an den Platten an. Zeichne die wirkenden Kräfte qualitativ ein.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.2. </summary>

Zeichne einen Plattenkondensator mit einer Platten oben und einer Platte unten. Zeichne in die Mitte das punktförmige Proton. Überprüfe, welche Kraft auf das Proton aufgrund seiner Masse wirkt. Zeichne diese Kraft ein. Da das Proton schweben soll, muss diese Kraft durch eine weitere Kraft genau aufgehoben werden. Zeichne auch diese Kraft ein. Überlege nun, wie die obere Platte geladen sein muss.

</details>

<details>

<summary> Lösung 4.2. </summary>

![Lsg_1.3_A4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/bW2JAqywjYBA2Wx/download)<!-- style="width:80%"-->

</details>

</div>

4. 3. Bestimme die Spannung, die am Kondensator angelegt werden muss, damit das Elektron schwebt.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.3. </summary>

Gewichtskraft und elektrische Kraft müssen gleich groß sein, damit das Proton schwebt. Recherchiere Masse $m_p$ und Ladung $q$ eines Protons mit Hilfe der IQB-Formelsammlung. Überprüfe im Skript die Formeln für Gewichtskraft und elektrische Kraft auf eine Probeladung im elektrischen Feld. Nutze die Formel für die elektrische Feldstärke in einem Plattenkondensator.

</details>

<details>

<summary> Lösung 4.3. </summary>

![Lsg_1.3_A4.3](https://diversewolken.ddns.net/nextcloud/index.php/s/Y8risbAANPaWwTq/download)<!-- style="width:80%"-->

</details>

</div>

## 1.5 Energie im elektrischen Feld

> Im elektrischen Feld eines Kondensators ist energie gespeichert und wird als __elektrische Feldenergie $E_{Feld}$__  bezeichnet.
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

5. 1. Ergänze folgende Aussage: Um die Feldenergie eines Kondensators zu erhöhen kann man:

     <!-- data-solution-button="off" -->
     [[X]] die Spannung verringern
     [[ ]] die Spannung erhöhen
     [[ ]] ein Dielektrikum zwischen die Platten des Kondensators einbringen
     [[X]] ein Dielektrikum zwischen den Platten des Kondensators entfernen
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

5. 6. Ein Plattenkondensator der zwischen den Platten mit Luft gefüllt ist hat eine Kapazität von 1 nF. Dann wird ein Stoff zwischen die Platten geschoben und die Kapazität erhöht sich auf den Wert 4 nF. Benenne den Stoff, der zwischen die Platten geschoben wurde.

     <!-- data-solution-button="off" -->
     [[ Porzellan ]]
     [[?]] Überprüfe in der Formel zur Berechnung der Kapazität eines Plattenkondensators [-> 1.4], welche physikalische Größe sich auf ein Material bezieht.
     [[?]] Das Material zwischen den Platten wird durch die Dielektizitätszahl $\varepsilon_r$ repräsentiert. Nutze die Formelsammlung für die Dielektrizitätszahl verschiedener Materialen.
     [[?]] Die Dielektrizitätszahl verschiedener Materialien wird in der Formelsammlung auf Seite 54 aufgeführt. Überprüfe, welches Material eine Dielektrizitätszahl von 4 besitzt.


5. 7. [LEIFI-Quiz zur Kondensatorformel](https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/aufgabe/quiz-zur-kondensatorformel)


## 1.6 Potentielle Energie elektrischer Ladungen im Feld eines Plattenkondensators

## 1.7 Pendel im elektrischen Feld

