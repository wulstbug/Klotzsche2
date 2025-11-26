<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://static.wixstatic.com/media/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg

@style
.lia-effect__circle {
    display: none !important;
}
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 40px;
}
.flex-child,
.flex-child-1 { flex: 1; }
.flex-child-2 { flex: 2; }
.flex-child-3 { flex: 3; }
.flex-child-4 { flex: 4; }
.flex-child-5 { flex: 5; }
.flex-child-6 { flex: 6; }
.flex-child-7 { flex: 7; }
.flex-child-8 { flex: 8; }

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
<div style="float:left;margin-right:5px">
@0$\ $=$\ $ 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
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
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
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
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

@rangeQuiz0
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)
    input == 0
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

mode: presentation

-->

# LB 11 Einführung in die Quantenphysik 

![Schrödingers-Katze](https://static.wixstatic.com/media/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg)

## 11. 0. Einführende Überlegungen zur Quantenmechanik

1. Die Abgabe von Energie erfolgt immer in Energiepaketen (in __Quantisierter Form__).

2. Die Aufnahme von Strahlung erfolgt immer in Energiepaketen (in __Quantisierter Form__).

3. Das Licht hat Teilcheneigenschaften.

4. Teilchen haben Welleneigenschaften.

5. Die Genauigkeit der gleichzeitigen Messung von Impuls und Ort eines Teilchens ist begrenzt (__Unbestimmtheit__).

## 11. 1. Schrödingers Katze 

> <H4>Gedankenexperiment nach Erwin Schrödinger (1935)</H4>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![SchrödingersKatze](https://static.wixstatic.com/media/56b499_c7f1163b77fb4f1cb98a78361b977eda~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_c7f1163b77fb4f1cb98a78361b977eda~mv2.jpg "Quelle: https://www.sci-fakt.com/post/quantenphysik-schr%C3%B6dingers-katze-gedankenexperiment-in-3-schritten-einfach-erkl%C3%A4rt")

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

1. Eine (lebendige) Katze wird mit einer Giftampulle (verschlossen), einer geringen Menge radioaktiver Substanz, einem Geiger-Zählrohr und einem Hammer in eine Kiste gesteckt.

2. Die radioaktive Substanz sei so gewählt, dass die Wahrscheinlichkeit für einen radioaktiven Zerfall exakt genauso groß ist, wie die Wahrscheinlichkeit das nichts passiert.

3. Sobald die radioaktive Substanz zerfällt, registriert das der Detektor, der Hammer zerschlägt die Phiole und die Katze stirbt.

4. Die Kiste ist zu. Man hört nichts, riecht nichts, sieht nichts.

> @color(Ist die Katze nun lebendig oder tot?, blue)

</div>

</section>

> <H4>Quantenmechanische Deutung: So lange wir nicht nachgesehen (d.h. gemessen) haben, ist sie lebendig und tot gleichzeitig.</H4>

## 11. 2. Experiment: Der äußere lichtelektrische Effekt (Photoeffekt)

> <H4>Experiment nach Albert Einstein (1905)</H4>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Skizze-Photoeffekt](https://diversewolken.ddns.net/nextcloud/index.php/s/zL6DpdmEcFEiAJA/download)

[Simulation-Photoeffekt](https://phet.colorado.edu/sims/cheerpj/photoelectric/latest/photoelectric.html?simulation=photoelectric&locale=de)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__ 

 - Zwei Metallelektroden befinden sich in einer Vakuum-Röhre

 - Eine Elektrode wird mit monochromatischen (d.h. einfarbigem) Licht bestrahlt

__Beobachtung:__

1. Bestrahlt man die Elektrode mit Licht einer großen Wellenlänge, kann man zwischen den Elektroden keinen Strom messen, @color(egal wie hoch die Lichtintensität, red) (d.h. wie hell die Lampe) ist.

2. Verringert man hingegen die Wellenlänge (erhöht die Frequenz), so werden unterhalb einer bestimmten Wellenlänge @color(Elektronen aus dem Material emmitiert, red). Man kann einen Stromfluss messen.

3. Erhöht man jetzt die @color(Intensität, blue), so erhöht sich die @color(Anzahl der emmitierten Elektronen, blue).

4. Verringert man @color(die Wellenlänge, red) (erhöht @color(die Frequenz, red)) weiter, so erhöht sich die @color(kinetische Energie der Elektronen, red).

</div>

</section>



> __Schlussfolgerung:__

> 1. Ob überhaupt Elektronen aus dem Material herausgelöst werden, hängt nicht von der Lichtintensität ab, sondern von der Wellenlänge/Frequenz. Es existiert eine Grenzwellenlänge/Grenzfrequenz.

> 2. Da die Elektronen kinetische Energie erhalten, muss das @color(einfallende Licht Energie auf die Elektronen übertragen, red).




> 3. Da die Elektronen eine größere kinetische Energie erhalten, je kleiner die Wellenlänge ist, muss die @color(Energie des Lichts mit sinkender Wellenlänge/wachsender Frequenz steigen, red).

> 4. Nehmen wir an, dass @color(Energie in Paketen übertragen wird, red) (siehe Grundannahmen), trägt das Licht quantisierte Energiepakete (wir nennen sie Photonen), deren Energie von der Wellenlänge/Frequenz abhängt.

> @color(Wie ist der Zusammenhang von Wellenlänge/Frequenz und Energie?, blue)

## 11. 3. Die Gegenfeldmethode beim Photoeffekt

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Versuchsaufbau:__

![Gegenfeldmethode-Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/w3iQGHQEGejyTt8/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__

- eine Metallelektrode (Kathode) wird mit monochromatischem Licht beleuchtet

- werden Elektronen aus dem Metall herausgelöst, so erhalten sie eine kinetische Energie $E_{kin}$

- aufgrund der emitierten Elektronen kann man zwischen Kathode und Anode einen elektrischen Stromfluss $I$ beobachten

- legt man zwischen Kathode und Anode eine __Gegenspannung__ $U_g$ an, so werden die Elektronen durch $U_g$ abgebremst, sie erhalten durch die Spannung die kinetische Energie $U \cdot e$ ($e$ .. Elementarladung)

- wählt man $U_g$ gerade so groß, dass kein Strom mehr zwischen Kathode und Anode fließt, so entspricht die zugeführte Energie $U\cdot e$ gerade der kinetischen Energie der Elektronen

</div>

</section>

__Messwerte:__

| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $\mathrm{J}$ |
| 365 | 8.22 | | |
| 405 | 7.41 | | |
| 436 | 6.88 | | |
| 546 | 4.49 | | |
| 577 | 5.20 | | |

<p style="color:blue">
0. _Bereite die Tabelle vor. Ermittle bereits die zugehörigen Frequenzen._

1. _Ergänze die gemessenen Daten $U_g$ für die verschiedenen Wellenlängen und berechne $E_{kin}$._ 

2. _Zeichne ein Diagramm der $E_{kin}(f)$._

3. _Zeichne eine geeignete Ausgleichsgerade und ermittle den Anstieg $h = \frac{\Delta E_{kin}}{\Delta f}$._
</p>

## 11. 4. Energie, Masse und Impuls von Photonen

> Der äußere lichtelektrische Effekt legt nahe, dass das Licht auch Teilcheneigenschaften besitzt. 


> Wir nennen die Lichtteilchen @color(__Photonen__, blue). Jedes Photon trägt Energie mit sich, welche von seiner Frequenz bzw. Wellenlänge abhängt.


> __Die Energie __eines Photons
>
> $$ \boxed{E_{ph} = h \cdot f = \frac{h\cdot c}{\lambda}}$$


_Nutzt man die Äquivalenz aus Masse und Energie  $E = m \cdot c^2$ der speziellen Relativitätstheorie so beträgt:_


> __Die Masse__ eines Photons
>
> $$ \boxed{m_{ph} = \frac{E_{ph}}{c^2} = \frac{h \cdot f}{c^2} = \frac{h}{c\cdot \lambda}} $$


_Das bewegte massebehaftete Objekte einen Impuls $p = m \cdot v$ besitzen, können wir einen Photonenimpuls berechnen zu_


> __Der Impuls__ eines Photons
>
> $$ \boxed{p_{ph} = m_{ph} \cdot c = \frac{h \cdot f}{c}} $$


__Hinweis zur Einheit @color(Elektronenvolt $\mathrm{eV}$, red):__

> Für die Energie von Elementarteilchen (z.B. Elektronen) und Photonen wird häufig die Einheit $\mathrm{eV}$ (gesprochen _Elektronenvolt_) genutzt. 
>
> Ein $\mathrm{eV}$ entspricht genau der Energie, die ein Elektron erhält, wenn es mit einer Spannung von $1\,\mathrm{V}$ beschleunigt wird.
>
> $$ \boxed{1 \mathrm{eV} = 1\,\mathrm{V}\cdot e = 1,602\cdot10^{-19} J}$$


_Beispiel:_

Ein Photon von rotem Licht mit der Wellenlänge $\lambda = 630\,\mathrm{nm}$ besitzt eine Energie von

<p style='margin-left:10%'>

__In Joule__

@rangeQuiz2($E_{ph}$, 3.155e-19 , $\mathrm{J}$)

__bzw. in Elektronenvolt__

@rangeQuiz2($E_{ph}$, 1.97 , $eV$)

</p>



### Übungsaufgaben zum Photoeffekt

1. Kennzeichnen Sie wahre Aussagen, wenn der äußere lichtelektrische Effekt.

<p style="margin-left:5%">

[[x]] Je kurzwelliger das Licht, je besser werden Elektronen aus der Katode gelöst
[[ ]] Wird die Intensität des Lichts verstärkt, erhöht sich die Geschwindigkeit der herausgelösten Elektronen.
[[x]] Die Energie des Lichtes ist von der Frequenz abhängig.
[[ ]] Die Grenzfrequenz hängt vom Licht ab.
[[ ]] Das Plancksche Wirkungsquantum hängt vom verwendeten Katodenmaterial ab.

</p>

---

2. Eine Fotokathode (Austrittsarbeit $W_A=2,4\cdot10^{-19}\,\mathrm{J}$) wird mit Licht der Wellenlänge $\lambda = 500\,\mathrm{nm}$ bestrahlt.

2. 1. Ermitteln Sie die Gegenspannung $U_g$, bei welcher die Stromstärke gerade auf Null zurückgeht.

<p style='margin-left:10%'>

@rangeQuiz2($U_g$,0.99,$\mathrm{V}$)

</p>

<details style='margin-left:10%; color:blue'>

<summary> Lösung </summary>

![Lsg_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/s3aNGoxT4RWE2eT/download)

</details>

---

2. 2. Ermitteln Sie die Grenzfrequenz $f_g$ für dieses Kathodenmaterial.

<p style='margin-left:10%'>

@rangeQuiz2($f_g$, 3.62e14 , $\mathrm{Hz}$)

</p>

<details style='margin-left:10%; color:blue'>

<summary> Lösung </summary>

![Lsg_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/ySJTndor5tNotmc/download)

</details>

---

2. 3. Ermitteln Sie die Energie der Photonen in der Einheit $\mathrm{eV}$ für diese Grenzfrequenz und die Farbbezeichnung des Lichts.

<p style='margin-left:10%'>

@rangeQuiz2($E_{ph}$, 1.497 , $\mathrm{eV}$)

Farbbezeichnung: [[ Infrarot ]]

</p>

---

3. Albert Einstein bekam im Jahre 1921 den Physiknobelpreis für die Erklärung des Photoeffektes, bei dem unter bestimmten Bedingungen Elektronen aus einer Metalloberfläche austreten, wenn diese mit Licht bestrahlt wird. Mit Hilfe der Gegenspannungsmethode kann z.B. der Zusammenhang zwischen der Frequenz des eingestrahlten Lichtes und der maximalen Geschwindigkeit der ausgelösten Elektronen bestimmt werden. Welches Diagramm stellt den Zusammenhang zwischen den beiden Größen am besten dar? <br> ![Diagramme_Photoeffekt](https://physikaufgaben.de/bild/a1044_1.jpg/download)

<p style='margin-left:10%'>

[( )] a)
[( )] b)
[( )] c)
[(x)] d)

</p>

<details style='margin-left:10%;color:blue'>

<summary> Lösung </summary>

![Lsg_3](https://diversewolken.ddns.net/nextcloud/index.php/s/XwgEHRcwRNg2zp6/download)

</details>

---

4. ![Pitty_1115](https://diversewolken.ddns.net/nextcloud/index.php/s/rHpitZDaci8oTCm/download)Das Licht einer weißen Leuchtdiode (LED) wird untersucht. Das  Diagramm zeigt die Abhängigkeit der Strahlungsintensität von der Wellenlänge. (Quelle: http://ledmuseum.candlepower.us/led/specx02.htm) 

4. 1. Geben Sie die Wellenlängen der Photonen der beiden intensivsten Lichtanteile an.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_1$,455,$\mathrm{nm}$)

@rangeQuiz2($\lambda_2$,560,$\mathrm{nm}$)

</p>

---

4. 2. Ein schmales paralleles Bündel des LED-Lichtes durchläuft ein optisches Gitter. Es wird dadurch gebeugt und spektral zerlegt. Der Abstand Gitter-Schirm beträgt 2,0 m. Um gute Untersuchungsergebnisse zu erzielen, müssen die zwei lokalen Intensitätsmaxima in einem Spektrum 1. Ordnung mindestens den Abstand 5,0 cm voneinander haben. Berechnen sie, welche Gitterkonstante das genutzte Gitter höchstens haben darf.

<p style='margin-left:10%'>

@rangeQuiz2($g$,4.2e-6,$\mathrm{m}$)

</p>

---

<p style="margin-left:10%">

![Pitty1115_b](https://physikaufgaben.de/bild/a1115_2.jpg) Der Schirm wird entfernt. das gebeugte Licht fällt nun nach dem Durchlaufen einer schmalen Spaltblende auf die lichtempfindliche Schicht einer Fotozelle. Spaltblende und Fotozelle können parallel zum Gitter in y-Richtung bewegt werden. Die Abbildung zeigt das Prinzip.

</p>

---

4. 3. Untersuchen Sie rechnerisch, welche Ablösearbeit das Material der lichtempfindlichen Schicht der Fotozelle höchstens haben darf, damit Intensitätsverteilung mit der Fotozelle detektiert werden kann.

<p style='margin-left:10%'>

@rangeQuiz2($W_A$,1.65,$\mathrm{eV}$)

</p>

---

4. 4. Photonen einer bestimmten Wellenlänge des untersuchten Strahlungsspektrums lösen Elektronen mit der größten kinetischen Energie aus der lichtempfindlichen Schicht der Fotozelle heraus. Geben Sie diese Wellenlänge an und begründen Sie.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda$,400,$\mathrm{nm}$)

</p>


## 11. 5. Elektroneninterferenz am Doppelspalt

> Ein Elektronenstrahl wird auf einen Doppelspalt (oder ein Gitter) gerichtet, dahinter befindet sich ein Schirm, der auftrefende Elektronen sichtbar macht.

Im Jahr 1924 schlug der französche Physiker _Victor Louis de Broglie_ vor, jedem Teilchen eine Wellenlänge zuzuordnen, genannt __de Broglie Wellenlänge__

> Die **_de-Bloglie_ Wellenlänge**
>
> $$ \boxed{\lambda = \frac{h}{p} = \frac{h}{m \cdot v}}$$
>
> wobei $m$->Teilchenmasse, $v$->Bewegungsgeschwindigkeit und $p$->Teilchenimpuls



Für das Doppelspaltexperiment mit Elektronen (Experiment von Jönsson 1957) ergab sich auf dem Schirm ein ähnliches Bild wie bei Licht:

![Schema-Doppelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/F7g83jD4FLA9eZW/download)


### Aufgaben zum Welle-Teilchen-Dualismus

1. Duden S. 469 Aufgabe 2

---

2. Duden S. 469 Aufgabe 4

---

3. Duden S. 471 Aufgabe 19

---

4. Duden S. 471 Aufgabe 21

---

5. Duden S. 472 Aufgabe 22

---

> [AlleLösungen](https://diversewolken.ddns.net/nextcloud/index.php/s/MHP5NyL6LCajTay)

## 11. 6. Das Unschärfeprinzip / die Heißenberg'sche Unschärferelation

__Aufgabe:__ Bei einem Farbmonitor werden Elektronen mit $U=25\,\mathrm{kV}$ beschleunigt und treten durch eine Streifenmaske, deren Spaltöffnung $2\Delta x=0,25\,\mathrm{mm}$ betragen. 

<p style="margin-left:5%">

a) Vergleichen Sie die DE-BROGLIE-Wellenlänge der Elektronen mit der Spaltbreite. 

<details style='margin-left:10%'>

<summary> Lösung </summary>


$$E_{kin} = \frac{1}{2}\cdot m_e \cdot v^2 = U \cdot e = 25\,\mathrm{keV}$$

$$v = \sqrt{\dfrac{2\cdot U \cdot e}{m_e}}=9,377\,\mathrm{\frac{m}{s}}$$

$$ \lambda = \dfrac{h}{m_e \cdot v} = 7,76\cdot 10^{-12}m$$

=> Die Wellenlänge ist viel kleiner als die Spaltbreite.

</details>

b) Bewerten Sie die Unschärfe auf dem Leuchtschirm in $1\,\mathrm{cm}$ Abstand hinter der Streifenmaske.

<details style='margin-left:10%'>

<summary> Hinweis </summary>

Ermitteln Sie die Impulsunschärfe $\Delta p$ in x-Richtung, bei gegebener Ortsunschärfe $\Delta x$. Überprüfen Sie nun die Verbreiterung des Elektronenstrahls aufgrund Unschärfe $\Delta p$.

</details>

</p>


### Übungsaufgabe zu Elektronen als Quantenobjekte


Elektronen bewegen sich mit einer Geschwindigkeit von $v = 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$.

---

>a) Berechne den Impuls $p$ eines Elektrons.

