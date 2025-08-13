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

# LK Physik 2025/2026
<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg
-->

![WhyPhysics](https://cdn.sanity.io/images/i2z87pbo/production/986d42d83b06e224216a5129cdcfd179bf4ce59c-1440x1079.jpg)

@uhr

# LB 9 - Mechanische und elektromagnetische Schwingungen

## (optional) Definition eines periodischen Vorgangs

!?[Motivationsvideo](https://diversewolken.ddns.net/nextcloud/index.php/f/719652/downlaod)

{{1}}
************
> Definition: Wir beobachten eine Größe $B$. Der Wert von B zum Zeitpunkt t wird mit $B(t)$ bezeichnet. Wir nennen B eine <span style="color:orange">***periodische Größe***</span>, wenn sich die Werte von B nach einer bestimmten Zeit T wiederholen.
Es soll gelten:

> $$ B(t) = B(t+T) $$ <br> _In Worten: Der Wert von B zum Zeitpunkt t ist genauso groß, wie der Wert von B zum Zeitpunkt t+T._

> <span style="color:red">***T heißt Periodendauer ***</span> von B
************

## 9. 1. Beschreibung einer mechanischen Schwingung

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

## 9.2 Der Federschwinger (Beispiel 1)

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

## 9.3 Definition mechanische Schwingung

<p class="newspaper">

__Begriffe allgemein:__

> Eine __mechanische Schwingung__ ist die _periodische Änderung_ einer physikalischen Größe um eine __Ruhelage__.

- Die __momentane Auslenkung__( z.B. y(t) ) nennen wir @color(Elongation, red).

- Die __maximale Auslenkung__ ( z.B. $y_{max}$ oder $\hat{y}$ ) nennen wir @color(Amplitude, red).

<p class="cb">

__Am Beispiel des Federschwingers:__ <br> <br> ![Auslenkung-Federschwinger](https://diversewolken.ddns.net/nextcloud/index.php/s/YQGPkWDc5t2Bd5P/download)

</p>

</p>

### Experimentierauftrag zu Federschwingern

<p style="color:blue">

Untersuchen Sie die Federkonstante eines Federschwingers mit einem (1.) statischen und einem (2.) dynamischen Ansatz.

<details style="margin-left:10%">

<summary> Foto Experiment </summary>

![Foto-Experiment](https://diversewolken.ddns.net/nextcloud/index.php/s/NQsq6rKzrjDbLfr/download)

</details>

_Bemerkung:_

1. als statischen Ansatz nutzen sie die Auslenkung einer mechanischen Feder beim Anhängen eines bekannten Massestücks

2. als dynamischen Ansatz nutzen sie eine Schwingung und bestimmen Sie daraus die Federkonstante

---

$\Rightarrow$ A) Überlegen Sie, wie Sie jerweils Experimente durchführen könnten. 

$\Rightarrow$ B) Diskutieren Sie, welche Messgröße in Ihrem Setup die wesentliche Fehlerquelle ist. Schätzen Sie dazu den absoluten Fehler der Messung begründet ein.

$\Rightarrow$ C) Überlegen Sie, wie auftretende Messfehler möglichest gering halten können. Schlagen Sie dazu geeignete Messungen vor und vermeiden Sie Aussagen wie: _Einfach genauer messen_.

---

Vergleichen Sie Ihre Überlegungen hier.

<details style="margin-left:10%">

<summary> Hinweise zum 1. Experiment </summary>

A) Mit Hilfe der Proportionalität zwischen Federdehnung $s$ und wirkender Kraft $F$ $$F=D \cdot s$$ lässt sich die Federkonstante D bestimmen. Dazu muss ein Massestück mit bekannter Masse $m$ genutzt werden. Die wirkende Kraft ist dann die Gewichtskraft $F_g$. Gemessen wird die Federdehnung $s$.

B) Da die Masse $m$ als sehr genau bekannt angenommen werden kann, ist die wesentliche Fehlerquelle die Messung der Federdehnung $s$. Je nach Massband und Ablesemethode sollte man hier von einer Ungenauigkeit der Längenmessung von ca. 1-2mm ausgehen.

C)  Ist die Federdehnung nur sehr gering (d.h. mit einer sehr kleinen Masse), so ist der relative Fehler deutlich größer. Je stärker sich die Feder dehnt, desto geringer ist die Auswirkung der Ungenauigkeit. @color(Achtung: Feder nicht überdehnen., red)

</details>

     ---

<details style="margin-left:10%">

<summary> Hinweise zum 2. Experiment </summary>

A) Mit Hilfe einer Schwingung der Feder mit einem angehängten Massestück kann die Federkonstante bestimmt werden. Dazu muss die Schwingungsdauer $T$ ermittelt werden.

B) Da die Masse $m$ als sehr genau bekannt angenommen werden kann, ist die wesentliche Fehlerquelle die Messung der Periodendauer $T$. Durch die Reaktionszeit des Menschen kann der zufällige Messfehler der Zeitmessung auf etwa $0,3s$ abgeschätzt werden.

