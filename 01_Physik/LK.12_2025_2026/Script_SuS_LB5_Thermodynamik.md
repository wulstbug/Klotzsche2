<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://diversewolken.ddns.net/nextcloud/s/SfR8K6Tn6mDEFkf/download

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

# LB 13 Thermodynamik (Wärmelehre)

![Thermodynamik](https://diversewolken.ddns.net/nextcloud/s/SfR8K6Tn6mDEFkf/download)

<section class="flex-container">

<div class="flex-child-2" style="min-width: 400px; margin-bottom: -10px">

> __Wikipedia:__ Die Wärmelehre hat ihren Ursprung im __Studium der Dampfmaschinen__ und ging der Frage nach, wie man @color(Wärme in mechanische Arbeit umwandeln, red) kann. Dazu beschreibt sie @color(Systeme, red) aus hinreichend @color(vielen Teilchen, red) und deren Zustandsübergänge anhand von __makroskopischen Zustandsgrößen__.

Zustandsgrößen eines Systems sind @color(__Temperatur__, blue), @color(__Druck__, blue) und @color(__Volumen__, blue).

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Dampfmaschine](https://upload.wikimedia.org/wikipedia/commons/8/8a/Triple_expansion_engine_animation.gif)

</div>

</section>

### 13. 1. Einführung

<section class="flex-container">

<div class="flex-child-2" style="min-width: 400px; margin-bottom: -10px">

Wir betrachten zunächst ein Gas in einem Behälter.


__Ideales Gas:__ Modell, bei dem die Gasteilchen als punktförmige Massepunkte ohne Eigenvolumen betrachtet werden, die keine Anziehungskräfte aufeinander ausüben. Einzige Wechselwirkung sind elastische Stöße zwischen den Teilchen.

</div>

<div class="flex-child-2" style="min-width: 200px; margin-bottom: -10px">

![GasImBehälter](https://www.grund-wissen.de/physik/_images/geschwindigkeitsverteilung-gasteilchen.png)

</div>

</section>



<br> <br>
<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Zustandsgröße:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Temperatur T__, blue)



</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Druck p__, blue)


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Volumen V__, blue)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Definition:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Die Temperatur ist ein Maß für die _mittlere Bewegungsenergie_ der einzelnen Teilchen. 

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Der Druck gibt an, welche Kraft $F$ ein Gas auf eine Fläche $A$ ausübt. <br> <br> $$ p = \dfrac{F}{A} $$

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Volumen gibt an, welchen Raumbereich ein Gas einnimmt.

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Einheit:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

K .. Kelvin (absolute Temperatur)

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Pa .. Pascal (Standardeinheit) <br>
bar .. Bar 


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

m$^{3}$ .. Kubikmeter <br>

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Bemerkungen:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">


_Eine Temperatur von $$T=0\,\mathrm{K} = -273,15^\circ\mathrm{C}$$ bedeutet, dass die Teilchen __keine Bewegungsenergie__ mehr besitzen, d.h. ihre Geschwindigkeit ist Null._

_Wird die Temperatur in $^\circ\mathrm{C}$ angegeben, so verwendet man das Formelzeichen $\vartheta$_. <br>

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">


_Ein Pascal entspricht einer Kraft von einem Newton pro Quadratmeter. <br> $$ \Big[ 1\,\mathrm{Pa} = 1 \dfrac{\mathrm{N}}{\mathrm{m}^2} \Big]$$  $$ \Big[ 1\,\mathrm{bar} = 100\,000\,\mathrm{Pa} \Big] $$


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

_Umrechnung von Volumina z.B. Liter -> m³ oder mm³ in m³ sollte geübt werden _

$$ \Big[ 1\,\mathrm{ℓ} = 10^{-3}\,\mathrm{m}^3\Big]$$ 

</div>

</section>