<p style='margin-left:10%'>

@rangeQuiz2($p$, 7.38e-23, $\text{kg} \cdot \text{m} \cdot \text{s}^{-1}$)

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Der Impuls $p$ eines Teilchens wird durch die klassische Formel $p = m_e \cdot v$ berechnet.

Dabei ist $m_e$ die Ruhemasse des Elektrons.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Zur Berechnung wird die Beziehung $$p = m_e \cdot v$$ verwendet.
Mit $m_e \approx 9,109 \cdot 10^{-31} \, \text{kg}$ und $v = 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$ folgt:

$$p = 9,109 \cdot 10^{-31} \, \text{kg} \cdot 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$$

$$p \approx 7,378 \cdot 10^{-23} \, \text{kg} \cdot \text{m} \cdot \text{s}^{-1}$$

</details>

---

> b) Berechne die De Broglie-Wellenlänge $\lambda$ dieses Elektrons.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda$, 8.98e-12, $\text{m}$)

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Die De Broglie-Wellenlänge $\lambda$ eines Teilchens ist direkt mit seinem Impuls $p$ verknüpft [1, 2].

Nutze das Planck’sche Wirkungsquantum $h \approx 6,626 \cdot 10^{-34} \, \text{J} \cdot \text{s}$.
Die Beziehung lautet: $$\lambda = \frac{h}{p}$$

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die De Broglie-Wellenlänge wird berechnet mittels: $$ \lambda = \frac{h}{p} $$

