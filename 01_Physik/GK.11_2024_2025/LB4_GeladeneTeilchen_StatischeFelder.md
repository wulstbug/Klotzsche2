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



# Grundkurs Physik 2024/2025 - LB IV - Geladene Teilchen in statischen Feldern

![ProtonCollisionCern](https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg)

## 1.1. Geladene Teilchen in statischen Magnetfeldern

_Tafelbildvideo zur Lorentzkraft:_

!?[TB_Video_Lorentzkraft](https://youtu.be/f0BNQ6uSvIQ)

<br>

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Lorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/tE56E3MWpqtozxx/download)

</details>


## 1.2. Hand-Regel zur Richtungsbestimmung der Lorentzkraft

_Bitte anschauen und ausprobieren_

!?[HandRegel](https://www.youtube.com/watch?v=snM3g4zWeNw)

__Bemerkungen zur Lorentzkraft:__

_Bitte Lückentext und weiteres probieren_

@color(siehe LB. S. 110, blue)

??[Lorentzkraft_LearningApps](https://learningapps.org/4454537)

__Tafelbild:__

![TB_KräfteAufBewegteElektrischeLadungen](https://diversewolken.ddns.net/nextcloud/index.php/s/aBZZK9rneamRSyf/download)


### Übungsaufgaben zur Lorentzkraft

1. Bitte schau dir zunächst dieses kleine Quiz zur Richtungsbestimmung der Lorentz-Kraft an.

      [QuizZurLorentzkraftRichtung](https://www.leifiphysik.de/elektrizitaetslehre/bewegte-ladungen-feldern/aufgabe/quiz-zu-bewegten-ladungen-im-magnetfeld)

      _Hinweis: Die magnetischen Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, green)._

---

2. Berechne für das Beispiel im Tafelbild die Lorentzkraft, wenn die Geschwindigkeit des Elektrons $v_e = 1\cdot 10^5 \frac{m}{s}$ und die magnetische Flussdichte $B = 0,2 mT$ beträgt.

<p style="margin-left:10%">

__Endergebnis:__

@rangeQuiz2($F_L$, 3.204e-18 , $N$)

__Zwischenwert:__

@rangeQuiz2($q_e$, 1.602e-19 , $C$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Ermittle mit der Formelsammlung die Ladung eines Elektrons $q_e$. Setze diese Werte in die Formel für die Lorentzkraft ein.

</details>

<details>

<summary> __Lösung__ </summary>

Die Bedingung Geschwindigkeit steht senkrecht auf Feldlinien ist gegeben.

$$F_L = q_e \cdot v_e \cdot B$$

$$ F_L = 1,602\cdot10^{-19}C \cdot 1\cdot 10^5 \frac{m}{s} \cdot 0,2 \cdot 10^{-3} T $$

$$ \underline{F_L = 3,204\cdot 10^{-18} N}$$

</details>


</p>

---

3. Die Lorentzkraft wirkt in jedem Moment senkrecht zur Flugbahn des Elektrons. Nenne die Form der Flugbahn auf der sich das Elektron bewegt, wenn eine Kraft immer senkrecht zur Bewegungsrichtung wirkt.

<p style="margin-left:10%">

- [( )] geradlinig
- [( )] parabelförmig
- [(x)] kreisförmig
- [( )] eckig

</p>

---

4. Die Flugbahn eines Elektrons in einem statischen magnetischen Feld ist eine Kreisbahn. Die Lorentzkraft $F_L$ wirkt als Zentritedalkraft $F_Z$ (siehe LB I, Kreisbewegung). Ermittle den Radius der Kreisbahn für die Aufgabe 2.

<p style="margin-left:10%">

@rangeQuiz2($r$, 0.00284 ,$m$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Um die Kreisbahn zu berechnen muss man (wie in der Aufgabe beschrieben) die Formel für die Zentripetalkraft $F_Z$ gleich der Formel für die Lorentzkraft $F_L$ setzen. $F_Z$ wurde in __LB I -> Kreisbewegung__ notiert.

<details style="margin-left:10%">

<summary> __Hinweis zur Formel__ </summary>

$F_Z = F_L$

$\hspace{2cm}$ mit $\boxed{F_Z = \dfrac{m\cdot v^2}{r}}$ und $\boxed{F_L = q \cdot v \cdot B}$

$ \dfrac{m\cdot v^2}{r} = q \cdot v \cdot B$

$\hspace{2cm}$ Nun noch nach $r$ umstellen und ausrechnen.

</details>

</details>

<details>

<summary> __Lösung__ </summary>

Aus dem Ansatz: 
$$F_Z = F_L$$

wobei die Zentripetalkraft $F_Z$ gleich 

$$F_Z = \dfrac{m\cdot v^2}{r}$$ 

und die Lorentzkraft $F_L$ gleich

$$F_L = q \cdot v \cdot B$$

ergibt sich für $r$

$$ r = \dfrac{m\cdot v}{q\cdot B}$$

mit den Werten:

$$ m_e = 9,11\cdot10^{-31} kg$$

$$ q_e = 1,602\cdot10^{-19} C$$

$$ v_e = 1 \cdot 10^5 \frac{m}{s}$$

$$ B = 0,2 mT = 0,2 \cdot 10^{-3} T$$

$$\boxed{\underline{\Rightarrow r = 2,84\cdot10^{-3} m}}$$

</details>

</p>

### Demonstrationsexperiment: Kräfte auf bewegte elektrische Ladungen in Magnetfeldern

@color(siehe LB. S. 110, blue)

![FotoLorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/mLFceeEL2jP7BDC/download)


## 1.3. Flugbahn von Elektronen in einem statischen, homogenen Magnetfeld

@color(siehe LB. S. 110, blue)

![TB_Flugbahn_Elektron_Magnetfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/gmPT93dWaFALw3f/download "Herleitung des Flugbahnradius")



### Aufgaben zur Vorbereitung der LK

#### 1. Vermischte Aufgaben

1. 1. Welche Eigenschaften muss ein Elektromagnet haben, der ein möglichst starkes Magnetfeld erzeugt?

<p style="margin-left:10%">

<details>

<summary> Hinweis </summary>

Untersuchen Sie den Einfluss der physikalischen Größen zur Berechnung der magnetischen Flussdichte $B$ in einer schlanken Spule.

</details>

<details>

<summary> Lösung </summary>

- Große Windungszahl $N$
- Kurze Baulänge $ℓ$
- Eisenkern
- Große Stromstärke $I$ (dicker Draht)

</details>

</p>

1. 2. In einer Spule (relative Dielektrizitätszahl = 1) mit 800 Windungen, einer Länge von 5 cm und einem Widerstand von 45 Ohm soll ein magnetisches Feld mit einer magnetischen Flussdichte von 12mT erzeugt werden. <br> a) Berechne die Spannung, die an die Spule angelegt werden muss. <br> b) Geben Sie zwei Möglichkeiten an, mit der man die magnetische Flussdichter verdoppeln kann.

<p style="margin-left:10%">

@rangeQuiz2($U$,26.786,$V$)

<details>

<summary> Zwischenergebnis </summary>

@rangeQuiz2($I$,0.595, $A$)

</details>

<details>

<summary> Hinweis a) </summary>

Ermittlen Sie zunächst die elektrische Stromstärke $I$, die fließen muss, damit das geforderte Magnetfeld erzeugt werden kann. <br> Nutzen Sie im Anschluss den Zusammenhang von Spannung $U$, Stromstärke $I$ und Widerstand $R$ um die Spannung zu ermittlen.

</details>

<details>

<summary> Lösung a) </summary>

<p class="newspaper">

geg.: 

<p style="margin-left:10%">

$B = 12 mT = 12 \cdot 10^{-3} T$

$N = 800$

$\mu_r = 1$

$R = 45 \Omega$

$ℓ=5cm = 5\cdot10^{-2}m$

</p>

ges.: $I$, $U$

<p class="cb">

Lsg.:

$B = \mu_0 \cdot \mu_r \cdot \frac{N\cdot I}{ℓ}$

$I = \dfrac{B \cdot ℓ}{\mu_0\cdot \mu_r \cdot N}$

$I=0,595 A$

$R=\frac{U}{I}$

$U=26,8V$

</p>

</p>

</details>

<details>

<summary> Lösung b) </summary>

