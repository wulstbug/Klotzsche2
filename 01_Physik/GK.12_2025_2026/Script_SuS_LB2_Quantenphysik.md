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

# LB VII Einführung in die Quantenphysik 

![Schrödingers-Katze](https://static.wixstatic.com/media/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg)

## 7. 0. Einführende Überlegungen zur Quantenmechanik

1. Die Abgabe von Energie erfolgt immer in Energiepaketen (in __Quantisierter Form__).

2. Die Aufnahme von Strahlung erfolgt immer in Energiepaketen (in __Quantisierter Form__).

3. Das Licht hat Teilcheneigenschaften.

4. Teilchen haben Welleneigenschaften.

5. Die Genauigkeit der gleichzeitigen Messung von Impuls und Ort eines Teilchens ist begrenzt (__Unbestimmtheit__).

## 7. 1. Schrödingers Katze 

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

## 7. 2. Experiment: Der äußere lichtelektrische Effekt (Photoeffekt)

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


## 7. 3. Die Gegenfeldmethode beim Photoeffekt

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Versuchsaufbau:__

![Gegenfeldmethode-Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/w3iQGHQEGejyTt8/download)

</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__

- eine Metallelektrode (Kathode) wird mit monochromatischem Licht beleuchtet

- werden Elektronen aus dem Metall herausgelöst, so erhalten sie eine kinetische Energie $E_{kin}$

- aufgrund der emitierten Elektronen kann man zwischen Kathode und Anode einen elektrischen Stromfluss $I$ beobachten

- legt man zwischen Kathode und Anode eine __Gegenspannung__ $U_g$ an, so werden die Elektronen durch $U_g$ abgebremst, sie erhalten durch die Spannung die kinetische Energie $U \cdot e$ ($e$ .. Elementarladung)

- wählt man $U_g$ gerade so groß, dass kein Strom mehr zwischen Kathode und Anode fließt, so entspricht die zugeführte Energie $U\cdot e$ gerade der kinetischen Energie der Elektronen

</div>

</section>


<p style="color:blue">

0. Übernimm den Versuchsaufbau und die Beschreibung in deinen Hefter.

1. Ermittle die Gegenspannung für die Natrium(engl. Sodium)-Elektrode bei der Bestrahlung mit Licht der Wellenlängen $425\,\mathrm{nm}$, $375\,\mathrm{nm}$ und $325\,\mathrm{nm}$. Nutze dafür die folgende Simulation: [Gegenfeldmethode-Simulation](https://phet.colorado.edu/sims/cheerpj/photoelectric/latest/photoelectric.html?simulation=photoelectric)

<p style='margin-left:10%'>

@rangeQuiz20($425\mathrm{nm}:U_g$,0.6,$\mathrm{V}$)

@rangeQuiz20($375\mathrm{nm}:U_g$,1.0,$\mathrm{V}$)

@rangeQuiz20($325\mathrm{nm}:U_g$,1.5,$\mathrm{V}$)

</p>

---

2. Ergänze die folgenden Daten $U_g$ für die verschiedenen Wellenlängen und berechne f in $10^{4}\,\mathrm{Hz}$ und $E_{kin}$ in J (nicht wie der Tabelle eV). 

<details style='margin-left:10%'>

<summary> __Messwerte für Natrium und Calcium:__ </summary>

![Messwerte](https://diversewolken.ddns.net/nextcloud/index.php/s/YqabxD3j8Jk8exe/download)

</details>

---

3. Zeichne ein Diagramm der $E_{kin}(f)$. Auf der y-Achse trage die $E_{kin}$ in der Einheit $10^{-19}\,\mathrm{J}$ ein (Bereich: -3 bis +3). Auf der x-Achse trage die Frequenz in der Einheit $10^{14}\,\mathrm{Hz}$ ein (Bereich: 0-10).

---

4. Zeichne eine geeignete Ausgleichsgerade und ermittle den Anstieg $h = \frac{\Delta E_{kin}}{\Delta f}$.
</p>


<details style='margin-left:10%'>

<summary> Lösung </summary>

![Diagramm_Gegenfeldmethode](https://diversewolken.ddns.net/nextcloud/index.php/s/Yz2zwkbRtEAEjPi/download)

</details>

[Video zur Gegenfeldmethode](https://www.youtube.com/watch?v=Xm8LAEA7Gy8)


__Energiebilanz beim Photoeffekt__

> Die von den Lichtteilchen (Photonen) transportierte Energie $E_{ph}$ wird in Austrittsarbeit/Auslösearbeit $W_A$ der Elektronen und kinetische Energie $E_{kin, max}$ umgewandelt.
>
> $$ E_{ph} = E_{kin, max} + W_A $$
>
> _Hinweise:_ 
>
> - _die Austrittsarbeit/Auslösearbeit verschiedener Metalle finden Sie in der Formelsammlung S. 56_
>
> - _oben genannte Gleichung gilt für die Elektronen mit maximaler kinetischer Energie_



## 7. 4. Energie und Masse von Photonen

> Der äußere lichtelektrische Effekt legt nahe, dass das Licht auch Teilcheneigenschaften besitzt. 

> Wir nennen die Lichtteilchen @color(__Photonen__, blue). Jedes Photon trägt Energie mit sich, welche von seiner Frequenz bzw. Wellenlänge abhängt.

> __Die Energie __eines Photons
>
> $$ \boxed{E_{ph} = h \cdot f = \frac{h\cdot c}{\lambda}}$$


_Nutzt man die Äquivalenz aus Masse und Energie  $E = m \cdot c^2$ der speziellen Relativitätstheorie so beträgt:_


> __Die Masse__ eines Photons
>
> $$ \boxed{m_{ph} = \frac{E_{ph}}{c^2} = \frac{h \cdot f}{c^2} = \frac{h}{c\cdot \lambda}} $$

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

4. [Bitte anklicken: Verständnisfragen-Photoeffekt-KI-Gestützt](http://10.102.1.3:3001/?q=Stelle%20mir%20f%C3%BCnf%20Verst%C3%A4ndnisfragen%20zum%20Thema%20Photoeffekt,%20d.h.%20Expermentprinzip,%20Gegenfeldmethode,%20Berechnung%20des%20planckschen%20Wirkungsquantums,%20Licht%20als%20Teilchen.%20Stelle%20mir%20die%20Fragen%20einzeln%20nacheinander.%20Bewerte%20meine%20Antwort%20im%20Anschluss%20auf%20einer%20Skala%20von%200%20bis%2010.%20Mein%20Niveau%20ist%20Grundkurs%20Klasse%2012%20Physik.%20Gib%20mir%20am%20Schluss%20der%205%20Fragen%20ein%20Gesamtfeedback%20auf%20meine%20Antworten.)

---

5. ![Pitty_1115](https://diversewolken.ddns.net/nextcloud/index.php/s/rHpitZDaci8oTCm/download)Das Licht einer weißen Leuchtdiode (LED) wird untersucht. Das  Diagramm zeigt die Abhängigkeit der Strahlungsintensität von der Wellenlänge. (Quelle: http://ledmuseum.candlepower.us/led/specx02.htm) 

5. 1. Geben Sie die Wellenlängen der Photonen der beiden intensivsten Lichtanteile an.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_1$,455,$\mathrm{nm}$)

@rangeQuiz2($\lambda_2$,560,$\mathrm{nm}$)

</p>

---

5. 2. Ein schmales paralleles Bündel des LED-Lichtes durchläuft ein optisches Gitter. Es wird dadurch gebeugt und spektral zerlegt. Der Abstand Gitter-Schirm beträgt 2,0 m. Um gute Untersuchungsergebnisse zu erzielen, müssen die zwei lokalen Intensitätsmaxima in einem Spektrum 1. Ordnung mindestens den Abstand 5,0 cm voneinander haben. Berechnen sie, welche Gitterkonstante das genutzte Gitter höchstens haben darf.

<p style='margin-left:10%'>

@rangeQuiz2($g$,4.2e-6,$\mathrm{m}$)

</p>

---

<p style="margin-left:10%">

![Pitty1115_b](https://physikaufgaben.de/bild/a1115_2.jpg) Der Schirm wird entfernt. das gebeugte Licht fällt nun nach dem Durchlaufen einer schmalen Spaltblende auf die lichtempfindliche Schicht einer Fotozelle. Spaltblende und Fotozelle können parallel zum Gitter in y-Richtung bewegt werden. Die Abbildung zeigt das Prinzip.

</p>

---

5. 3. Untersuchen Sie rechnerisch, welche Ablösearbeit das Material der lichtempfindlichen Schicht der Fotozelle höchstens haben darf, damit Intensitätsverteilung mit der Fotozelle detektiert werden kann.

<p style='margin-left:10%'>

@rangeQuiz2($W_A$,1.65,$\mathrm{eV}$)

</p>

---

5. 4. Photonen einer bestimmten Wellenlänge des untersuchten Strahlungsspektrums lösen Elektronen mit der größten kinetischen Energie aus der lichtempfindlichen Schicht der Fotozelle heraus. Geben Sie diese Wellenlänge an und begründen Sie.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda$,400,$\mathrm{nm}$)

</p>