Mit $h \approx 6,626 \cdot 10^{-34} \, \text{J} \cdot \text{s}$ und dem Impuls $p \approx 7,378 \cdot 10^{-23} \, \text{kg} \cdot \text{m} \cdot \text{s}^{-1}$ (aus Teilaufgabe a) folgt:

$$ \lambda = \frac{6,626 \cdot 10^{-34} \, \text{J} \cdot \text{s}}{7,378 \cdot 10^{-23} \, \text{kg} \cdot \text{m} \cdot \text{s}^{-1}} $$

$$ \lambda \approx 8,981 \cdot 10^{-12} \, \text{m} $$

</details>

---

> c) Ermitteln Sie die Spannung $U$, welche zur Beschleunigung der Elektronen benötigt wird.

<p style='margin-left:10%'>

@rangeQuiz2( $U$, 18653, $\text{V}$ )

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Die kinetische Energie $E_{kin} = \frac{1}{2} m_e v^2$, welche die Elektronen durch die Geschwindigkeit $v$ besitzen, muss gleich der elektrischen Energie $E_{el} = e \cdot U$ sein, die durch die Beschleunigungsspannung $U$ gewonnen wurde [1].

Nutze die Gleichung: $$E_{el} = E_{kin} \Rightarrow e \cdot U = \frac{1}{2} m_e v^2$$

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Zur Berechnung wird die Beziehung $U = \frac{m_e v^2}{2 \cdot e}$ verwendet [1].