Aus der Gleichung der magnetischen Flussdichte für eine lange Spule kann man entnehmen:

1. Die Stromstärke kann verdoppelt werden (entspricht einer Spannungsverdopplung, da I ~ U)

2. Die Windungszahl kann verdoppelt werden.

3. Die Länge der Spule kann halbiert werden.

4. In die Spule kann ein Stoff mit µ = 2 eingeführt werden. 

Bei jeder der 4 Möglichkeiten bleiben die anderen Größen konstant.

</details>

</p>

1. 3. LB S. 126 / 37 a)

<details style="margin-left:10%">

<summary> Lösung </summary>

Treten die Elektronen senkrecht zu den Feldlinien des homogenen Magnetfelds ein (Bild 1 und 2), so bewegen sie sich auf einer Kreisbahn. -> Kreisbewegung

Werden die Ladungsträger parallel zum Magnetfeld eingeschossen (Bild 3), dann ist die auf die Elektronen wirkende Lorentzkraft und somit die Ablenkung null. Die Bahnform ist eine Gerade. -> gleichförmige Bewegung

Treten die Elektronen schräg in das Magnetfeld ein (Bild 4), so bewegen sie sich auf einer spiralförmigen Bahn. Es liegt eine ungestörte Überlagerung einer gleichförmigen geradlinigen Bewegung und einer gleichförmigen Kreisbewegung vor.
</details>

#### 2. Aus Abi GK-2013

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

### Zur Erinnerung: Experimentvideo aus der letzten Stunde (bis 3:24 min)

