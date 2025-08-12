<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://www.sciencedaily.com/images/1920/Quantum-Clock.webp

@style
.lia-slide__footer {
      display: none !important;
}
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


# LB 9 - Mechanische und elektromagnetische Schwingungen
<!-- 
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg
-->

![WhyPhysics](https://examio-mediafiles.s3.eu-west-1.amazonaws.com/schwingung-sinus-print.jpg)

@uhr

## 9. 1. Definition eines periodischen Vorgangs

!?[Motivationsvideo](https://diversewolken.ddns.net/nextcloud/index.php/f/719652/downlaod)

{{1}}
************
> Definition: Wir beobachten eine Größe $B$. Der Wert von B zum Zeitpunkt t wird mit $B(t)$ bezeichnet. Wir nennen B eine <span style="color:orange">***periodische Größe***</span>, wenn sich die Werte von B nach einer bestimmten Zeit T wiederholen.
Es soll gelten:

> $$ B(t) = B(t+T) $$ <br> _In Worten: Der Wert von B zum Zeitpunkt t ist genauso groß, wie der Wert von B zum Zeitpunkt t+T._

> <span style="color:red">***T heißt Periodendauer ***</span> von B
************

## 9. 2. Beschreibung einer mechanischen Schwingung

{{1-2}}
********
??[Federschwinger](https://www.geogebra.org/m/g5vm3e2r)
********

{{2}}
********

Für eine mechanische Schwingung verwenden wir die physikalischen Größen _Momentanauslenkung_ ($y(t)$), Momentangeschwindigkeit ($v(t)$) und Momentanbeschleunigung ($a(t)$).

Für eine @color(harmonische Schwingung, orange) gelten die Zusammenhänge:

> $$y(t) = y_{max} \cdot \sin(\omega \cdot t)$$
>
> $$v(t) = \frac{\mathrm{d}y}{\mathrm{d}t}$$
>
> $$a(t) = \frac{\mathrm{d}v}{\mathrm{d}t}$$

<p style="color:blue">

Aufgabe: Ermittle für eine harmonische Schwinung aus dem Zusammenhang $y(t)$ die Ausdrücke für $v(t)$ und $a(t)$.

<details>

<summary> Lösung </summary>

![Loesung_9.1](https://diversewolken.ddns.net/nextcloud/index.php/s/YZRoKNqaTzAnFja/download)

</details>

</p>

********

{{3}}
********

Hier beschreibt $\omega$ die @color(Kreisfrequenz, orange), die definiert ist als

> $$ \omega = 2 \pi \cdot f = \dfrac{2 \pi}{T}  $$

und $T$ ist die @color(Periodendauer, orange).

********

## 9.3 Der Federschwinger (Beispiel 1)

Beschreibung: Ein Massestück hängt an einer Feder, wird ausgelenkt und losgelassen.

{{1-4}}
********
??[Federschwinger](https://www.geogebra.org/m/g5vm3e2r)
********


{{2}}
********

Annahmen:

1. Die Feder schwinkt nach dem Hook'schen Gesetz, das heißt die rücktreibende Kraft $F$ ist proportional zur Auslenkung $y$. Der Proportionalitätsfaktor ist die Federkonstante $D$.

$$ F = - D \cdot y $$

2. Das System schwingt reibungsfrei.

********

{{3}}
********
> Unter den Vorraussetzungen 1. und 2. lässt sich die Periodendauer $T$ sich mit Hilfe der Formel
>
>$$ \boxed{T = 2\pi \sqrt{\dfrac{m}{D}}} $$
>
>berechnen. Hier ist $m$ die angehängte Masse. 

********


### Aufgaben zu 9. 2./3. Schwingungen

1. Ermittle Frequenz, Kreisfrequenz und Periodendauer eines Tages. Nutze die Standardeinheiten.

<p style="margin-left:10%">

@rangeQuiz2($f$,1.1574e-5,$s$)

@rangeQuiz2($\omega$,7.2722e-5,$s$)

@rangeQuiz0($T$,86400,$s$)

<details style="margin-left:10%">

<summary> Lösungshinweise </summary>

Beginne mit der Periodendauer $T$. Überlege, wie lange die Periode eines Tages dauert. Berechne $T$ in Sekunden. Nutze anschließend die Formeln aus 1. um $f$ und $\omega$ zu berechnen.

</details>

</p>


2. An eine Hook'sche Feder soll eine Masse gehängt werden, sodass eine vollständige Schwingung genau eine Sekunde dauert.Die Federkonstante $D$ beträgt $0.4\frac{N}{m}$. Ermitteln Sie aus den Angaben die Masse in der Einheit Gramm, welche angehängt werden muss.

<p style="margin-left:10%">

@rangeQuiz2($m$,10.13,$g$)

</p>

<details style="margin-left:10%">

<summary> Lösungshinweise </summary>

Verwenden Sie die Formel zur Ermittlung der Periodendauer eines Federschwingers. Stellen Sie diese Formel nach der Masse um.

</details>

<details style="margin-left:10%">

<summary> Lösungsweg </summary>

![Loesung-2.1.2](https://diversewolken.ddns.net/nextcloud/index.php/s/D9eJbRdg5wja99t/download)

</details>