Dabei wird die Geschwindigkeit $v = 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$ (aus den vorherigen Teilaufgaben), die Elektronenmasse $m_e \approx 9,109 \cdot 10^{-31} \, \text{kg}$ und die Elementarladung $e \approx 1,602 \cdot 10^{-19} \, \text{C}$ eingesetzt.

$$U = \frac{9,109 \cdot 10^{-31} \, \text{kg} \cdot (8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1})^2}{2 \cdot 1,602 \cdot 10^{-19} \, \text{C}}$$

$$\mathbf{U \approx 18653 \, \text{V}}$$

</details>

---

> d) Die Elektronen werden nun durch ein atomares Gitter mit der Gitterkonstanten $b = 10 \, \text{pm}$ geschickt. Ermitteln Sie den Abstand $s_k$ des ersten ($k=1$) und des zweiten ($k=2$) Maximums vom Maximum Nullter Ordnung. <br> Der Abstand des Schirms vom Gitter beträgt 6 cm.

<p style='margin-left:10%'>

@rangeQuiz2( $a_1$, 0.1225, $\text{m}$ )

</p>


<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Nutzen Sie die allgemeine Interferenzgleichung für Maxima: $$b \cdot \sin(\alpha_k) = k \cdot \lambda$$

Überprüfen Sie zunächst, ob $\frac{k \cdot \lambda}{b} \le 1$ gilt. Ist dies der Fall, existiert das Maximum der Ordnung $k$.