!?[Fadenstrahlrohr](https://youtu.be/j5y64SPRnH0?si=MxXy0qlxifHUnRlz)


## 1.1. Der Millikan-Versuch

_Tafelbildvideo zum Millikan-Versuch:_

!?[Millikan-Experiment](https://www.youtube.com/watch?v=XMfYHag7Liw)

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Millikan](https://diversewolken.ddns.net/nextcloud/index.php/s/ocNCHdfqgfNNt44/download)

</details>

---

__Erklärung:__

Robert Millikan führte einen berühmten Versuch durch, um die Elementarladung $q_e$ zu bestimmen. Dabei wurden geladene Öltröpfchen in einem homogenen elektrischen Feld zwischen zwei Platten zum Schweben gebracht, indem sich die elektrische Kraft und die Gewichtskraft gegenseitig kompensieren. 

---

<p style="color:blue">

__1. Gleichung für Ladung ableiten:__ 

 - notieren Sie das genannte Kräftegleichgewicht als Gleichung

 - setzen Sie für beide Kräfte die gegebenen Formeln ein, notieren Sie für die elektrische Feldstärke die Formel im Plattenkondensator

 - stellen Sie die Gleichung nach der Ladung $q$ um

 - notieren Sie die Gleichung in Ihrem Hefter
</p>

---

<details>

<summary> __Lösung: Formel zur Bestimmung Ladung q des Öltröpfchens:__ </summary>

$$\boxed{q = m \cdot g \cdot \frac{d}{U}}$$

<p style="margin-left:10%">

$q$ ... Ladung des Öltröpfchens

$m$ ... Masse des Öltröpfchens

$U$ ... angelegte Spannung

$d$ ... Plattenabstand

</p>

</details>

---

<p style="color:blue">

__2. Berechnung der Ladung (+)__

Die Elementarladung wurde von Millikan bestimmt. Berechnen Sie die Ladung eines Öltröpfchens im Gleichgewicht, wenn die Masse $m = 2.5 \cdot 10^{-15} kg$ beträgt, Plattenabstand $d = 6 mm$ und die angelegte Spannung $U = 900 V$.

@rangeQuiz2($q$, 1.635e-19, $C$)

</p>

---

<p style="color:blue">

__3. Präzisierung des Experiments I (++)__

__Hintergrund:__ Tatsächlich konnte Milikan die Masse der Öltröpfchen nicht messen, da sie viel zu klein waren. Anstelle dessen versuchte er, den Durchmesser der Tröpfchen zu bestimmen und so mittels Kugelvolumen und der Dichte von Öl, die Masse der Öltröpfchen zu bestimmen. 

__Aufgabenstellung:__ Ermittln Sie für ein Tröpfchen, dass einen Durchmesser von 1,2µm besitzt und bei einer Spannung von 674 V (d=6mm) schwebt, die elektrische Ladung. Als Dichte kann $\rho_{Öl}=0,875 \frac{g}{cm^3}$ angenommen werden.

@rangeQuiz2($q$, 3.2e-19, $C$)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweise:__ </summary>

- ermitteln Sie aus der Formelsammlung die Formel für das Volumen einer Kugel 

- nutzen Sie den Durchmesser des Tröpfchens um dessen Volumen zu bestimmen 

- ermitteln Sie mit Hilfe von Volumen und Dichte die Masse des Tröpfchens

- berechnen Sie mit Hilfe von Masse, Spannung und Plattenabstand die Ladung

</details>

<details style="margin-left:10%">

<summary> __Lösungen:__ </summary>

$V=\frac{4}{3}\pi r^3$ 

@rangeQuiz2($V$, 9.05e-19 , $m^3$) 

@rangeQuiz2($m$,  7.972e-16 , $kg$)

Hinweis: $\rho_{Öl} = 0,875 \frac{g}{cm^3} = 875 \frac{kg}{m^3}$

@rangeQuiz2($q$, 6.914e-20, $C$)

</details>

---

<p style="color:blue">

__3. Simualtion des Experiments II (++)__

__Hintergrund:__ Wie man in der vorhigen Analyse sehen konnte, war es bei dem Versuch nicht sicher, dass das Öltröpfchen mit genau einer Elementarladung geladen war. Tatsächlich variierte die Anzahl an Elementarladungen von Tröpfchen zu Tröpfchen. Millikan konnte bei seiner Analyse allerdings zeigen, dass die Ladung der Tröpfchen keine beliebigen Werte annehmen konnte. 

__Aufgabenstellung:__ Nutzen Sie die Simulation auf LEIFI-Physik ([SIMULATION_MILIKAN](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/versuche/millikan-versuch-schwebemethode-simulation)). Bringen Sie mindestens fünf Tröpfchen nacheinander in einen Schwebezustand, notieren Sie Spannung und Tröpfchenradius und ermitteln Sie die zugehörigen Ladungen. Tragen Sie anschließend die Datenpunkte in ein Diagramm ein. 

![MILIKAN_FOTO](https://diversewolken.ddns.net/nextcloud/index.php/s/RgskbsAYNLX2ibX/download)<!-- style="max-width=500px" -->

</p>
