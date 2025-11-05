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
| $\lambda$ in nm | $f$ in $10^{14}\,$Hz | $U_g$ in V | $E_{kin}=U\cdot e$ in eV |
| 365 | | |
| 405 | | |
| 436 | | |
| 546 | | |
| 577 | | |

@color(_Bereite die Tabelle vor. Ermittle bereits die zugehörigen Frequenzen._, blue)