Da die Beugungswinkel bei Elektronen oft groß sind, darf die Kleinwinkelnäherung $\sin(\alpha_k) \approx \tan(\alpha_k)$ nicht ohne Prüfung angewendet werden. Nutzen Sie allgemein den Zusammenhang: $$a_k = e \cdot \tan(\alpha_k)$$

Die De Broglie-Wellenlänge $\lambda$ beträgt $\lambda \approx 8,981 \cdot 10^{-12} \, \text{m}$ und die Gitterkonstante $b = 10 \cdot 10^{-12} \, \text{m}$.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

**1. Prüfung der Existenz der Maxima:**

Die Bedingung für Maxima ist: $$ \sin(\alpha_k) = \frac{k \cdot \lambda}{b} $$

Für das Maximum 1. Ordnung ($k=1$):
$$ \sin(\alpha_1) = \frac{1 \cdot 8,981 \cdot 10^{-12} \, \text{m}}{10 \cdot 10^{-12} \, \text{m}} = 0,8981 $$
Da $0,8981 \le 1$ ist, existiert das erste Maximum.

Für das Maximum 2. Ordnung ($k=2$):
$$ \sin(\alpha_2) = \frac{2 \cdot 8,981 \cdot 10^{-12} \, \text{m}}{10 \cdot 10^{-12} \, \text{m}} = 1,7962 $$
Da $1,7962 > 1$ ist, ist die Gleichung **physikalisch nicht lösbar**. Das zweite Maximum existiert nicht.

