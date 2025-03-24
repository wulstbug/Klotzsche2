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


## 2.1. Der Millikan-Versuch

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

__Aufgabenstellung:__ Ermittln Sie für ein Tröpfchen, dass einen Durchmesser von 1,2µm besitzt und bei einer Spannung von 165 V (d=6mm) schwebt, die elektrische Ladung. Als Dichte kann $\rho_{Öl}=0,875 \frac{g}{cm^3}$ angenommen werden.

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

@rangeQuiz2($q$, 3.2e-19, $C$)

</details>

---

<p style="color:blue">

__3. Simualtion des Experiments II (++)__

__Hintergrund:__ Wie man in der vorhigen Analyse sehen konnte, war es bei dem Versuch nicht sicher, dass das Öltröpfchen mit genau einer Elementarladung geladen war. Tatsächlich variierte die Anzahl an Elementarladungen von Tröpfchen zu Tröpfchen. Millikan konnte bei seiner Analyse allerdings zeigen, dass die Ladung der Tröpfchen keine beliebigen Werte annehmen konnte. 

__Aufgabenstellung:__ Nutzen Sie die Simulation auf LEIFI-Physik ([SIMULATION_MILIKAN](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/versuche/millikan-versuch-schwebemethode-simulation)). Bringen Sie mindestens fünf Tröpfchen nacheinander in einen Schwebezustand, notieren Sie Spannung und Tröpfchenradius und ermitteln Sie die zugehörigen Ladungen. Tragen Sie anschließend die Datenpunkte in ein Diagramm ein. 

![MILIKAN_FOTO](https://diversewolken.ddns.net/nextcloud/index.php/s/RgskbsAYNLX2ibX/download)<!-- style="max-width=500px" -->

</p>

<details>

<summary> Ergebnis des Versuchs </summary>

> Die kleinste mögliche Ladung, die für das Experiment ermittelt werden konnte betrug $1,6\cdot10^{-19}C$. Alle höheren Ladungen sind immer Vielfache dieser @color(Elementarladung $e$, red)
>
> $$ \boxed{e = 1,602\cdot10^{-19}C}$$

</details>


## 2.2. Bewegung geladener Teilchen im elektrischen Feld

<p class="newspaper">

__Elektronenkanone__

![Elektronenkanone](https://diversewolken.ddns.net/nextcloud/index.php/s/cC5JWAYmimFKmrC/download)

_35 min_

<p class="cb">

__Ablenkröhre__

![Ablenkröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/HaNg8rpJnyZj7F5/download)

_35 min_

</p>

</p>

### 2.2.1 Beschleunigung im Längsfeld - ElLektronenkanone

@timer(35,00)

__Aufbau einer Elektronenkanone__

??[VirtuelleExperiment_Elektronenkanone_Aufbau](https://virtuelle-experimente.de/kanone/klassisch/aufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de, CC BY-NC-SA 3.0 DE")

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

3. 3. Löse das Quiz.

3. 4. Bearbeite die Rechenaufgaben. 

      __Aufgabe 1:__ Als __Partnerübung__, d.h. eine Person stellt die Frage und liest die Lösung, die andere Person beantwortet die Frage.

      __Aufgabe 2:__ Als __Einzelarbeit__ mit Lösungsüberprüfung und Diskussion des Lösungswegs in der Gruppe.

</p>

### 2.2.2 Ablenkung Querfeld - Ablenkröhre

@timer(35, 00)

__Aufbau einer Elektronen-Ablenkröhre__

??[VirtuelleExperiment_ElektronenAblenkrhre](https://virtuelle-experimente.de/e-feld/hypothesen/versuchsaufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de, CC BY-NC-SA 3.0 DE")

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

2. Wechsle zu den _Übungen_ (oberes Menü) und bearbeite:

2. 1. Übung Fachbegriffe

2. 2. _Optional:_ Übung Anschluss

2. 3. Mulitple Choice kurze Version

2. 4. Abituraufgaben

      - Aufgabe 2

      - Aufgabe 5 (a, b, d)

</p>

</p>


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

### Übungsaufgabe II

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

2. 2. Ermitteln Sie die Eintrittsgeschwindigkeit $v_0$, bei welcher die Elektronen genau die hinteren Rand der Platte erreichen. 


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

2. 7. *Ermitteln Sie minimale Eintrittsgeschwindigkeit der Elektronen in das magnetische Feld, damit Sie den Feldbereich wieder verlassen, ohne auf eine Kondensatorplatte zu treffen.<br>_Hinweis: Hier müssen zur Vollständigkeit zwei Fälle betrachtet werden._

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![262_Lsg_f](https://diversewolken.ddns.net/nextcloud/index.php/s/qNeT5R6rQDm5DQ7/download)

</details>