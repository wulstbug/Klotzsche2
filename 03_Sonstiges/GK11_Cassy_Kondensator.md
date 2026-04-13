
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

@color
<bdi style="color:@1">@0</bdi>
@end

@orange
<bdi style="color:orange">@0</bdi>
@end

@align
<p style="text-align: @1">@0</p>
@end

@indent
<div style="text-indent:@1">@0</div>
@end

@onload
window.LIA.settings.font_size = 2


const canvas = document.querySelector('.lia-canvas')
if (canvas) {
  canvas.classList.remove('lia-navigation--visible')
  canvas.classList.add('lia-navigation--hidden')
}

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

-->



## 1.7 Elektronische Schaltkreise mit Kondensatoren

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

### Einführungsvideo zu Mobile-Cassy 2

Youtube-Link

[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

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

Youtube-Link

[Tutorial Oszilloskop](https://www.youtube.com/watch?v=5vfNUj-2P4M)

### Experimentierüberblick

__Lernziele:__

- Cassy mit Tablet verbinden

- Ladekurve im Cassy mit Osszilloskopmodus aufnehmen

- Zeitkonstante berechnen

- Messparameter einstellen lernen (ohne Trigger)

- gespeicherte Ladung bestimmen

- Auswertung der Messdaten

__Physikalische Inhalte:__

- Kondensator C = 4600 µF, Ohmscher Widerstand R = 1 kOhm

- Zeitkonstante für Laden/Entladen $\tau=R\cdot C$

- Ladungsbestimmung via Berechnung $Q=C\cdot U$

- Ladungsbestimmung bei verschiedenen Spannungen mit Hilfe der Ladekurve

- Vergleichendes Diagramm erstellen

__Lernhilfen:__

- LB S. 75 Protokollgestaltung

- LB S. 76/77 Messfehler bei physikalischen Messungen

- Anleitung für Verbindung von Tablet und Cassy

- Anleitung zur Steuerung von Cassy

- Anleitung zum Aufbauen des Versuchs

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


### Teil 2 - neuer Widerstand (ca. 20min)

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

### Teil 3 - Vergleich (mind. 20 min)

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