**2. Berechnung des Abstands $a_1$ (1. Maximum):**

Zuerst wird der Beugungswinkel $\alpha_1$ berechnet:
$$\alpha_1 = \arcsin(0,8981) \approx 63,9^\circ$$

Nun wird der Abstand $s_1$ vom Zentralmaximum ermittelt (mit $e = 0,06 \, \text{m}$):
$$ a_1 = e \cdot \tan(\alpha_1) $$
$$ a_1 = 0,06 \, \text{m} \cdot \tan(63,9^\circ) \approx 0,06 \, \text{m} \cdot 2,0416 $$
$$\mathbf{a_1 \approx 0,123 \, \text{m}}$$

**Ergebnis:** Der Abstand des ersten Maximums beträgt $0,123 \, \text{m}$. Das zweite Maximum existiert nicht.

</details>


## 11. 7. Einzelphotoneninterferenz am Doppelspalt

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


Reduziert man bei einem Doppelspalt-Experiment die Lichtintensität, so lässt sich nachweisen, dass sich im Versuchsaufbau zu einem Zeitpunkt lediglich ein Photon befindet.

<p style="color:blue">

Bestimmen Sie für einen Laser der Wellenlänge 650 nm die maximale Lichtleistung, damit sich in der Aperatur der Länge ℓ lediglich 1 Photon befindet.