C) Misst man nur eine kurze Zeit (z.B. eine Schwingung), so wird der relative Fehler durch die Zeitmessung groß. Je länger die Zeitmessung ist, desto kleiner wird der relative zufällige Fehler (durch die Reaktionszeit). Es empfiehlt sich hier mehrere Schwingunen (z.B. $n=20-30$ Stück) zu messen. Der relative Fehler kann dann durch $n$ geteilt werden.

</details>

---

$\Rightarrow$ D) Führen Sie Ihre Messungen durch und dokumentieren Sie Ihre Messergebnisse adäquat.

<p style="margin-left:10%">

Näherungsweise Überprüfung des Messergebnisses

@rangeQuiz20($D$,21.1,$\frac{N}{m}$)

</p>


<details style="margin-left:10%">

<summary> Vergleichswerte Lehrkraft </summary>

1. Messwerte:

- $m = 100g$

- $s = 4,7 cm = 0,047m$

- $D \approx 21,3 \frac{N}{m} $

2. Messwerte:

- $m = 100g$

- $t=12,9s$ (bei $n=30$ Messungen)

- $D = 21,3 \frac{N}{m}$

</details>


---

$\Rightarrow$ E) Vergleichen Sie die Werte Ihrer Messergebnisse.


---

$\Rightarrow$ F) Schätzen Sie für jede Ihrer Messungen den zufälligen Fehler ab. Vergleichen Sie die Größe beider Fehler miteinander. Schlussfolgern Sie daraus auf die Genauigkeit beider Messmethoden.


<details style="margin-left:10%">

<summary> Vergleichswerte Lehrkraft </summary>

1. Fehlerrechnung

     - Absoluter Fehler: $\Delta s = 2 mm = 0,002 m$

     - Relativer Fehler: $\frac{\Delta s}{s} = 0,043 = 4,3 \%$

     - Relativer Fehler Federkonstante: $\frac{\Delta D}{D} =  4,3 \%$

2. Messwerte:

     - $\Delta t=0,3 s$ bei 30 Messungen

     - $\Delta T=0,01s$ bei $T=0,43s$

     - Relativer Fehler Periodendauer: $\frac{\Delta T}{T}=0,023 = 2,3%$

     - Relativer Fehler Federkonstante: $\frac{\Delta D}{D} =  2,3 \%$

---

Nach dieser Analyse kann die dynamische Methode als bevorzugt betrachtet werden. Hier kann der Fehler durch die Anzahl an beobachteten Schwingungen veringert werden.

</details>

</p>


### Theoretische Aufgabe zu Federschwingern

<p style="color:blue">

Aufgabe 9.3: Leite aus Proportionalität der Rücktreibenden Kraft (siehe 9.2, Annahme 1), dem zweiten Newton'schen Gesetz und den Gleichungen für momentane Auslenkung y(t), momentane Geschwindigkeit v(t) und Beschleunigung a(t) den Ausdruck für die Schwingungsdauer eines Federschwingers her.

_Diese Herleitung ist Teil der Tafelbilder. Löse sie soweit du kannst alleine, überprüfe deine Lösungen mit den Hilfen. Notiere sie im Hefter._

<details style="margin-left:10%">

<summary> Geführter Lösungsweg </summary>

1. Notiere die Annahme zur rücktreibenden Kraft aus 9.2.

<details style="margin-left:10%">

<summary> Lösung </summary>

$ F = - D \cdot y $

</details>

2. Notiere das zweite Newton'sche Gesetz.

<details style="margin-left:10%">

<summary> Lösung </summary>

$ F = m \cdot a $

</details>

3. Setze die Gleichungen für die Kräfte (1. & 2. gleich).

<details style="margin-left:10%">

<summary> Lösung </summary>

$ - D \cdot y = m \cdot a $

</details>

3. Notiere die Ausdrücke für y(t) und a(t) mit Hilfe der trigonometrischen Funktionen

<details style="margin-left:10%">

<summary> Lösung </summary>

$y(t) = y_{max} \cdot \sin(\omega \cdot t)$

$a(t) = -a_{max} \cdot \sin(\omega \cdot t)$ wobei $a_{max} = y_{max} \cdot \omega^2$ (siehe Lösung 9.1)

</details>

4. Setze die Ausdrücke für y(t) und a(t) in die Gleichung aus 3. ein. Löse die Gleichung nach der Periodendauer $T$ auf.

<details style="margin-left:10%">

<summary> Lösung </summary>

$ - D \cdot y(t) = m \cdot a(t) $

$ - D \cdot y_{max} \cdot \sin(\omega \cdot t) = m \cdot -a_{max} \cdot \sin(\omega \cdot t) $

$ - D \cdot y_{max} = m \cdot -y_{max} \cdot \omega^2 $

$ T = 2\pi \sqrt{\dfrac{m}{D}} $

</details>

</details>

</p>
