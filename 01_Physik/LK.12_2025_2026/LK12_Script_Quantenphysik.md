<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

language: de

logo: https://www.sciencedaily.com/images/1920/Quantum-Clock.webp

@style
.lia-effect__circle {
    display: none !important;
} 
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 20px;
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

@media (max-width: 500px) {
    .flex-child,
    .flex-child-1,
    .flex-child-2,
    .flex-child-3,
    .flex-child-4,
    .flex-child-5,
    .flex-child-6,
    .flex-child-7,
    .flex-child-8 {
        flex: 100%; /* Makes the child divs take up the full width on slim devices */
        margin-right: 0; /* Removes the right margin */
    }
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
    display: block;
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


# LB 11 - Einführung in die Quantenphysik

![Schrödingers-Katze](https://static.wixstatic.com/media/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg)

## Lesch's Kosmos - Einführung in die Quantenphysik

!?[Wie funktioniert Quantenmechanik? Quantenphysik erklärt Teil 1 | Harald Lesch | Terra X Lesch & Co](https://www.youtube.com/watch?v=cWf1OUVUObw)

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

{{1}}
************
1. Eine (lebendige) Katze wird mit einer Giftampulle (verschlossen), einer geringen Menge radioaktiver Substanz, einem Geiger-Zählrohr und einem Hammer in eine Kiste gesteckt.
************

{{2}}
************
2. Die radioaktive Substanz sei so gewählt, dass die Wahrscheinlichkeit für einen radioaktiven Zerfall exakt genauso groß ist, wie die Wahrscheinlichkeit das nichts passiert.
************

{{3}}
************
3. Sobald die radioaktive Substanz zerfällt, registriert das der Detektor, der Hammer zerschlägt die Phiole und die Katze stirbt.
************

{{4}}
************
4. Die Kiste ist zu. Man hört nichts, riecht nichts, sieht nichts.
************

{{5}}
************
> @color(Ist die Katze nun lebendig oder tot?, blue)
************

</div>

</section>

{{6}}
************
> <H4>Quantenmechanische Deutung: So lange wir nicht nachgesehen (d.h. gemessen) haben, ist sie lebendig und tot gleichzeitig.</H4>
************

## 11. 2. Experiment: Der äußere lichtelektrische Effekt (Photoeffekt)

> <H4>Experiment nach Albert Einstein (1905)</H4>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

{{1-8}}
***********
??[Simulation-Photoeffekt](https://phet.colorado.edu/sims/cheerpj/photoelectric/latest/photoelectric.html?simulation=photoelectric&locale=de)
***********

{{8}}
***********
![Skizze-Photoeffekt](https://diversewolken.ddns.net/nextcloud/index.php/s/zL6DpdmEcFEiAJA/download)
***********

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

{{1}}
***********
__Beschreibung:__ 

{{2}}
*********
 - Zwei Metallelektroden befinden sich in einer Vakuum-Röhre

 - Eine Elektrode wird mit monochromatischen (d.h. einfarbigem) Licht bestrahlt
 *********
***********

{{3}}
*********
 __Beobachtung:__

 1. Bestrahlt man die Elektrode mit Licht einer großen Wellenlänge, kann man zwischen den Elektroden keinen Strom messen, @color(egal wie hoch die Lichtintensität, red) (d.h. wie hell die Lampe) ist.
*********

{{4}}
*********
 2. Verringert man hingegen die Wellenlänge (erhöht die Frequenz), so werden unterhalb einer bestimmten Wellenlänge @color(Elektronen aus dem Material emmitiert, red). Man kann einen Stromfluss messen.
*********

{{5}} 
*********
 3. Erhöht man jetzt die @color(Intensität, blue), so erhöht sich die @color(Anzahl der emmitierten Elektronen, blue).
*********

{{6}}
*********
 4. Verringert man @color(die Wellenlänge, red) (erhöht @color(die Frequenz, red)) weiter, so erhöht sich die @color(kinetische Energie der Elektronen, red).
*********

</div>

</section>

{{7}}
*********
> __Schlussfolgerung:__

{{8}}
*********
> 1. Ob überhaupt Elektronen aus dem Material herausgelöst werden, hängt nicht von der Lichtintensität ab, sondern von der Wellenlänge/Frequenz. Es existiert eine Grenzwellenlänge/Grenzfrequenz.
*********

{{9}}
*********
> 2. Da die Elektronen kinetische Energie erhalten, muss das @color(einfallende Licht Energie auf die Elektronen übertragen, red).
*********

{{10}}
*********
> 3. Da die Elektronen eine größere kinetische Energie erhalten, je kleiner die Wellenlänge ist, muss die @color(Energie des Lichts mit sinkender Wellenlänge/wachsender Frequenz steigen, red).
*********

{{11}}
*********
> 4. Nehmen wir an, dass @color(Energie in Paketen übertragen wird, red) (siehe Grundannahmen), trägt das Licht quantisierte Energiepakete (wir nennen sie Photonen), deren Energie von der Wellenlänge/Frequenz abhängt.
*********

{{12}}
*********
> @color(Wie ist der Zusammenhang von Wellenlänge/Frequenz und Energie?, blue)
************

*********

## 11. 3. Die Gegenfeldmethode beim Photoeffekt

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Versuchsaufbau:__

![Gegenfeldmethode-Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/w3iQGHQEGejyTt8/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__


{{1}}
**********
- eine Metallelektrode (Kathode) wird mit monochromatischem Licht beleuchtet
**********

{{2}}
**********
- werden Elektronen aus dem Metall herausgelöst, so erhalten sie eine kinetische Energie $E_{kin}$
**********

{{3}}
**********
- aufgrund der emitierten Elektronen kann man zwischen Kathode und Anode einen elektrischen Stromfluss $I$ beobachten
**********

{{4}}
**********
- legt man zwischen Kathode und Anode eine __Gegenspannung__ $U_g$ an, so werden die Elektronen durch $U_g$ abgebremst, sie erhalten durch die Spannung die kinetische Energie $U_g \cdot e$ ($e$ .. Elementarladung)
**********

{{5}}
**********
- wählt man $U_g$ gerade so groß, dass kein Strom mehr zwischen Kathode und Anode fließt, so entspricht die zugeführte Energie $U_g \cdot e$ gerade der maximalen kinetischen Energie der Elektronen
**********

</div>

</section>

{{6-7}}
**********
__Messwerte:__


| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $\mathrm{J}$ |
| 365 | | | |
| 405 | | | |
| 436 | | | |
| 546 | | | |
| 577 | | | |

@color(_Bereite die Tabelle vor. Ermittle bereits die zugehörigen Frequenzen._, blue)
**********

{{7}}
****************
__Messwerte:__

| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $\mathrm{J}$ |
| 365 | 8.22 | | |
| 405 | 7.41 | | |
| 436 | 6.88 | | |
| 546 | 5.50 | | |
| 577 | 5.20 | | |

<p style="color:blue">

1. _Ergänze die gemessenen Daten $U_g$ für die verschiedenen Wellenlängen und berechne $E_{kin}$._ 

2. _Zeichne ein Diagramm der $E_{kin}(f)$._

3. _Zeichne eine geeignete Ausgleichsgerade und ermittle den Anstieg $h = \frac{\Delta E_{kin}}{\Delta f}$._
</p>
****************

{{8}}
****************
![TB_Diagramm-Planck](https://diversewolken.ddns.net/nextcloud/index.php/s/zaKaAjcBMaNcdnr/download)
****************

{{9}}
****************
Das __Plancksche Wirkungsquantum__ oder auch __Planck-Konstante__ $h$ ist eine fundamentale Naturkonstante. Sie hat den Wert: $$ \boxed{h = 6,626\cdot10^{-34}\,\mathrm{J\cdot s}} $$
****************

{{10}}
****************
> Die Energiebilanz beim äußeren Lichtelektrischen Effekt lautet:
>
> $$ h\cdot f = W_A + E_{kin} $$
>
> wobei:
>
> $\hspace{1cm} f$ .. Frequenz des Lichts
>
> $\hspace{1cm} W_A$ .. Austrittsarbeit (Auslösearbeit) des Kathodenmaterials (vlg. FS S. )
>
> $\hspace{1cm} E_{kin}$ .. kinetische Energie der Elektronen
****************

## 11. 4. Energie, Masse und Impuls von Photonen

{{1}}
*********
> Der äußere lichtelektrische Effekt legt nahe, dass das Licht auch Teilcheneigenschaften besitzt. 
*********

{{2}}
*********
> Wir nennen die Lichtteilchen @color(__Photonen__, blue). Jedes Photon trägt Energie mit sich, welche von seiner Frequenz bzw. Wellenlänge abhängt.
*********

{{3}}
*********
> __Die Energie __eines Photons
>
> $$ \boxed{E_{ph} = h \cdot f = \frac{h\cdot c}{\lambda}}$$
*********

{{4}}
*********
_Nutzt man die Äquivalenz aus Masse und Energie  $E = m \cdot c^2$ der speziellen Relativitätstheorie so beträgt:_
*********

{{5}}
*********
> __Die Masse__ eines Photons
>
> $$ \boxed{m_{ph} = \frac{E_{ph}}{c^2} = \frac{h \cdot f}{c^2} = \frac{h}{c\cdot \lambda}} $$
*********

{{6}}
*********
_Das bewegte massebehaftete Objekte einen Impuls $p = m \cdot v$ besitzen, können wir einen Photonenimpuls berechnen zu_
*********

{{7}}
*********
> __Der Impuls__ eines Photons
>
> $$ \boxed{p_{ph} = m_{ph} \cdot c = \frac{h \cdot f}{c}} $$
*********

{{8}}
*********
__Hinweis zur Einheit @color(Elektronenvolt $\mathrm{eV}$, red):__

> Für die Energie von Elementarteilchen (z.B. Elektronen) und Photonen wird häufig die Einheit $\mathrm{eV}$ (gesprochen _Elektronenvolt_) genutzt. 
>
> Ein $\mathrm{eV}$ entspricht genau der Energie, die ein Elektron erhält, wenn es mit einer Spannung von $1\,\mathrm{V}$ beschleunigt wird.
>
> $$ \boxed{1 \mathrm{eV} = 1\,\mathrm{V}\cdot e = 1,602\cdot10^{-19} J}$$
*********

{{9}}
*********
_Beispiel:_

Ein Photon von rotem Licht mit der Wellenlänge $\lambda = 630\,\mathrm{nm}$ besitzt eine Energie von

<p style='margin-left:10%'>

__In Joule__

@rangeQuiz2($E_{ph}$, 3.155e-19 , $\mathrm{J}$)

__bzw. in Elektronenvolt__

@rangeQuiz2($E_{ph}$, 1.97 , $eV$)

</p>

*********

### Übungsaufgaben zum Photoeffekt

1. Kennzeichnen Sie wahre Aussagen zum äußeren lichtelektrischen Effekt.

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

### Welle -> Teilchen , Teilchen -> Welle

> [LESCH-Quantenphysik-Teilchenwellen](https://youtu.be/cWf1OUVUObw?t=493)

## 11. 5. Elektroneninterferenz am Doppelspalt

> Ein Elektronenstrahl wird auf einen Doppelspalt (oder ein Gitter) gerichtet, dahinter befindet sich ein Schirm, der auftrefende Elektronen sichtbar macht. ([Anschauung](https://youtu.be/ZdO4ERBrgnw?t=225))

{{1}}
*******
[Erklärungsvideo](https://youtu.be/M8MuyfjtUFU?t=39), [Anschauungsvideo](https://youtu.be/3ohjOltaO6Y?t=127)
*******

{{2}}
*******
Im Jahr 1924 schlug der französche Physiker _Victor Louis de Broglie_ vor, jedem Teilchen eine Wellenlänge zuzuordnen, genannt __de Broglie Wellenlänge__

> Die **_de-Bloglie_ Wellenlänge**
>
> $$ \boxed{\lambda = \frac{h}{p} = \frac{h}{m \cdot v}}$$
>
> wobei $m$->Teilchenmasse, $v$->Bewegungsgeschwindigkeit und $p$->Teilchenimpuls
*******

{{3}}
*******
Für das Doppelspaltexperiment mit Elektronen (Experiment von Jönsson 1957) ergab sich auf dem Schirm ein ähnliches Bild wie bei Licht:

![Schema-Doppelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/F7g83jD4FLA9eZW/download)
*******

### Aufgaben zum Welle-Teilchen-Dualismus

1. Duden S. 469 Aufgabe 2

<p style='margin-left:10%'>

@rangeQuiz2(N,5,.)

</p>

---

2. Duden S. 469 Aufgabe 4

---

3. Duden S. 471 Aufgabe 19

---

4. Duden S. 471 Aufgabe 21

---

5. Duden S. 472 Aufgabe 22

---

[AlleLösungen](https://diversewolken.ddns.net/nextcloud/index.php/s/MHP5NyL6LCajTay)

### Interferenz mit Fullerene Molekülen

{{1}}
**************
<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Informationen aus dem Text:__ 

- $C_{60}$-Molekül

- Temperatur Ofen $T=900\,\mathrm{K}$

- Geschwindigkeit $v=200\,\mathrm{\frac{m}{s}}$

- Abstand Ofen-Gitter $l = 1,2\,\mathrm{m}$

- Spaltbreite $b = 50\,\mathrm{nm}$

- Gitterkonstante $g = 100\,\mathrm{nm}$

- Abstand Gitter-Detektor $e=1,25\,\mathrm{m}$

- Ortsauflösung $\Delta x = 5 \, \mathrm{\mu m}$

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Diagramm:__

![Diagramm_Fullerene](https://diversewolken.ddns.net/nextcloud/index.php/s/dgqp4DaR7L6NDdn/download)

</div>

</section>

---
**************


{{2}}
**************
> __Aufgabe a)__ Berechnen Sie mithilfe der Daten, die in Text und Diagramm gegeben sind, so genau wie möglich die DE-BROGLIE-Wellenlänge und die Masse der verwendeten Fulleren Moleküle.

---
**************

{{3}}
**************
<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Fullerene Molkekül:__

{{4}}
**************
![Fullerene-Molekül](https://diversewolken.ddns.net/nextcloud/index.php/s/yznFrwgRJxpr444/download)<!-- style="max-width:200px"-->
**************
</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

__Versuchsaufbau:__

{{5}}
**************
![Versuchsaufbau2](https://diversewolken.ddns.net/nextcloud/index.php/s/Kyqmij9z2sraH36/download)
**************

</div>

</section>

---
**************

{{6}}
**************

@color(__Berechnung der Wellenlänge:__, blue)

<br>

<br>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__DE-BROGLIE Wellenlänge__

$ \boxed{\lambda = \frac{h}{p} = \frac{h}{m_{C_{60}} \cdot v}}$

{{7}}
**************
__Problem:__ Wir kennen die Masse der Moleküle nicht. 

__Hinweis:__ $m_{C_{60}}=60\cdot m_C$ ist nicht zulässig, aufgrund des möglichen Massendefektes.
**************

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{8}}
**************
__Berechnung der Wellenlänge aus dem Interferenzmuster:__

$ \boxed{ \sin(\alpha) = \dfrac{\purple{k\cdot\lambda}}{\blue{g}}  } \hspace{.5cm} \boxed{\tan(\alpha) = \blue{\dfrac{a}{e}}}$

__Problem:__ Wir kennen das $a$ noch nicht. Können wir aber ermitteln.
**************

{{10}}
**************
__Berechnung:__ 

$ \alpha = tan^{-1}\Big(\dfrac{a}{e}\Big) = 0,00138^\circ $

=> __Kleinwinkelnäherung__ $\dfrac{\lambda}{g} = \dfrac{a}{e}$
**************

{{11}}
**************
=> $ \underline{\lambda = 2,4\cdot 10^{-12}\,\mathrm{m}}$
**************
</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{9}}
**************
![DiagrammAnalysiert](https://diversewolken.ddns.net/nextcloud/index.php/s/2sPidXRFZmp3F9y/download)

$ \red{a_1 \approx 30\,\mathrm{µm} }$
**************
</div>

</section>

---
**************

{{11}}
**************
@color(Berechnung der Masse, blue)

<br> <br>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

$ \boxed{\lambda = \dfrac{h}{p} = \dfrac{h}{m_{C_{60}} \cdot v}}$

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

$m_{C_{60}} = \dfrac{h}{\lambda \cdot v} $

$\underline{m_{C_{60}} = 1,38\cdot 10^{-24}\,\mathrm{kg}}$

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">



</div>

</section>

---
**************


{{12}}
**************
> __Aufgabe b)__ Zeigen Sie, dass mit der Anordnung die Maxima 2. Ordnung nicht beobachtet werden können.

<br>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{13}}
**************
__Ansatz:__ Wenn die Gitterkonstante $g$ kleiner ist, als der notwendige Gangunterschied $\Delta s$, so kann keine konstruktive Interferenz entstehen.
**************
</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{14}}
**************
__Gangunterschied:__ Für ein Maximum zweiter Ordnung ist der Gangunterschied $\Delta s = 2 \cdot \lambda = 4,8\cdot\mathrm{10^{-12}}\,\mathrm{m}$
**************

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{15}}
**************
__Analyse:__ Gitterkonstante $g=100\cdot 10^{-9}\mathrm{m}$ ist deutlich größer als $\Delta s = 2\cdot\lambda$, somit wäre das kein Hinderungsgrund.
**************

</div>

{{16}}
**************
__Lösung:__ Da aufgrund der Einzelspalte ebenfalls Interferenz auftritt und hier diese destruktive Interferenz genau bei $$\sin\alpha=\dfrac{\lambda}{b}=\dfrac{\lambda}{\frac{g}{2}} = \dfrac{2\cdot\lambda}{g}$$ auftritt, heben sich konstruktive Interferenz des Gitters und destruktive Interferenz des Einzelspaltes gegenseitig auf.
**************

</section>

---
**************

{{17}}
**************
> __Aufgabe c)__ Inwiefern weicht die Kurve von der theoretisch nach dem Wellenmodell erwarteten Intensitätskurve eines Gitters ab und wie kann man die beobachtete Abweichung durch die Geschwindigkeitsverteilung der Fullerene erklären.
**************

{{18}}
**************
Da die Fullerene nicht alle dieselbe Geschwindigkeit besitzen, sondern eine Verteilung der Geschwindigkeit der Moleküle vorliegt, ist auch die Wellenlänge der Moleküle nach der DE-BROGLIE-Gleichung $$ \lambda  = \dfrac{h}{m_{C_{60}} \cdot v} $$ nicht für jedes Molekül identisch und somit treten die Interferenz-Maxima für die Moleküle nicht an genau einem Ort ($x$), sondern an leicht variierenden Abständen vom Maximum auf. Eine weitere Rolle könnte die Ortsauflösung des Detektors spielen.
**************

## Was bisher geschah

!?[LESCH-Quantenmechanik-ZurTheorie](https://youtu.be/oh-dIbiHs48?si=aqqhkBKnZa7Afqfc)



## 11. 6. Das Unschärfeprinzip / die Heißenberg'sche Unschärferelation

> Bei einer __Messung__ von Ort ($x$) und Impuls $p$ eines quantenmechanischen Teilchens, können beide Größen nicht __gleichzeitig__ mit einer beliebigen Genauigkeit $\Delta x$ bzw. $\Delta p$ ermittelt werden. Die maximale Beobachtungsgenauigkeit beträgt: $$ \boxed{\Delta x \cdot \Delta p \geq \dfrac{h}{4\pi}} $$ Hierbei ist $\Delta x$ die __Ortsunschärfe__ und $\Delta p$ die __Impulsunschärfe__.
>
> Dieselbe gleichzeitige Unbestimmtheit ergibt sich bei einer Messung von _Energie_ und _Zeit_ als $$ \boxed{\Delta E \cdot \Delta t \geq \dfrac{h}{4\pi}}$$ Hierbei ist $\Delta E$ die Energieunschärfe und $\Delta t$ die Zeitunschärfe.

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