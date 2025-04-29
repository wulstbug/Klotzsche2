
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

@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0$\ =\ $
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

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Grundkurs Physik 2024/2025 - LB II: Das elektrische Feld

## 1.1 Grundlagen Elektrizität

### 1.1.1 Atomaufbau

### 1.1.2 Elektrisch geladene Atome und Körper

__Übung:__

<iframe src="https://learningapps.org/watch?app=21709772" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### Physikalische Beschreibung der elektrischen Ladung

### 1.1.3 Kräfte zwischen elektrisch geladenen Körpern

## 1.2 Das elektrische Feld

### Kurze Wiederholung zum elektrischen Feld

<p style="color:orange"> Bitte schau dir folgendes Video an. Bis zur Minute 3:00 ist es Wiederholung, dann folgenden Fakten zum elektrischen Feld, welche wir noch nicht besprochen haben. Du kannst es dir zur Information ansehen, musst du aber nicht. </p>

!?[ElektischesFeld](https://www.youtube.com/watch?v=EN6dTZH-HDs)

### 1.2.1 Berechnung des elektrischen Feldes

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

### Aufgabe 1. - Plattenkondensator

An einem Plattenkondensator beträgt die Spannung 1,5 kV und der Plattenabstand 3,2cm. 

Bestimme die Kraft, die auf einen Körper mit einer Ladung von 20 nC wirkt <br> @color(Hinweis: $nC=10^{-9}C$ [Nano-Coulomb], grey) <br> @color(Lösung: siehe Lehrbuch S.97, grey)

## 1.4. Die Kapazität

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

### Aufgabe 5: Feldenergie im Kondensator

5. 1. Ergänze folgende Aussage: Um die Feldenergie eines Kondensators zu erhöhen kann man:

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


## 1.6 Potentielle Energie elektrischer Ladungen im Feld eines Plattenkondensators

### Aufgabe zur elektrischen potentiellen Energie

6. Wir betrachten ein Elektron im elektrischen Feld eines Plattenkondensators. Im Raum zwischen den Platten sei Vakuum, die Platten haben eine Querschnittsfläche von $0,02\,m^2$, einen Abstand von $10\,cm$. Am Kondensator sei eine Spannung von $500\,V$ angelegt.

---

6. 1. Gib die elektrische Ladung und die Masse des Elektrons an.

     ---

     __Ergebnisse:__

     _Hinweis: 10er-Potenzen (z.b: $10^{-9}$ können hier mit dem Buchstaben $\footnotesize\textbf{E}$ angegeben werden (wie im CAS EXP-Taste)._

     ![GTR](https://diversewolken.ddns.net/nextcloud/index.php/s/939gMiCMEoNn7bL/download)<!-- style="width:80%" -->

@rangeQuiz2($\hspace{1cm}$ $q$, 1.602E-19, C)

---

@rangeQuiz2($\hspace{1cm}$ $m_e$, 9.109E-31, kg)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

siehe Formelsammlung _Naturkonstanten_

</details>

</div>

6. 2. Bestimme den Wert des elektrische Feldes innerhalb des Kondensators.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $E_{el}$, 5000, $\frac{V}{m}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

siehe Formelsammlung _Elektrisches Feld im Plattenkondensator_

</details>

</div>

---

6. 3. Ermittle die elektrische Kraft, die auf das Elektron wirkt und vergleiche sie mit der Gewichtskraft, die auf das Elektron wirkt.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $F_{el}$, 8.01e-16, $N$)

@rangeQuiz2($\hspace{1cm}$ $F_{g}$, 8.936e-30, $N$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zum Vergleich</summary>

Die elektrische Kraft $F_{el}=8.01\footnotesize\textbf{E}-16\,N$ ist viel viel größer, als die Gewichtskraft $F_g=8,94\footnotesize\textbf{E}-30\,N$. 

Mit anderen Worten, die Gewichtskraft kann man für dieses Beispiel vernachlässigen.

</details>

</div>

---

6. 4. Ermittle die potentielle elektrische Energie, die dem Elektron hinzugefügt wird, wenn es von der positiven Platte des Kondensators zur negativen Platten _angehoben_ wird.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $E_{pot\ el}$, 8.01e-17, $J$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Berechnung</summary>

siehe Skript 1.6: $E_{pot\,el} = F_{el} \cdot d$

</details>

</div>

---

6. 5. Wenn das Elektron an der negativen Platten angekommen ist, wird es aus der Ruhe heraus losgelassen. Ermittle die Beschleunigung, mit welcher das Elektron beschleunigt wird. Ermittle auch die Geschwindigkeit, die es besitzt, wenn es bei der positiven Platten ankommt (nutze dafür die Energieerhaltung). <br> _Hinweis: Hier kommen sehr große Werte heraus._

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $a$, 8.794e14, $\frac{m}{s^2}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Beschleunigung</summary>

Die Beschleunigung lässt sich nach dem zweiten Newton'schen Gesetz berechnen.

<details>

<summary> Berechung zur Beschleunigung</summary>

$$ F_{el} = m_e \cdot a$$ 

$$ a = \frac{F_{el}}{m_e} = \frac{8,01 \cdot 10^{-16} N}{9,11 \cdot 10^{-31} kg}$$ 

$$ a = 8,79 \cdot 10^{14} \Big[ \frac{N}{kg} = \frac{m}{s^2} \Big] $$ 

</details>

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $v$, 1.326e7, $\frac{m}{s}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Geschwindigkeit</summary>

Setze die potentielle elektrische Energie aus 6.4 mit der kinetischen Energie gleich und löse nach der Geschwindigkeit auf.

<details>

<summary> Berechung zur Geschwindigkeit</summary>

$$ E_{pot\,el} = E_{kin}$$ 

$$ E_{pot\,el} = \frac{1}{2}\cdot m_e \cdot v^2$$ 

$$ v = \sqrt{ \frac{2\cdot E_{pot\,el}}{m_e}} = \sqrt{ \frac{2\cdot 8,01 \cdot 10^{-17} J}{9,019 \cdot 10^{-31} kg}} $$ 

$$ v = 1,326 \cdot 10^{7} \frac{m}{s} $$

</details>

</details>

</div>

### Lösungen Lehrbuchaufgaben

@color(_Auf Wunsch hier ein paar Lösungen zu Übungsaufgaben.<br><br> MfG CG_<br><br>, orange)

---

__LB S. 123 Aufgabe 15__

<div style="text-indent:10%"> 

<details>

<summary> Lösung a) </summary>

![Lsg_LB123_15](https://diversewolken.ddns.net/nextcloud/index.php/s/W3SQgTE7JErmfbb/download)<!-- style="width:80%"-->

</details>


<details>

<summary> Lösung b) </summary>

![Lsg_LB123_15](https://diversewolken.ddns.net/nextcloud/index.php/s/rjwJHMBwm3NbwrT/download)<!-- style="width:80%"-->

</details>

</div>

---

__LB S. 123 Aufgabe 17__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB123_17](https://diversewolken.ddns.net/nextcloud/index.php/s/9wA3JnFcLnmWqEZ/download)<!-- style="width:80%"-->

</details>


</div>

---

__LB S. 124 Aufgabe 23__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB123_17](https://diversewolken.ddns.net/nextcloud/index.php/s/JRCxMQoBCgFDWcW/download)<!-- style="width:80%"-->

</details>


</div>

### Sim1 Elektronische Schaltkreise mit Kondesatoren

??[PhET-Kondensator1](https://phet.colorado.edu/sims/html/capacitor-lab-basics/latest/capacitor-lab-basics_all.html?locale=de)

### Sim2 Elektronische Schaltkreise mit Kondensatoren

??[PhET-Kondensator2](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac/latest/circuit-construction-kit-ac_all.html?locale=de)

## 1.7 Elektronische Schaltkreise mit Kondensatoren

@color(_Hinweis: Für die folgenden Unterrichtseinheiten werden wir mit dem Formelzeichen $Q$ immer die Ladung auf den Platten des Kondensators bezeichnen._,darkgrey) 

<br>

__Wiederholung:__ Schließen wir den Kondensator an eine Gleichspannungsquelle (Spannung $U-$) an, so fließen elektrische Ladungen auf den Kondensator. Im Kondensator wird die Ladungsmenge $Q$ gespeichert.


<p class="newspaper">

__Ladung $Q$__

<p style="margin-left:5%">

Die Ladung $Q$ beschreibt Anzahl von Elemtarladungen $e$.

_Einheit: 1C (1 Coulomb)_

$$ \boxed{1 e = 1,6 \cdot 10^{-19} C} \,\,\,\mathrm{oder}\,\,\, \boxed{1C = 6,24 \cdot 10^{18} e}$$

</p>

---

__Spannung $U$__


<p style="margin-left:5%">

Die Spannung $U$ beschreibt den @color(das Potential bzw. den Antrieb für das Fließen von Ladungsträgern, orange). 
Je größer die Spannung, desto größer ist die gespeicherte Ladung.

_Einheit: 1V (1 Volt)_

</p>

---

__Stromstärke $I$__

<p style="margin-left:5%">

Die Stromstärke $I$ beschreibt <bdi style="color:orange">die Menge der elektrischen Ladungen $Q,$ die pro Sekunde durch einen Leiterquerschnitt fließen</bdi>.

_Einheit: 1A (1 Ampere)_

_Eine Stromstärke von 1A bedeutet, dass pro Sekunde eine Ladung von 1 C fließt._

$$ \Big[ A = \frac{C}{s} \Big] $$

</p>

--- 

__Gespeicherte Energie $E_{Feld}$__

<p style="margin-left:5%">

Die im Kondensator (im elektrischen Feld) gespeicherte Energie $E_{Feld}$ wird berechnet mit

$$ E_{Feld} = \frac{1}{2}\cdot Q \cdot U $$

$$ E_{Feld} = \frac{1}{2}\cdot C \cdot U^2 $$

_Einheit: 1J (1Joule)_

</p>

<p class="cb">

__Schaltplan zum Laden des Kondensators__

![Schaltkreis_Kondensator1](https://diversewolken.ddns.net/nextcloud/index.php/s/ARdjFMxTDoDoAWz/download)

</p>

</p>

### 1.7.1 Experiment: Vorübung zur Schulung mit Cassy

__Aufgabenstellung:__ Nimm mit die U-I-Kennlinie für einen ohmschen Widerstand ($R=512\Omega$) auf. Variiere die Spannung in Schritten von 1 V im Intervall 0 - 10 V.


<p style="color:blue">

__Durchführung:__ _(muss nicht notiert werden)_ 

1. Übernimm Überschrift und Aufgabenstellung auf eine neue Seite.

2. Übernimm den Schaltplan und die zugehörige Tabelle für die Messwerte.

3. Stelle das Cassy-Messgerät anhand der Erklärungen ein.

4. Variiere die Spannung an der Spannungsquelle von 0..10V in Schritten von 1 V. Notiere Spannung und Stromstärke an Cassy-Messgerät.

5. Zeichne eine U-I-Kennlinie: Zeichne dazu ein Diagramm (x-Achse: U in V | y-Achse: I in A).

6. Öffne die nächste Seite: @color(_1.7.2 Automatische Messwert-Erfassung mit Cassy_,darkgreen). Folge den Anweisungen und wiederhole die Messung mit einer Automatischen Messwert-Aufname.

</p>

<p class="newspaper">

__Schaltkreis:__

![Schaltkreis_Exp1](https://diversewolken.ddns.net/nextcloud/index.php/s/rAwYZqysffqknd6/download)

__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | |
| 1 | |
| 2 | |
| .. | |
| 9 | |
| 10 | |

__Diagramm Kennlinie:__

![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/Z9at8rKH75N4Agt/download)

<p class="cb" style="color:blue">

__Einstellen des Cassy-Messgerätes:__

_(muss nicht notiert werden)_

1. Schließe den blauen Anschluss (_I_) an den Minuspol der Spannungsquelle. Der schwarze Anschluss wird an den Widerstand angeschlossen.

2. Schalte das Cassy-Messgerät ein. Im oberen linken Bereich des Fensters sind die messbaren Größen dargestellt. Deaktiviere mit [Cursor-Rad + OK] die Spannung und aktiviere die Stromstärke.

![VGl-Cassy1](https://diversewolken.ddns.net/nextcloud/index.php/s/e7eaHcHB4YkGf95/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Klicke auf das Symbol für Stromstärke (I) und stelle für den (Mess-)Bereich [-0,03A .. 0,03A] ein. Wechsle zurück Anzeige der Stromstärke. Achte auf: __Nullpunkt links__.

![VGl-Cassy2](https://diversewolken.ddns.net/nextcloud/index.php/s/JiSJbjqy3SkS2CN/download)<!-- style="max-width:80%;margin-left:10%" -->

</p>

</p>

### Einführungsvideo zu Mobile-Cassy 2

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

### 1.7.2 Automatische Messwerterfassung mit Cassy:

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

### 1.7.3 Aufgaben zur Berechnung an Kondensatoren

1. Ein Plattenkondensator mit Luft gefüllt besteht aus zwei kreisförmigen Platten mit dem Radius 5,5 cm. Die Platten haben einen Abstand von 7,0 cm. 

1. 1. Ermitteln Sie die Kapazität des Kondensators in pF.

@rangeQuiz2($\hspace{1cm}$ $C$, 1.2, $pF$)

<details style="margin-left:10%">

<summary> Lösung 1.1 </summary>

$$C = 8,86\cdot 10^{-12} \cdot \frac{\pi (5,5\cdot 10^{-3})^2}{7\cdot 10^{-2}} \hspace{1cm} \Big[ \frac{A\cdot s}{V\cdot m} \frac{m^2}{m} = \frac{A\cdot s}{V} = \frac{C}{V} = F \Big]$$

</details>

---

1. 2. Geben Sie zwei Möglichkeiten an, wie die Kapazität vergrößert werden kann, ohne das die geometrischen Größe der Platten verändert wird.

<details style="margin-left:10%">

<summary> Lösung 1.2 </summary>

- Stoff mit höherer Dielektrizitätskonstante einfügen

- Plattenabstand s verkleinern

</details>

---

2. Ein Kondensator hat einen Kapazität von 200µF. Ermitteln Sie die Ladung Q, welche sich auf dem Kondensator befindet, wenn er an eine Spannung von 14 V angeschlossen wird.

@rangeQuiz2($\hspace{1cm}$ $Q$, 2.8E-3, $C$)

---

3. Die in einem Kondensator bei einer Ladespannung von 8,0 V gespeicherte elektrische Feldenergie $E_{Feld}$ soll für die Zündung einer Blitzlichtlampe genutzt werden. Für den Lichtblitz wird eine elektrische Energie von 20 mJ benötigt. Berechnen Sie die Kapazität des Kondensators in der Einheit µF.

@rangeQuiz2($\hspace{1cm}$ $C$, 625, $\mu F$)

<details style="margin-left:10%">

<summary> Lösung 3 </summary>

$$ E_{Feld} = \frac{1}{2} \cdot C \cdot U^2 $$

$$ C = \frac{2 \cdot 0,02 J}{8V^2} = 0,000625 F = 625 µF $$

</details>

## 1.8 Lade und Entladevorgang eines Kondensators

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


### 1.8.1 Theoretische Beschreibung des Ladevorgangs an einem Kondensator

__Schaltplan:__ Lade- und Entladevorgang eines Kondensators

<p class="newspaper">

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/mK4zfakTRqYPmG3/download)

<p class="cb">

__Ladekreis__ 

- Wird der Ladekreis geschlossen, so fließen elektrische Ladungen (angetrieben durch die Spannung) von den Polen auf die Platten des Kondensators <br> @color(-> die Ladung $Q$ auf den Kondensatorplatten wird größer, orange)

- da sich gleichnamige Ladungen auf den Kondensatorplatten abstoßen, sinkt die Anzahl der Ladungsträger die pro Sekunde auf die Kondensatorplatten fließen <br> @color(-> während des Ladevorgangs nimmt die Ladestromstärke $I$ ab, orange)

- der zeitliche Verlauf der Stromstärke $I(t)$ kann mit <br> $$ I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t} $$ <br> beschrieben werden. Hierbei gilt $ \hspace{0.5cm} I_0 = \dfrac{U}{R} $

- Beispielhafter Graph $I(t)$ -> die Stromstärke I nimmt mit der Zeit exponentiell ab <br> ![Ladekurve_1](https://diversewolken.ddns.net/nextcloud/index.php/s/knoEKKZaKBL9q6w/download)

</p>

</p>

### 1.8.2. Simulation

_Aufgaben:_ 

1. Erstelle anhand des Schaltplans (siehe 1.8.1) in der Simulation einen Lade- und Entladekreis für einen Kondensator. <br> Link: [Simulation-Ladekurve](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac/latest/circuit-construction-kit-ac_all.html?locale=de) <br>  Wähle in der Simulation die Option __Labor__.

<details style="margin-left:10%">

<summary> Lösungshinweis bei Problemen </summary>

![LösungLadekurve](https://diversewolken.ddns.net/nextcloud/index.php/s/gsJ8NSCt5DsgXcm/download)

</details>

---

2. Beobachte, wie die Stromstärke mit zunehmender Ladung auf den Kondensatorplatten abnimmt.

---

3. Nutze das Stromstärke Diagramm um eine simulierte Messung durchzuführen. Erstelle davon einen Screenshot.

---

### Tutorial Oszilloskop-Modus mit Cassy 2

!?[Tutorial Oszilloskop](https://www.youtube.com/watch?v=5vfNUj-2P4M)



## 1.9 Experiment Entladevorgang eines Kondensators

__Aufgabenstellung:__ Untersuche den Entladevorgang eines Kondesators mit Hilfe der elektronischen Messwerterfassung ***Mobile Cassy 2***.

__Teilaufgaben:__ (_können_ in selbst gewählter Reihenfolge bearbeitet werden)

- [ ] Inhalten eines Protokolls notieren

- [ ] Vorbetrachtungen zum Versuch vornehmen und notieren

- [ ] ***Mobile Cassy 2*** mit Tablet verbinden

- [ ] Einstellen der Parameter am Cassy

- [ ] Schaltkreis zur Messung aufbauen @color(und von Lehrkraft abnehmen lassen, red)

- [ ] Messwerte aufzeichnen

- [ ] Daten auswerten und Ergebnisse analysieren

- [ ] Ergebnisse formulieren

### Inhalte eines Protokolls

Nutzen Sie Lehrbuch Seite 75 und erarbeiten Sie sich die wesentlichen Inhalte eines Protokolls

### Vorbetrachtungen zum Versuch

<p class="newspaper">

__Schaltplan:__

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/JqJRbJpBMJXNwTq/download)

<p class="cb">

__Ladekreis__ 

Der Kondensator wird in dieser Schaltung direkt über die Spannungsquelle und ohne ohmschen Widerstand aufgeladen.

__Entladekreis:__

Wird der Entladekreis geschlossen, fließt die auf dem Kondensator gespeicherte Ladung $Q$ über den ohmschen Widerstand $R$ ab. Dabei wird mit der elektronischen Messwerterfassung _Cassy_ der Entladestrom $I$ in Abhängigkeit der Zeit $t$ aufgenommen. Die gesamte Messzeit wird mit $T$ bezeichnet (s.u.).

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

Die Fläche unter dem $I(t)$ Graphen kann mit Hilfe des Cassy-Messgerätes ausgewertet werden.

*****

{{3}}
*****
__Ermittlung der Messdauer $T$ für Cassy:__

Für die Kombination aus Kondensator (Kapazität $C$) und ohmscher Widerstand (Widerstand $R$) kann eine Zeitkonstante $\tau$ ermittelt werden: 

$$ \boxed{\tau = R \cdot C} \Rightarrow \boxed{T = 4 \cdot \tau} $$

Als Messdauer $T$ für die elektronische Erfassung wird eine Zeit von @color($4\tau$,red) empfohlen. Nach dieser Zeit sind ca. $98,2\%$  der Gesamtladung Q abgeflossen.
*****

</p>

</p>

### Anleitung zur Verbindung von Cassy und Tablet

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

### Einstellen der Messparameter am Cassy

__Grundlage:__ Hier werden die Messparameter eingestellt

__Arbeitsablauf:__

- wechseln Sie auf der linken Seite zu Einstellungen

- hier müssen Sie den Messbereich für die Stromstärke einstellen __0,03 A__ und den Nullpunkt (des Diagramms) auf __links__ setzen(_Hinweis: diese Einstellung kann auch im Cassy direkt vorgenommen werden_)

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/KQLjMB5CoYRR34o/download)<!-- style="max-width:80%; margin:5%"-->

- wechseln Sie auf der linken Seite zu ***Diagramm*** und vergleichen Sie Ihre Anzeige

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9APdepf3in8wQ86/download)<!-- style="max-width:80%; margin:5%"-->

### Aufbau der Messchaltung

$ \red{\boxed{\mathrm{Es\ muss\ keine\ Gewalt\ angewendet\ werden.}}}$

__Grundlage:__ Für diesen Versuch ist der Schaltplan in den Vorbetrachtungen des Versuchs gezeichnet. 

__Materialien:__ Sie erhalten einen Kondensator mit der Kapazität $4700 \mu F$ und einen ohmschen Widerstand mit $1000 \Omega$.

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

### Aufnahme der Entladekurve

$ \red{\boxed{\mathrm{Die Schaltung\ muss\ abgenommen\ worden\ sein.}}}$

__Grundlage:__ Hier wird der Kondensator zunächst geladen. Dann wird die automatische Messung mit dem _Cassy_ gestartet und die Entladekurve wird aufgezeichnet.

- legen Sie den Wechselschalter in die Ladeposition

- schalten Sie die Spannungsquelle ein und wählen eine Spannung von 10 V

- starten Sie anschließend die Messung auf dem _Cassy_ indem Sie oben auf __"Messzeit nicht vorgegeben"__ klicken, legen Sie anschließend den Schalter um

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/dDiiE3cYDgGqM3W/download)<!-- style="max-width:80%; margin:5%"-->

- stoppen Sie die Messung nach etwa $T=4\tau$ (4 charaktieristischen Zeiteinheiten)

- achten Sie darauf, dass die eigentliche Entladung erst beginnt, wenn Sie den Schalter umlegen


### Auswertung einer Messung

__Grundlage:__ Hier werden die Messdaten ausgewertet.

__Ermittlung der geflossenen Ladung:__

- wählen Sie unter Auswertungen (unterhalb des Diagramms) den Menupunkt _"Fläche zur x-Achse"_

- angezeigt wird die geflossene Ladung in der Einheit $A\cdot s = C$ 

- notieren Sie den Messwert

![Cassy_-_Auswertung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/BXHx8eeCy8oXBSD/download)<!-- style="max-width:80%; margin:5%"-->

__Diagramm zeichnen aus einzelnen Messwerten:__

- wechseln Sie auf der linken Seit zum Reiter __Tabelle__

- notieren Sie in einer Messwerttabelle __t in s__ und __I in A__ und übernehmen Sie 10 charakteristische Messwerte

- zeichnen Sie anschließend den I(t)-Graph für Ihre Messwerte in das Protokoll

## 1.10 Untersuchungen am Entladevorgang eines Kondensators

@timer(60,00)

### Teil 1 - Wiederholung (ca. 20 min)

<details>

<summary>
</summary>

<p style="margin-left:5%">

__Aufgabenstellung:__ 

- [ ] @color(Bauen Sie den Entladekreis eines Kondensators anhand der Erklärungen 1.9 auf. , blue)

- [ ] @color(Lassen Sie sich die Schaltung abnehmen. ,red)

- [ ] @color(Ermitteln Sie die auf dem Kondensator gespeicherte elektrische Ladung. ,blue)

- [ ] @color(Überprüfe Sie mit Hilfe der Kontrollboxen Ihre Messwerte. Achten Sie dabei auf die geforderten Einheiten. ,blue)

__Daten/Messwerte zur Kontrolle:__ 

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 1000 , $\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4.7 , $mF$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 4.7 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 18.8 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.01 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

</p>

</details>

---

### Teil 2 - neuer Widerstand (ca. 20min)

<details>

<summary>
</summary>

<p style="margin-left:5%">

__Aufgabenstellung:__ 

- [ ] @color(Lassen Sie sich von der Lehrkraft einen neuen Widerstand $470\Omega$ aushändigen. , blue)

- [ ] @color(Tauschen Sie die Widerstände aus., blue)

- [ ] @color(Widerholen Sie den Experimentierablauf. Überprüfen Sie die neuen Parameter anhand der Kontrollwerte., blue)

- [ ] @color(Notieren Sie sich Ihre Werte zur Messung mit dem neuen Widerstand., red)

__Daten/Messwerte zur Kontrolle:__ 

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 0.47 , $k\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4700 , $\mu F$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 2.209 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 8.836 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.0213 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

- [ ] @color(Sollten Sie noch mehr als 30min Restzeit zur Verfügung haben: Wiederholen Sie die Messung für einen $2.2 k\Omega$-Widerstand., blue)

<details>

<summary> __Daten/Messwerte zur Kontrolle:__ </summary>

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 2200 , $\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4700 , $\mu F$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 10.34 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 41.36 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.0045 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

</details>

</p>

</details>

---

### Teil 3 - Vergleich (mind. 20 min)

<details>

<summary>
</summary>

<p style="margin:5%">

- [ ] @color(Vergleichen Sie für beide Messungen folgende Werte in einer Tabelle. Ergänzen Sie diese Tabelle in Ihren Aufzeichnungen. , blue)


{{0-1}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | ..                 | .. | .. | .. | .. |
| Teil 2  | ..                 | .. | .. | .. | .. |
| @color(_optional_, darkgrey) | ..                 | .. | .. | .. | .. |
************

{{1-2}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | .. | .. | .. |
| Teil 2  | 10                 | 470 | .. | .. | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | .. | .. | .. |
************

{{2-3}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | .. | .. |
| Teil 2  | 10                 | 470 | 0,021 | .. | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | .. | .. |
************

{{3-4}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | 18,8 | .. |
| Teil 2  | 10                 | 470 | 0,021 | 8,8 | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | 41,4 | .. |
************

{{4}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | 18,8 | 0,047 |
| Teil 2  | 10                 | 470 | 0,021 | 8,8 | 0,047 |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | 41,4 | 0,047 |
************

- [ ] <bdi style="color:blue">Überprüfen Sie den Zusammenhang von Ladespannung, Kapazität und gespeicherter Ladung. Formulieren Sie ein Ergebnis.</bdi> 


{{5}}
********
@color(Der Widerstand hat keinen Einfluss auf die gespeicherte Ladung. Die gespeicherte Ladung kann mit der Formel $Q=C\cdot U$ berechnet werden. , orange)
********

- [ ] <bdi style="color:blue">Stellen Sie anhand Ihrer Daten eine Vermutung über den Einfluss des eingesetzten Widerstands $R$ beim Entladen des Kondensators auf. Gehen Sie dabei auf Ladespannung, Entladezeit, maximale Stromstärke und gespeicherte Ladung ein. Formulieren Sie ein Ergebnis</bdi>

{{6}}
********
@color(Je größer der Widerstand desto langsamer erfolgt die Entladung. Die Entladezeit kann mit $T=4\cdot \tau = 4 \cdot R \cdot C$ berechnet werden. , orange)
********


- [ ] @color(Überprüfen Sie den Zusammenhang von Ladespannung Widerstand und maximaler Stromstärke. Formulieren Sie ein Ergebnis, blue)

{{7}}
********
@color(Der Zusammenhang von Widerstand R Ladespannung U und maximaler Stromstärke folgt dem ohmschen Gesetz $R=\frac{U}{I_{max}}$. , orange)
********


</p>

</details>