@rangeQuiz2($P_L$, 9.18e-11, $\mathrm{W}$)

<details style='margin-left:10%'>

<summary> Lösungshinweis </summary>

Bestimmen Sie die Energie eines Photons. Ermitteln Sie Flugzeit eines Photons. Passen Sie nun die Lichtleistung so an, dass die Zeit, zwischen zwei ausgesandten Photonen größer ist als die Flugzeit.

</details>

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/bgosKyRYWKax9zX/download)

</div>

</section>

__Beobachtungen auf dem Schirm:__

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

Für dieses Experiment wird ein photographischer Schirm genutzt. Jedes auftreffende Photon hinterlässt einen hellen Fleck. Wird das Experiment mit wenigen Photonen durchgeführt (a), so ergibt sich eine scheinbar zufällige Verteilung der Photonen. 

> Der Ort des Auftreffens ist für das einzelne Photon @color(nicht vorhersagbar, red) (@color(nicht determiniert, red)).

Eine größere Anzahl von Photonen (b+c) hinterlässt auf dem Schirm ein Bild, welches einem Interferenzmuster (d) ähnelt

> Die @color(Zufallsverteilung, red) für eine große Anzahl an Photonen ist @color(determiniert, red) (@color(vorherbestimmt, red)).

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Einzelphotoneninterferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/Hpjzn7WP4Eb9eWA/download)

</div>

</section>


### Übungsaufgabe Einzelelektroneninterferenz

In einem Experiment von Jöhnson 1950 wurde ein Elektronenstrahl auf ein Beugungsgitter geschickt und die Auftreffpunkte der Elektronen wurden anschließend auf einem Schirm sichtbar gemacht. Dabei ergab sich ein sehr ähnliches Bild, wie es bei den Photonen zu beobachten ist.

Mit einer Elektronenkanone werden Elektronen mit einer Spannung von 5 kV beschleunigt und auf ein Gitter gelenkt. Ermitteln Sie den maximalen Stromfluss $I_{max}$, bei welchem sich immer nur genau ein Elektron in der Aperatur der Länge $ℓ=1\,\mathrm{m}$ befindet.

<p style='margin-left:10%'>


@rangeQuiz2($I_{max}$, 6.718e-12 , $\mathrm{A}$)

</p>

<details style='margin-left:10%;color:blue'>

<summary> Lösungshinweis </summary>

Ermitteln Sie zunächst die Geschwindigkeit der Elektronen. Gehen Sie anschließend ähnlich vor, wie bei den Photonen. Nutze Sie die Definition der Stromstärke.

@rangeQuiz2($v$,4.19,$\mathrm{\frac{m}{s}}$)

</details>

<details style='margin-left:10%;color:blue'>

<summary> Lösung </summary>

Die kinetische Energie $E_{kin} = \frac{1}{2} m_e v^2$, welche die Elektronen durch die Geschwindigkeit $v$ besitzen, muss gleich der elektrischen Energie $E_{el} = e \cdot U$ sein, die durch die Beschleunigungsspannung $U$ gewonnen wurde.

Es folgt:

$$ \frac{1}{2} m_e v^2 = e \cdot U $$

für die Geschwindigkeit der Elektronen:

$$ v = \sqrt{2\cdot e \cdot U}{m_e} = 4,19 \cdot 10^{7} \,\mathrm{\frac{m}{s}} $$

Die Flugzeit der Elektronen beträgt:

$$ t = \frac{ℓ}{v} = 2,38\cdot 10^{-8} \,\mathrm{s}$$

Die maximale Stromstärke ergibt sich zu

$$ I = \frac{Q}{t} = \frac{e}{t} = 6,718 \cdot 10^{-12}\,\mathrm{A}$$

</details>
