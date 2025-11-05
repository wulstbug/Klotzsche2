<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

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

# LK Physik 2025/2026
<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg
-->

![WhyPhysics](https://cdn.sanity.io/images/i2z87pbo/production/986d42d83b06e224216a5129cdcfd179bf4ce59c-1440x1079.jpg)

@uhr

# LB 9 - Mechanische und elektromagnetische Schwingungen

## 9. 1. (optional) Definition eines periodischen Vorgangs

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

## 9. 3. Der Federschwinger (Beispiel 1)

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

@rangeQuiz2($f$,1.1574e-5,$Hz$)

@rangeQuiz2($\omega$,7.2722e-5,$\frac{1}{s}$)

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

## 9. 4. Definition mechanische Schwingung

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


### Rechenaufgaben zum Federschwinger

Ein vertikaler Federschwinger besteht aus einer Feder mit der Federkonstante D = 2,5 N/m und einem angehängten Körper mit der Masse m = 0,10 kg. Der Abstand zwischen den Umkehrpunkten des schwingenden Körpers beträgt s = 10 cm.

- a)  Skizzieren Sie das y-t-Diagramm für mindestens eine Periode. Geben Sie eine Schwingungsgleichung mit den speziell vorgegebenen Werten an.

<details style="margin-left:10%">

<summary> Lösung a) </summary>

![Lsg_9.3_a](https://diversewolken.ddns.net/nextcloud/index.php/s/Ger7Mg4LraekEGn/download)

</details>

---

- b) Geben Sie für den Zeitpunkt t = 0,10 s die Elongation an.

<details style="margin-left:10%">

<summary> Lösung b) </summary>

![Lsg_9.3_a](https://diversewolken.ddns.net/nextcloud/index.php/s/LFxTxsAtHFTj5pg/download)

</details>

---

- c)  Geben Sie eine Möglichkeit an, wie durch Veränderung der gegebenen Größen die Frequenz des Oszillators halbiert werden kann. Begründen Sie Ihre Antwort.

<details style="margin-left:10%">

<summary> Lösung c) </summary>

![Lsg_9.3_c](https://diversewolken.ddns.net/nextcloud/index.php/s/2SyNqYTKqoRxHe4/download)

</details>

---

- d) Ermitteln sie die maximale Geschwindigkeit des Massestücks, sowie die maximale Beschleunigung. Geben Sie jeweils auch die zugehörigen Zeitpunkte an.

<details style="margin-left:10%">

<summary> Lösung d) </summary>

Die maximale Geschwindigkeit $v_{max}$ kann mit der Formel

$v_{max} = y_{max} \cdot \omega = y_{max} \cdot \frac{2\pi}{T}$

ermittelt werden. Laut a) ist $T = 1,26 s$ und $y_{max}=0,05m$. Es ergibt sich

$ \underline{v_{max} = 0,249 \frac{m}{s}}$

Die maximale Geschwindigkeit wird zu den Zeitpunkten erreicht, wo die Funktion $cos(\omega t)$ maximal wird. Das geschieht periodisch bei

- $t = 0$

- $t = T/2 = 0,63s$

- $t= T = 1,26s$

- ...

---

Die maximale Beschleunigung $a_{max}$ kann mit der Formel

$a_{max} = y_{max} \cdot \omega^2 = y_{max} \cdot \frac{(2\pi)^2}{T^2}$

ermittelt werden. Laut a) ist $T = 1,26 s$ und $y_{max}=0,05m$. Es ergibt sich

$\underline{a_{max} = 1,24 \frac{m}{s^2}}$

Die maximale Beschleunigung wird erreicht, wenn die Funktion $\sin(\omega t)$ maximal wird.

Das geschieht periodisch bei

- $t = T/4 = 0,315s$

- $t = 3T/4 = 0,945s$

- $t= 5T/4 = 1,575s$

- ...

Hier ist nochmal die Verschiebung von $y(t)$, $v(t) und $a(t)$ in einem gemeinsamen Diagramm dargestellt.

![Diagramme-y-v-t](https://www.leifiphysik.de/sites/default/files/2021/05/image/Harmonische-Schwingungen-Diagramm_vereinfacht_03.svg)

</details>

- e) [Aufgabe-LEIFI-Physik-Bungee-Eifelturm](https://www.leifiphysik.de/mechanik/mechanische-schwingungen/aufgabe/bungeesprung-vom-eiffelturm)

## 9. 5. Das Fadenpendel

{{0-1}}
**********
!?[0-1](https://www.youtube.com/watch?v=smAGZVa1TJE)
**********


{{1}}
*********
![TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/rnojn8pF2ZWsFaJ/download)

![TB2](https://diversewolken.ddns.net/nextcloud/index.php/s/ayq4NXMCQMbc5Bt/download)
*********

### Übung: Schwingungen ja/nein

Entscheiden Sie für die folgenden Beispiele, ob es sich dabei um eine Schwingung (nach Definition handelt) oder nicht. Begründen Sie Ihre Aussage in jedem Fall.

<p style="margin-left:5%">

1. Ein Kind sitzt auf einer Schaukel, die Schaukel wird von einem Elternteil ausgelenkt und losgelassen. 

     - [(x)] Ja
     - [(x)] Nein

<details style="margin-left:5%">

<summary> Begründung: </summary>

Hier sind beide Antworten richtig, @color(wenn, red) die passende Begründung gegeben werden kann.

__Antwort Ja:__ Wenn Sie diese Antwort mit Ja beantwortet haben, müssen sie begründen unter welchen Bedingungen die Bewegung periodisch (d.h. zeitlich wiederkehrend) ist. Das gilt nur, wenn man Reibungseffekte vernachlässigt.

__Antwort Nein:__ Wenn Sie diese Antwort mit Nein beantwortet haben, müssen sie begründen warum es keine Schwingung ist. Hier kann man argumentieren, dass sich die Schaukelhöhe durch Reibung mit der Zeit verlangsamt. Daher ist es keine periodische Bewegung und somit laut Definition (siehe 3.) kein periodischer Vorgang. Man nennt diesen Vorgang @color(gedämpfte Schwingung, orange).

</details>

---

2. Ein Tischtennisball wird über einer Platte losgelassen und springt senkrecht auf der Platte auf und nieder. Sie können Reibungsverluste hier vernachlässigen.

     - [( )] Ja
     - [(x)] Nein

<details style="margin-left:5%">

<summary> Begründung: </summary>

__Antwort Nein:__ Egal ob man diesen Prozess mit oder ohne Reibung betrachtet, es ist keine Schwingung, da es hier keine Ruhelage gibt.

</details>

---

3. Ein Bungeespringer spring an einem elastischen Seil von einer Brücke. Das Seil soll sich wie eine mechanische Feder (Hook'sches Gesetz ist gültig) verhalten, Reibung und andere Verluste werden vernachlässigt. Seillänge, Seildehnung und Bodenabstand sollen derart sein, dass der Springer den Boden nicht berührt.

     - [(x)] Ja
     - [( )] Nein

<details style="margin-left:5%">

<summary> Begründung: </summary>

__Antwort Ja:__ Diese Bewegung entspricht einer Schwingung, da es eine periodische Bewegung ist, die um eine Ruhelage (der Springer hängt ruhig am Seil) stattfindet.

</details>


---

4. Ein Planet (z.B. die Erde) kreist auf einer elliptischen Bahn um die Sonne.

     - [( )] Ja
     - [(x)] Nein

<details style="margin-left:5%">

<summary> Begründung: </summary>

__Antwort Nein:__ Diese Bewegung ist streng periodisch, aber es gibt keine Ruhelage, um welche die Bewegung stattfindet.

</details>

</p>

### Übung: Die Abrissbirne (aus Abi95)

![Abrissbirne](https://diversewolken.ddns.net/nextcloud/index.php/s/LwyBrGzFRBZYgwi/download)Zum Beseitigen baufälliger Mauern werden oft sogenannte Abrißbirnen verwendet. Das sind kleine, massereiche Körper, die an einem Stahlseil hängen. Sie werden ausgelenkt und schlagen nach dem Freigeben gegen die zu zerstörende Mauer. <br> Eine solche Abrißbirne mit der Masse 520 kg hängt an einem 6,80 m langen Seil mit vernachlässigbarer Masse. <br> Das Seil wird um α = 34° ausgelenkt. Aus diesem Zustand heraus wird die Birne freigegeben und stößt nach Durchlaufen ihrer tiefsten Lage gegen die 0,58 m davon entfernte Mauer. Die Bahn der Birne liegt in einer Ebene senkrecht zur Mauer. Die Birne darf als Massenpunkt angesehen werden.

- a) Beschreiben Sie die Energieumwandlungen bei einem schwingenden Fadenpendel.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Abi95_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/WmgoTpTo3BDNWx8/download)

</details>

---

- b) Berechnen Sie die Geschwindigkeit und die kinetische Energie der Abrissbirne in ihrer tiefsten Lage.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Abi95_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/XTpTS4BQFQzNXJ2/download)

</details>

---

- c) Berechnen Sie die Geschwindigkeit und die kinetische Energie der Birne beim Aufprall auf die Mauer.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Abi95_Lsg_c1](https://diversewolken.ddns.net/nextcloud/index.php/s/eZ3i3S64qCo9ixK/download)

![Abi95_Lsg_c2](https://diversewolken.ddns.net/nextcloud/index.php/s/E6epdYKzyEoSXKs/download)

</details>

---

- d) Näherungsweise wird Zeit, die die Abrissbirne von der Auslenkung bis zur Ruhelage durchläuft mit $t = 1,3 s$. Geben Sie an, wie man rechnerisch zu diesem Ergebnis kommen kann. Erklären Sie, warum diese Zeit lediglich näherungsweise zutrifft.

<details style="margin-left:10%">

<summary> Lösung </summary>

Die Abrissbirne kann näherungsweise als Pendel der Länge 6,8m betrachtet werden. Die Schwingungsdauer für ein solches Pendel kann für kleine Auslenkungen mit der Formel

$$ T = 2\pi \sqrt{\dfrac{ℓ}{g}}$$

berechnet werden, wobei $ℓ$ die Seillänge ist. Es ergibt sich eine Schwingungsdauer von $T=5,23s$ und da hier 1/4 der Bewegung stattfindet kann man die Zeit mit $t=(5,23/4) s=1,3s$ abschätzen.

Da die Birne allerdings um 34° ausgelenkt wird, gilt die @color(Kleinwinkelnäherung, orange) nicht, welche für die obige Formel Vorraussetzung ist.

</details>

---

## 9. 6. Simulation eines Pendels (_ohne Kleinwinkelnäherung_)

Für die Simulation einer Pendelschwingung mit der Länge 1m wird die Simulationssoftware Moebius verwendet

__A. Formelgrundlage für die Simulation__

> 1. Masse und Gewichtskraft
>
> $$ F_g = m \cdot g $$
>
> 2. Rücktreibende Kraft ($\varphi = \frac{x}{ℓ}$)
>
> $$ F_r = - F_g \cdot \sin(\frac{x}{ℓ}) $$
>
> 3. Newton'sche Bewegungsgesetze
> 
> $$ a = \frac{F}{m} $$


__B. Hinweise zum Simulationscode__

- Gleichung 1. können wir direkt verwenden

- Gleichung 2. stellt die Rücktreibende Kraft bei der Auslenkung um den Winkel $\varphi$ dar

- Gleichung 3. enthält die klassische Modellierung einer Bewegung (Geschwindigkeit und Ort müssen noch ergänzt werden)

> @color(__Erstellen Sie aus diesen Gleichungen den Simulationscode.__, blue)

---

<details style="margin-left:5%">

<summary> Lösung Code </summary>

``` 

PROGRAMM: (Pendel)

Fg=m*g
Fr = -Fg*sin(x/l)
a=Fr/m
v=v+a*dt
x=x+v*dt
t=t+dt


```

</details>

---

__C. Hinweise: Analyse der Anfangsbedingungen (t=0)__

- die Masse kann hier mit 0,1 kg angenommen werden

- die Pendellänge kann mit 1m angenommen werden

- der Startwert für die Länge $x$ muss aus dem Startwinkel $\varphi$ berechnet werden


__D. Überprüfung der Simulation__

> Wählen Sie für Ihre erste Simulation einen kleinen Anfangswinkel $\varphi$ von $1^\circ$. Ermitteln Sie mit Hilfe Simulation die Periodendauer $T$ und vergleichen Sie Ihr Ergebnis mit dem Resultat für die Periodendauer aus 9.5 (_Kleinwinkelnäherung_)

<details style="margin-left:5%">

<summary> Lösung für $\varphi=1^\circ$ </summary>

![Lsg_1Grad](https://diversewolken.ddns.net/nextcloud/index.php/s/q6izMWEkXY3tNWs/download)

__Modellierung:__ Aus der Messwerttabelle und dem Diagramm lässt sich entnehmen, dass die Periodendauer $T=2s$ beträgt.

__Formel:__ $T=2\pi\sqrt{\frac{ℓ}{g}}=2,006 s$ überein. 

</details>

---

__E. Analyse der Kleinwinkelnäherung__

> Nutzen Sie nun Ihre Simulation um die Abweichung der Periodendauer in Kleinwinkelnäherung von der Periodendauer der Simulation zu untersuchen. Ermitteln Sie dazu die Periodendauern für Startwinkel 1-90° in sinnvollen Schritten. Tragen Sie in einem Diagramm die prozentuale Abweichung der Kleinwinkelnäherung von dem Simulationsergebnis auf. 
>
>Schätzen Sie an Ihrem Diagramm den Startwinkel $\Phi$ ab, bei welchem der Fehler 10% überschreitet.
>
> @color(__Achtung: Dokumentieren Sie Ihre Simulationsergebnisse sinnvoll! Nutzen Sie z.B. eine Tabelle im Hefter oder am PC.__, red)


<details style="margin-left:5%">

<summary> Vergleichswerte </summary>

20° -> Abweichung ca. 0,75%

30° -> Abweichung ca. 1,7%

</details>



<details style="margin-left:5%">

<summary> Diagramm </summary>

![Diagramm-Vergleich-Simulation-KWN](https://diversewolken.ddns.net/nextcloud/index.php/s/EMyjstYCcnSEt28/download)

</details>

## 9. 7. Gedämpfte Schwingung

> Im folgenden soll eine Schwingung simuliert werden, bei der die Amplitude abnimmt. Speichere deine Simulation unter einem neuen Namen (z.B. Pendel-Daempfung) und versuche eine Reibungskraft in die Simulation einzufügen.

??[Federschwinger](https://www.geogebra.org/m/g5vm3e2r)

{{1}}
**************
Speichern Sie Ihr Programm unter einem neuen Namen. Verändern Sie Ihr Programm so, dass auf das Pendel eine konstante Reibungskraft wirkt.
**************

<details style="margin-left:5%">

<summary> Hinweise </summary>

Die Reibungskraft muss an den Bewegungszustand angepasst werden. Sie wirkt immer @color(entgegen,red) der Bewegungsrichtung.

Nutzen Sie für die Ermittlung der Rückstellenden Kraft die IF .. THEN .. (Wenn ... Dann ..) Anweisung.

<details style="margin-left:5%">

<summary> Lösung </summary>

Erfragen Sie Hilfe bei der Lehrkraft.

</details>

</details>

### Simulation zur gedämpften Schwingung

> Aufgabenstellung: 
>
> 1. Erstellen Sie ein Programm mit _Möbius_, welches eine Pendelschwingung der Länge 1 m und einer Anfangsauslenkung von 1° simuliert. 
>
> 2. Erstellen Sie das s(t) Diagramm und laden Sie Ihre Simulation (__Dateiname anpassen__) [DateiAblage](https://diversewolken.ddns.net/nextcloud/index.php/s/5HEGHD6NCqSawyF) hoch. Lassen Sie sich die Simulation von der Lehrkraft ausdrucken.
>
> 3. Fügen Sie nun eine konstante Reibungskraft in Ihrer Simulation derart ein, dass sich die Ampitude der Schwingung in jeder Periode um 5 % veringert. 
>
> 4. Erstellen Sie das s(t) Diagramm und laden Sie Ihre Simulation (__neuer Dateiname!__) [DateiAblage](https://diversewolken.ddns.net/nextcloud/index.php/s/5HEGHD6NCqSawyF) hoch. Lassen Sie sich die Simulation der gedämpften Schwingung von der Lehrkraft ausdrucken.
>
> 5. Berechnen Sie näherungsweise den prozentualen Anteil der Energie, der während einer Periode an die Umgebung angegeben wird.

---

__Überprüfung:__

<p style="margin-left:10%">

@rangeQuiz2($F_{reib}$,0.0002,$N$)

@rangeQuiz2($\dfrac{E_0-E_1}{E_0}$,13,$\%$)

</p>

<details style="margin-left:5%">

<summary> Lösung </summary>

Startwerte:

- $x_0 = 0.0175$, $\varphi_0 = 1^\circ$

- $T = 1s$

- $F_{Reib}=0,85 N$

- $x_1 = 0.0165$, $\varphi_0 = 0,93^\circ$

- $\frac{E_1}{E_0}=\frac{m\cdot g \cdot l \cdot(1-\cos(\varphi_1))}{m\cdot g \cdot l \cdot(1-\cos(\varphi_0))}=0,87$

- -> 13% gehen verloren

</details>

## 9. 8. Energieumwandlungen bei Schwingungen

> Bei einer (mechanischen) Schwingung wird die in der Schwingung gespeicherte Energie periodisch zwischen verschiedenen Energieformen umgewandelt

{{1}}
***********
<p style="margin-left:10%">

__Beispiel: Federschwinger__ (auftretende Energieformen)

__Mechanische Energieformen:__

- potentielle Energie (Lageenergie)     
     -> $E_{pot} = m \cdot g \cdot h$

- kinetische Energie (Bewegungsenergie)
     -> $E_{kin} = \frac{1}{2}\cdot m \cdot v^2$

- Spannenergie (Federdehnung)
     -> $E_{sp} = \frac{1}{2} \cdot D \cdot s^2$

__Reibung:__

- Thermische Energie

{{2}}
***********
??[Simulation-PHeT-FederSchwinger](https://phet.colorado.edu/sims/html/masses-and-springs/latest/masses-and-springs_all.html?locale=de)
***********


{{3}}
***********
<p class="newspaper">

> Bei einem @color(_idealen=reibungsfreien_,orange) Federschwinger ist die Summe aller mechanischer Energien konstant. Energie wird zwischen Lageenergie, Spannenergie und kinetischer Energie umgewandelt.
>
> Bei einem realen Federschwinger wird ein Teil der Energie in thermische Energie umgewandelt. Die Amplitude der Schwingung sinkt mit der Zeit. Eine solche Schwingung nennt man @color(gedämpfte Schwingung, red).


<p class="cb">

![Graph-Gedaempfte-Schwingung](https://diversewolken.ddns.net/nextcloud/index.php/s/eLDW3kNxPrXWRBP/download "Beispiel einer gedämpften Schwingung mit schwacher Dämpfung") <!-- style="max-height:300px" -->

</p>

</p>
***********

</p>
***********

### Aussagen zur Gedämpften Schwingung

@color(Entscheiden Sie für die folgenden Aussagen. Nutzen Sie im Zweifel die Simulation., blue)

-> [Simulation-PHeT-FederSchwinger](https://phet.colorado.edu/sims/html/masses-and-springs/latest/masses-and-springs_all.html?locale=de)

---

<!-- data-solution-button="off" -->
[[ richtig | (falsch) ]] 1. In der Ruhelage ist die Spannernergie gleich Null.

---

<!-- data-solution-button="off" -->
[[ richtig | (falsch) ]] 2. In der Ruhelage ist die kinetische Energie minimal.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 3. In der Ruhelage ist kinetische Energie maximal.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 4. Im unteren Umkehrpunkt ist die Spannenergie maximal.

---

<!-- data-solution-button="off" -->
[[ richtig | (falsch) ]] 5. Im oberen Umkehrpunkt ist die Spannenergie immer Null.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 6. Im oberen Umkehrpunkt ist die Spannenergie minimal.

---

<!-- data-solution-button="off" -->
[[ richtig | (falsch) ]] 6. Bei einer gedämpften Schwingung ist die Summe aller mechanischen Energien konstant.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 7. Bei einer ungedämpften Schwingung ist die Summe aller mechanischen Energien konstant.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 8. Tritt bei einem Federschwinger Reibung auf, so verringert sich die Amplitude mit der Zeit.

---

<!-- data-solution-button="off" -->
[[ (richtig) | falsch ]] 9. Bei einem gedämpften Federschwinger gilt der Energieerhaltungssatz.


### Übung Gedämpfte Schwingung

Bei jeder (realen) mechanischen Schwingung wird Energie durch Reibung an die Umgebung abgegeben. Im Experiment wird der Schwingungsverlauf bei laminarer Reibung des Federpendels in Wasser aufgenommen. Die Federkonstante beträgt $D=10\frac{N}{m}$.

![Aufgabe-Gedaempfte-Schwingung](https://diversewolken.ddns.net/nextcloud/index.php/s/gYaziaBmrreoNbF/download)

[Geogebra-Lsg](https://www.geogebra.org/classic/m4p2mtac)

1. Der Graph kann näherungsweise durch die Gleichung $s(t)=\hat{s}\cdot e^{-k\cdot t}\cdot \cos(\omega\cdot t)$ beschrieben werden. Bestimmen Sie aus dem Graphen die Größen $\hat{s}$, $k$, $\omega$ und $f$.

<p style="margin-left:10%">

@rangeQuiz2($\hat{s}$, 0.04 ,$m$)

@rangeQuiz2($k$, 0.575 ,$\dfrac{1}{s}$)

@rangeQuiz2($\omega$, 12.566 ,$\dfrac{1}{s}$)

@rangeQuiz2($f$, 2 ,$Hz$)

</p>

---

2. *Ermitteln Sie den mathematischen Ausdruck für $v(t)$. 

<details style="margin-left:10%">

<summary> Lösungshinweise </summary>

Die Geschwindigkeit $v(t)$ ist definiert als die erste Ableitung der Orts-Funktion $s(t)$ nach der Zeit $t$. Leiten Sie die Gleichung für $s(t)$ aus Aufgabe 1 nach der Zeit $t$ ab, d.h.

$$ v(t) = \frac{\mathrm{d}s}{\mathrm{d}t} $$

<details  style="margin-left:10%">

<summary> Lösung </summary>

Es gilt: $$v(t) = \frac{\mathrm{d}s}{\mathrm{d}t}$$

Die Gleichung für $s(t)$ lautet:

$$ s(t)=\hat{s}\cdot e^{-k\cdot t}\cdot \cos(\omega\cdot t) $$

$s(t)$ ist ein Produkt aus zwei Funktionen, farblich dargestellt

$$ s(t)=\hat{s}\cdot \blue{e^{-k\cdot t}} \cdot \red{\cos(\omega\cdot t)} $$

Vereinfacht dargestellt ist $s(t)$ also das Produkt aus zwei Funktionen $\blue{g(t)=e^{-k\cdot t}}$ und $\red{h(t)=\cos(\omega\cdot t)}$.

$$ s(t)=\hat{s}\cdot \blue{g(t)} \cdot \red{h(t)} $$

Nach der Kettenregel ist die Ableitung eines Produktes:

$$ \frac{\mathrm{d}s}{\mathrm{d}t} =\hat{s}\cdot \Big( \blue{g'(t)} \cdot \red{h(t)} + \blue{g(t)} \cdot \red{h'(t)}\Big) $$

Die einzelnen Ableitungen ergeben:

$$ \blue{g'(t) = -k \cdot e^{-k\cdot t}} $$

und

$$ \red{h'(t) = -\omega \cdot \sin(\omega\cdot t)} $$

Daraus ergibt sich für die momentane Geschwindigkeit $v(t)$

$$ v(t) = -\hat{s} \cdot \blue{k \cdot e^{-k\cdot t}} \cdot \red{\cos(\omega\cdot t)} - \hat{s} \cdot \blue{e^{-k\cdot t}} \cdot \red{\omega \cdot \sin(\omega\cdot t)} $$

$$ \boxed{v(t) = -\hat{s} \cdot \blue{e^{-k\cdot t}} \cdot \Big(\blue{k}\cdot \red{\cos(\omega\cdot t)} + \red{\omega \cdot \sin(\omega\cdot t)}\Big)} $$

</details>

</details>

---

3. Bestimmen Sie aus dem Ausdruck für $v(t)$ die Geschwindigkeit für den Zeitpunkt $t=0,125 s$. Geben Sie den Betrag der Geschwindigkeit an. <br> _Hinweis: Wenn Sie die Aufgabe 2 nicht lösen konnten, verwenden Sie die Lösung aus 2. zur Bearbeitung dieser Aufgabe._

<p style="margin-left:10%">

@rangeQuiz2($|v_{0.125s}|$, -0.46777 ,$\frac{m}{s}$)

</p>

---

4. *Ermitteln Sie einen Zeitpunkt $t>0$, an welchem die Geschwindigkeit $v=0$ ist. Geben Sie die Lösung zunächst Näherungsweise an, berechnen Sie dann den Zeitpunkt genau.

<p style="margin-left:10%">

__Näherung:__

@rangeQuiz0($t$,0.25,$s$)

__Exakte Lösung:__

</p>

<details style="margin-left:10%">

<summary> Lösungshinweise </summary>

Setzen Sie die Gleichung (s. Lsg 2.) für $v(t)$ gleich Null. 

$$ v(t) = 0 $$

<details  style="margin-left:10%">

<summary> Lösung </summary>

Es sei $$v(t) = 0$$ d.h.

$$ 0 = -\hat{s} \cdot \blue{e^{-k\cdot t}} \cdot \Big(\blue{k}\cdot \red{\cos(\omega\cdot t)} + \red{\omega \cdot \sin(\omega\cdot t)}\Big)$$

Da sowohl die Konstante $\hat{s}$ als auch die $e$-Funktion $\blue{e^{-k\cdot t}}$ nicht Null werden, kann man diese kürzen und es ergibt sich:

$$ 0 = \blue{k}\cdot \red{\cos(\omega\cdot t)} + \red{\omega \cdot \sin(\omega\cdot t)} \hspace{1cm}\Big| -\red{\omega \cdot \sin(\omega\cdot t)}$$

$$ -\red{\omega \cdot \sin(\omega\cdot t)} = \blue{k}\cdot \red{\cos(\omega\cdot t)} \hspace{1cm}\Big| : \red{\cos(\omega\cdot t)} $$

$$ -\red{\omega \cdot \tan(\omega\cdot t)} = \blue{k} \hspace{1cm}\Big| : \red{-\omega} $$

$$ \red{\tan(\omega\cdot t)} = -\dfrac{\blue{k}}{\red{\omega}} \hspace{1cm}\Big| \tan^{-1} $$

$$ \red{\omega\cdot t} = \tan^{-1}\Big(-\dfrac{\blue{k}}{\red{\omega}}\Big) \hspace{1cm}\Big| : \red{\omega} $$

An dieser Stelle kann man zwei Lösungswege verfolgen.

<p class="newspaper">

__1. Weg:__

$$ t = \frac{1}{\red{\omega}} \tan^{-1}\Big(-\dfrac{\blue{k}}{\red{\omega}}\Big)$$

$$ t = -0,00364s $$

Diese mathematische Lösung gibt an, dass das System kurz vor dem Zeitpunkt $t=0s$ die Geschwindigkeit $v=0s$ erreicht hat. Ein weiterer Zeitpunkt wäre kurz vor erreichen von $T/2$, d.h.

$$ t = \frac{T}{2} - 0,00364s $$
$$ t = 0,246s $$

<p class="cb">

__2. Weg__

Um die Zeitpunkte größer als 0 zu erhalten, kann man hier die Symmetrie des $\tan$ nutzen und auf der rechten Seite $n\cdot\pi$ addieren, wobei $n \in \N$.

$$ t = \frac{1}{\red{\omega}} \big(\tan^{-1}\Big(-\dfrac{\blue{k}}{\red{\omega}}\big) + n\cdot\pi \Big)$$

Den ersten Zeitpunkt erhält man für $n=1$ und es ergibt sich

$$ t = 0,246s $$

</p>

</p>

</details>

</details>

## 9. 9. Erzwungende Schwingungen und Resonanz

{{0}}
*****************
!?[BayOfFundy](https://www.youtube.com/watch?v=Mm5kaArK4FA)
*****************

### Demonstrationsexperiment

<p class="newspaper">

__Foto:__

![Demo-Erzwungene-Schwingung](https://diversewolken.ddns.net/nextcloud/index.php/s/H2s3ECYWkL9ygoc/download)<!-- style="max-height:400px"-->

<p class="cb">

__Skizze:__

![Demo-Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/6dpA32wA3WayA5M/download)

{{4}}
**********
$f_0 = \frac{1}{T_0}$ (siehe _Experiment Federschwinger_)
**********

{{5}}
**********
$f_0 = \frac{1}{0,4s}$ = 2,5 Hz
**********

</p>

</p>

{{1}}
**********
__1. Messung:__ Abhängigkeit der @color(Erregerfrequenz $f_E$ d.h. Motor, green) von der angelegten Spannung U. 
**********

{{2-3}}
***********
![Messung-U-f-1](https://diversewolken.ddns.net/nextcloud/index.php/s/T59sri22ftXSyrp/download)
***********

{{3}}
***********
![Messung-U-f-1](https://diversewolken.ddns.net/nextcloud/index.php/s/WSswxZj3BfcrcGe/download) Lineare Regression (@color(Ausgleichsgerade,red)) <br>$\boxed{\red{f(U) = 0,57 \frac{Hz}{V} \cdot U - 0,22 Hz}}$
***********

{{6}}
***********
__2. Messung:__

Abhängigkeit der @color(Amplitude des Federpendels, blue) von der Erregerfrequenz $f_E$.
***********

{{7}}
***********
<p style="margin-left:10%">
__Beobachtung:__

Die Amplitude des Federpendels steigt, je näher die @color(Erregerfrequenz $f_E$, green) der Eigenfrequenz $f_0$ des Systems kommt.
</p>
***********

{{8}}
*******
![Resonanz](https://diversewolken.ddns.net/nextcloud/index.php/s/iBAFKiD7Gs8faq9/download)
*******


### Beispiel 2

!?[Motivation-Video-Tacoma-Bridge](https://www.youtube.com/watch?v=XggxeuFDaDU)

### Simulation zur erzwungenen Schwingung

[LEIFI-Simulation-Erzwungene-Schwingung](https://www.leifiphysik.de/mechanik/kopplung-von-schwingungen/versuche/erzwungene-schwingung-eines-federpendels-simulation)


### Eigenschaften einer erzwungenen Schwingung

{{1}}
*****************
> Bei einem schwingenden System kann eine @color(periodische äußere Anregung, red) dem System permanent Energie zuführen. Die äußere Anregung erfolgt dabei mit Erregerfrequenz $f_E$. Die Frequenz des frei schwingenden Systems wird als  @color(Eigenfrequenz, red) $f_0$ bezeichnet. Eine solche äußere Anregung nennt man @color(erzwungene Schwingung, red).
*****************

{{2}}
*****************
> Es lassen sich folgende Grenzfälle beobachten

> 1. Für $f_E \ll f_0$: Erregerfrequenz ist sehr viel kleiner als Eigenfreqenz: @color(__niederfrequenter Bereich__, red)
>
> - Erreger und Schwinger haben beinahe die gleiche Amplitute.
>
> - Erreger und Schwinger haben fast keinen Phasenunterschied $\Delta\varphi\approx 0$
*****************

{{3}}
*****************
> 2. Für $f_E \approx f_0$: Erregerfrequenz ungefähr gleich der Eigenfreqenz: @color(__Resonanzfall__, red)
>
> - Amplitude des Schwingers ist viel höher als die Amplitude des Erregers
>
> - je nach Dämpfung des Schwingers kann dessen Amplitude viel größer werden, als die des Erregers
>
> - der Erreger eilt dem Schwinger um die Phase  $\frac{\pi}{2}$ vorraus: $\Delta\varphi\approx \frac{\pi}{2}$
*****************

{{4}}
*****************
> 3. Für $f_E \gg f_0$: Erregerfrequenz viel größer als Eigenfrequenz: @color(__hochfrequenter Bereich__, red)
>
> - Amplitude des Schwingers ist wesentlich kleiner als die Amplitude des Erregers
>
> - der Phasenunterschied zwischen Erreger und Schwinger beträgt fast $\pi$: $\Delta\varphi\approx \pi$
*****************

### (*) Quiz zu erzwungenen Schwingungen

[LEIFI-Quiz-Erzwungene-Schwingungen](https://www.leifiphysik.de/mechanik/kopplung-von-schwingungen/aufgabe/quiz-zu-erzwungenen-schwingungen)

### Aufgaben Resonanz/Erzwungene Schwingung (**)

1. Schwingender Holzdrache

<p style="margin-left:10%">


Zur Dekoration in einer Spielzeugabteilung soll ein Holzdrache zum Einsatz kommen,
der an einer Schraubenfeder vertikal harmonisch schwingt und dessen Flügel dabei in Bewegung versetzt werden. Der Drache hat eine Masse von 500 g. Betrachten Sie den Drachen zunächst als Massepunkt.
Als Ruhelage y = 0 des Schwingers wird der Punkt betrachtet, in dem der Drache an der Feder hängt, ohne zu schwingen. Die Masse der Feder wird vernachlässigt.
Im folgenden Diagramm wurde für drei Federn die Abhängigkeit der Verlängerung von der anhängenden Masse grafisch dargestellt:


![Graph](https://physikaufgaben.de/bild/a1348_1.png)

</p>

---

1. 1. Begründen Sie, dass Feder 1 und 2 grundsätzlich für den Drachen verwendet werden können, Feder 3 jedoch nicht verwendet werden sollte.

<details style="margin-left:10%">

<summary> Lösung </summary>

Laut Aufgabenstellung soll der Drachen harmonisch schwingen. Das sieht einfach besser aus.
Damit er harmonisch schwingt, muss die @color(rücktreibende Kraft proportional zur Auslenkung der Feder, red) sein. (lineares Kraftgesetz)
Das ist bei Feder 1 und 2 der Fall. Über die gesamte Ausdehnung ist die Ausdehnung proportional zur Masse und somit auch zur Gewichtskraft.
Bei Feder 3 ist das bis zur Masse von 500 g auch der Fall. Im oberen Bereich, den die Feder auf Grund der Schwingung ja auch erreichen wird, liegt aber keine Proportionalität vor. Die Feder dehnt sich bei steigender Belastung deutlich mehr aus als bei geringer Belastung.

</details>

---


1. 2. Berechnen Sie die Federkonstanten für Feder 1 und 2.

<p style="margin-left:10%">

@rangeQuiz2($D_1$, 29.43 , $\dfrac{N}{m}$)

@rangeQuiz2($D_2$, 9.81 , $\dfrac{N}{m}$)

</p>

---

1. 3. Der Drache soll eine möglichst große Schwingungsdauer haben, damit seine Bewegung deutlich sichtbar ist. Prüfen Sie, welche der Federn 1 oder 2 sich in dieser Hinsicht besser eignet. Begründen Sie Ihre Antwort. 

<details style="margin-left:10%">

<summary> Lösung </summary>

Die Schwingungsdauer einer Feder berechnet sich mit $T=2\pi\sqrt{\frac{m}{D}}$.<br>
Der Wunsch ist es, das die Schwingungsdauer möglichst groß ist. Das heißt, die Federkonstante sollte möglichst klein sein. D steht in der Gleichung unter dem Bruchstrich. Damit wird T immer größer, je kleiner D wird.
Es ist also die Feder 2 geeignet.
Die Feder ist im Vergleich zu Feder 1 weicher und schwingt dadurch langsamer.

</details>


---

> Verwenden Sie für weitere Berechnungen die Feder 2 mit $D_2=10\frac{N}{m}$ formel. Die Dämpfung der Drachenschwingung wird zunächst vernachlässigt.

1. 4. Der Drache wird zu Beginn um 5 cm nach unten ausgelenkt und dann losgelassen Berechnen Sie die maximale Geschwindigkeit des Drachens während seiner Bewegung.

<p style="margin-left:10%">

@rangeQuiz2($\hat{v}$, 0.224 , $\dfrac{m}{s}$)

</p>

<details style="margin-left:10%">

<summary> Lösung </summary>

Die Geschwindigkeit des Drachen ist in der Gleichgewichtslage am größten.

Da der Drache zunächst ausgelenkt wird, kann die Elongation $y(t)$ mit dem $\cos$ beschrieben werden.

$y(t) = \hat{y} \cdot \cos(\omega \cdot t)$

Für die Geschwindigkeit $v(t)$ ergibt sich

$v(t) = -\hat{v} \cdot \sin(\omega \cdot t)$

mit

$\hat{v} = \hat{y} \cdot \omega = 0,05m \cdot \sqrt{\frac{D}{m}}$

$ \underline{\hat{v} = 0,224 \frac{m}{s}}$

</details>

---

1. 5. Der Drache soll als Blickfang dienen und daher ununterbrochen schwingen. Dafür wird ein Motor eingesetzt, der bei jeder Umdrehung die Aufhängung der Feder kurz nach oben beschleunigt. Geben Sie an, bei welcher Drehzahl (in Umdrehungen je Minute) der Drache seine maximale Amplitude erreicht. Begründen Sie Ihre Aussage.


<p style="margin-left:10%">

@rangeQuiz2($\dfrac{N}{t}$, 42.6 , $\dfrac{1}{min}$)

</p>

<details style="margin-left:10%">

<summary> Lösung </summary>

Die Schwingung der Feder muss immer zum richtigen Zeitpunkt unterstütz werden, um Verluste durch die Reibung auszugleichen. Dazu muss durch den Motor periodisch Energie zugeführt werden. <br> Das geht am besten, wenn die Erregerfrequenz durch den Motor genau so groß wie die Eigenschwingung der Feder ist. Beide müssen in Resonanz schwingen. <br>
Die Zeit für eine Motorumdrehung muss dann genau so groß sein wie die Schwingungsdauer des Pendels. <br>
Aus der oben berechneten Frequenz ergibt sich eine Schwingungsdauer von 1,4 s. Der Motor muss sich also so drehen, dass er für eine Umdrehung 1,4 s benötigt. <br>
Das sind dann 0,71 Umdrehungen in einer Sekunde oder 42,6 Umdrehungen in einer Minute.

</details>

---

2. [Hängebrücke](https://www.leifiphysik.de/mechanik/kopplung-von-schwingungen/aufgabe/haengebruecke)

---

3. [Wagen-zwischen-zwei-Federn](https://www.leifiphysik.de/mechanik/kopplung-von-schwingungen/aufgabe/wagen-zwischen-zwei-federn)

### Theorie der Resonanz (***)

??[Mathematische-Aufgabe-zur-Resonanz](https://www.max-academy.de/contentPlayer/61bb2cbc3542e200665ee644/61bb30e13542e200665eeaef)


### Aufgabe Harmonische Schwingung

![Bild1](https://diversewolken.ddns.net/nextcloud/index.php/s/y3iM42qsbe25xb7/download)Bei der Erdölsuche am Nordpol wurde versehentlich ein Bohrloch durch den Mittelpunkt der Erde zum Südpol gebohrt (geht das?). Ein sehr dünner britischer Geologe fällt zur Zeit $t = 0$ in das Bohrloch und schreit sofort um Hilfe. Bei den folgenden Betrachtungen ist die Luftreibung zu vernachlässigen. Die Schallgeschwindigkeit ist c = 333 m/s.<br>
r: Abstand des Geologen vom Erdmittelpunkt;<br>
R: Erdradius $6,37\cdot10^3 km$<br>
M: Erdmasse $5,98\cdot10^{24} kg$<br>
m: Masse des Geologen $55 kg$

Die Gravitationskraft, die auf den Geologen wirkt, hängt wie folgt vom Abstand Erdmittelpunkt $r$ ab: $$F = - G \cdot \frac{M \cdot m}{R^3} \cdot r$$

1. Welchen Bewegungstyp führt der Geologe aus (Begründung)? Berechnen Sie die charakteristischen Größen der Bewegung und geben Sie die Bewegungsgleichung an.

<p style="margin-left:10%">

@rangeQuiz2($T$, 5.06e3 , $s$)

</p>

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_1](https://diversewolken.ddns.net/nextcloud/index.php/s/dpnEAzyBEGnkE4p/download)

</details>

---

2. Nach welcher Zeit $t_1$ kommt der Geologe am Südpol an?

<p style="margin-left:10%">

@rangeQuiz2($t$, 42 , $min$)

</p>

<details style="margin-left:10%">

<summary> Lösung3 </summary>

![Lsg_2](https://diversewolken.ddns.net/nextcloud/index.php/s/mCikdJekxSWQYmf/download)

</details>

---

3. Ermitteln Sie den Geschwindigkeitsbetrag des Geologen beim Passieren des Erdmittelpunkts.

<p style="margin-left:10%">

@rangeQuiz2($v$, 7.9e3 , $\dfrac{m}{s}$)

</p>

<details style="margin-left:10%">

<summary> Lösung3 </summary>

![Lsg_3](https://diversewolken.ddns.net/nextcloud/index.php/s/7fqB26ECJX9Aj68/download)


</details>

---

4. Ermitteln Sie den Zeitpunkt, an welchem der Geologe seinen Hilferuf das erste Mal überholt.

     __Hinweise:__ Bei der Lösung des zweiten Zeitpunktes kann $cos(x)$ näherungsweise durch den Ausdruck $1-\frac{x^2}{2}$ ersetzt werden.

<p style="margin-left:10%">

@rangeQuiz2($t$, 68 , $s$)

</p>

<details style="margin-left:10%">

<summary> Lösung4 </summary>

![Lsg_4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/YCxmpkFo8NbkmDf/download)

![Lsg_4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/mCikdJekxSWQYmf/download)

</details>



### Aufgabe Spielkonsole

![Skizze-Spielkonsole](https://diversewolken.ddns.net/nextcloud/index.php/s/wKS48wrDdHBqy2R/download)<!-- style="max-height:200px" --> In der Fernbedienung einer Spielekonsole ist ein Beschleunigungs­sen­sor eingebaut, der die Beschleunigung in vertikaler Richtung misst. Die Fernbedienung hat die Masse 300 g und hängt an einer Feder mit vernachlässigbarer Masse (siehe Abb. 1). Nachdem die Fernbedienung nach unten ausgelenkt und zum Zeitpunkt 0 s los­gelassen wurde, schwingt sie harmonisch. Ihre Signale werden von einem Computer erfasst und ausgewertet. Es ergeben sich unten dargestellte Messwerte. 

__Messwerte:__

![Messwerte](https://diversewolken.ddns.net/nextcloud/index.php/s/NpcGbBgmz9aqNzA/download)

1. Zeichnen Sie das zugehörige Zeit-Beschleunigungs-Diagramm.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg-1](https://diversewolken.ddns.net/nextcloud/index.php/s/KnoRnn5CbCMYAGb/download)

</details>

---

2. Ermitteln Sie daraus die Schwingungsdauer.

<p style="margin-left:10%">

@rangeQuiz2($T$, 1.6 ,$s$)

</p>

3. Geben Sie eine Funktionsgleichung für die Beschleunigung a(t) an.

<details style="margin-left:10%">

<summary> Lösung </summary>

$$ \omega = \frac{2\pi}{T} = 3,39 \frac{1}{s} $$

$$ a(t) = \hat{a} \cdot \cos(\omega \cdot t) = 4,6m \cdot \cos(3.93 \frac{1}{s} \cdot t) $$

</details>

---

4. Bestimmen Sie, zu welchen Zeitpunkten im Intervall zwischen 0 s und 1,5 s der Geschwindigkeitsbetrag der Fernbedienung maximal ist.

<p style="margin-left:10%">

@rangeQuiz2($t_{v_{max}1}$, 0.4 ,$s$)

@rangeQuiz2($t_{v_{max}2}$, 1.2 ,$s$)

</p>

---

5. Berechnen Sie die maximale Auslenkung und die maximale Geschwin­digkeit.

<p style="margin-left:10%">

@rangeQuiz2($y_{max}$, 0.298 ,$m$)

@rangeQuiz2($v_{max}$, 1.17 ,$\frac{m}{s}$)

</p>

---

6. Berechnen Sie die Federkonstante.

<p style="margin-left:10%">

@rangeQuiz2($D$, 4.63 ,$\frac{N}{m}$)

</p>

| | | | | | | |
| $t$ in $s$ | 0,0 | 0,2 | 0,4 | 0,5 | 0,7 | 1,0 |
| $a$ in $\frac{m}{s^2}$ | 4,60 | 3,25 | 0,00 | –1,76 | – 4,25 | –3,25 |

## 9. 10. Grundlagen Elektromagnetischer Schwingkreis

__Aufbau:__

<p class="newspaper">

> Elektromagnetische Schwingungen spielen in der modernen Elektronik eine entscheidende Rolle. Ein elektromagnetischer Schwingkreis besteht aus einer Parallelschaltung von einem __Kondensator (Kapazität $C$)__ und einer __Spule(Induktivität $L$)__. 

{{2}}
*********
> _Hinweis: Der Kondensator kann durch einen Wechselschalter von einer Spannungsquelle aufgeladen werden._
*********

<p class="cb">

{{1-2}}
**********
![Schaltkreis-Schwingkreis](https://diversewolken.ddns.net/nextcloud/index.php/s/geHrqMrBJmkFCo6/download)
**********

{{2}}
**********
![Schaltkreis-Schwingkreis](https://diversewolken.ddns.net/nextcloud/index.php/s/Wy3j3A8ekemEy3e/download)
**********

</p>

</p>

{{3}}
**********
      -> [Falstad-Simulation-AC-Circut](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcMBMcUHYMGZIA4UA2ATmIxAUgoqoQFMBaMMAKCA)

<p style="margin-left:10%">

__Aufgaben:__

1. Übernehmen Sie das Tafelbild

2. Öffnen Sie die Simulation

3. Stoppen Sie die Simulation mit dem Schalter Run/STOP

4. Erstellen Sie mit Hilfe der Simulation einen idealen Schwingkreis (siehe Schaltkreis)

<details style="margin-left:10%">

<summary> Beispiel-Lösung </summary>

![Lösung](https://diversewolken.ddns.net/nextcloud/index.php/s/kionyaX8epZXkeB/download)

</details>

4. Beobachten Sie die entstehende Schwingung in dem sie den Schalt auf Laden stellen, anschließend die Simulation starten und dann den Schwinkreis schließen

5. Stellen Sie eine Vermutung auf, welche physikalische Eigenschaft/Einheit hier eine Schwingung durchführt

6. Fügen Sie eine Messung hinzu. 

__Shortcuts:__

- Leertaste -> Auswählen

- w -> Verbindung / Kabel

- r -> Widerstand

- L -> Spule

- c -> Kondensator

- v -> Spannungsquelle

- S -> Wechselschalter

</p>

**********

## 9. 11. Herleitung der Periodendauer am idealen Schwingkreis

![ThomsonSG-HL-1](https://diversewolken.ddns.net/nextcloud/index.php/s/bgB97f49sZ2dqLM/download)

![ThomsonSG-HL-2](https://diversewolken.ddns.net/nextcloud/index.php/s/cod9taS83dYzocg/download)

![ThomsonSG-HL-3](https://diversewolken.ddns.net/nextcloud/index.php/s/98Q3m4yFHzSeR76/download)

![ThomsonSG-HL-4](https://diversewolken.ddns.net/nextcloud/index.php/s/sqaFGGczrS2F97f/download)


## 9. 12. Energiebetrachtungen am Schwingkreis

__Energiebetrachtung__

> In einem idealen Schwingkreis schwingt die Energie zwischen dem [[ elektrischen ]] Feld des Kondensators ([[ elektrische ]] Energie) und dem magnetischen Feld der Spule ([[ magnetische ]] Energie). Die Summe aus elektrischer und magnetischer Energie ist zu jedem Zeitpunkt [[ konstant ]].

{{1}}
**********
<p class="newspaper">

__Im Kondensator gespeicherte elektrische Energie__

$\boxed{E_{el}(t) = \frac{1}{2} \cdot C \cdot U^2(t)}$

<p class="cb">

__Im Magnetfeld der Spule gespeicherte Energie__

$\boxed{E_{mag}(t) = \frac{1}{2} \cdot L \cdot I^2(t)}$

</p>

</p>

**********

{{2}}
**********
__Idealer vs. realer Schwingkreis__

Bei einem realen Schwingkreis wird der elektrische Widerstand der Kabel (z.B. der Spule) berücksichtigt. Die im Schwingkreis gespeicherte Energie wird nach und nach in Form von Wärme abgegeben.
**********


### Abituraufgabe zum Schwingkreis (Abitur BY 2018 Ph11-1 A2)

<p class="newspaper">

Bestimmte Warensicherungsetiketten enthalten einen elektromagnetischen Schwingkreis mit der Eigenfrequenz $8,2\,\mathrm{MHz}$. Der Schwingkreiskondensator besteht aus zwei Platten im Abstand $15\,\mathrm{\mu m}$. Die Plattenfläche (in Abb. 1 grau dargestellt) beträgt ca.  $13\,\mathrm{\%}$
 der Gesamtfläche des Warensicherungsetiketts. Der Raum zwischen den Platten ist mit Polypropylen gefüllt, wodurch sich die Kapazität des Kondensators um den Faktor $\varepsilon_r=2,3$ gegenüber der eines luftgefüllten Kondensators erhöht. Aufgrund einer eingebauten Soll-Kurzschlussstelle wird der Kondensator zerstört, wenn die Plattenspannung einen Wert von $4,5\,\mathrm{V}$ übersteigt.

<p class="cb">

![Abi2018](https://www.leifiphysik.de/sites/default/files/2018/12/image/warensicherung_aufgabe_bild_1.svg "Abb. 1: Etikett zur Warensicherung")

</p>

</p>

- a) Bestimme mithilfe der Abb. 1 (im Original hat das quadratische Warensicherungsetikett die Kantenlänge 35 mm) die Induktivität der Spule.

<p style="margin-left:10%">

@rangeQuiz2($C$, 2.2E-10, F )

@rangeQuiz2($L$,1.7e-6, H)

</p>


<details style="margin-left:10%">

<summary> @color(__Lösungshinweise__, blue) </summary>

> Ermittlen Sie zunächst den Flächeninhalt des Kondensators. Nutzen Sie anschließend die Formeln zur Berechnung der Kapazität eines Plattenkondensators zur Bestimmung von C.
>
> Anschließend ermitteln Sie die Periodendauer der Eigenschwingung und daraus die Induktivität der Spule.

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![Abi18_SK_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/DKbH9koHRozMn6K/download)

</details>

</details>

---

- b) Berechne die maximale Energie, die der Schwingkreis aufnehmen kann, ohne zerstört zu werden

<p style="margin-left:10%">

@rangeQuiz2($E_{max}$, 2.2E-9, J )

</p>

<details style="margin-left:10%">

<summary> @color(__Lösungshinweise__, blue) </summary>

> Überlegen Sie zunächst, welcher Maximalwert/Grenzwert im Aufgabentext für eines der Bauelemente gegeben ist.
>
> Ermitteln Sie nun mit diesem Grenzwert die im Bauelement gespeicherte Energie.

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

> ![Abi18_SK_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/BkPWA6gny4sc6nK/download)

</details>

</details>

---

<p class="newspaper">

Warenhäuser besitzen am Ausgang Schleusen, die aus einer Sendespule S und einer Empfangsspule E in einem Abstand von ca. einem Meter bestehen (vgl. Abb 2). An die Sendespule wird eine sinusförmige Wechselspannung der Frequenz $f$ angelegt.

<p class="cb">

![Schleuse](https://www.leifiphysik.de/sites/default/files/2018/12/image/warensicherung_aufgabe_bild_2.svg "Abb. 2: Schleuse")<!-- style="max-height:300px"-->

</p>

</p>

---

- c) Erkläre, dass ein an E angeschlossenes Messgerät eine Wechselspannung anzeigt.

<details style="margin-left:10%">

<summary> @color(__Lösung__, blue) </summary>

> Die Wechselspannung an der Sendespule S erzeugt ein magnetisches Wechselfeld, das auch die Empfängerspule durchsetzt. Nach dem Induktionsgesetz tritt aufgrund der Änderung des magnetischen Flusses in der E eine Induktionsspannung auf, die vom Messgerät angezeigt wird.

</details>

---

<p class="newspaper">

Befindet sich eine Ware mit intaktem Sicherungsetikett in der Schleuse, so nimmt der Schwingkreis Energie auf, wenn die Frequenz $f$ mit seiner Eigenfrequenz übereinstimmt. Man beobachtet dann ein Absinken des Scheitelwerts $U_E$ der bei E gemessenen Wechselspannung. Größere Metallgegenstände führen ebenfalls zu einem Absinken von $U_E$ und können einen Fehlalarm auslösen. Um dies zu vermeiden, wird der Sender so eingestellt, dass die Frequenz periodisch um den Mittelwert $8,2\,\mathrm{MHz}$ schwankt (siehe Abb. 3).

<p class="cb">

![Wechselfrequenz](https://www.leifiphysik.de/sites/default/files/2018/12/image/warensicherung_aufgabe_bild_3.svg "Abb. 3: Sendesignal")

</p>

</p>

---

- d) In der Schleuse befinden sich <br> <br> α) ein intaktes Sicherungsetikett -> Zuordnung Diagramm: [[ 1 | 2 | 3 | (4) ]] <br> <br> β) ein größerer Metallgegenstand -> Zuordnung Diagramm: [[ 1 | 2 | (3) | 4 ]] <br> <br> Ordne den beiden Fällen je eines der Diagramme 1 bis 4 aus Abb. 4 passend zu. Begründe deine Entscheidung. 

<details style="margin-left:10%">

<summary> @color(__Lösungshinweise__, blue) </summary>

> Überlegen Sie zunächst, welchen Einfluss das äußere Wechselfeld auf das Etikett hat (Stichwort _Resonanz_). Achten Sie auf die Zeitskala der Frequenzänderung und schlussfolgern Sie auf das Signal am Empfänger.
> 
> Wiederholen Sie Ihre Überlegungen für das Metallstück (Stichwort _Induktion_)

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

> Zu α): Wenn sich ein intaktes Sicherungsetikett zwischen den Spulen S und E befindet, dann stellt das Diagramm 4 die Verhältnisse richtig dar: Immer dann, wenn Frequenz der Spannung $U_s$ an der Sendespule die Resonanzfrequenz des Schwingkreises im Sicherungsetikett erreicht, nimmt der Schwingkreis Energie auf. Dies ist im betrachteten Zeitraum von [0 ms - 4ms] fünfmal der Fall. Die Energieaufnahme des Schwingkreises führt dazu, dass die Spannung an der Empfängerspule im betrachteten Zeitraum fünfmal abnimmt.
>
> Zu β): Wenn sich ein größerer Metallgegenstand zwischen den Spulen S und E befindet, dann stellt das Diagramm 3 die Verhältnisse am besten dar: Im Metallgegenstand erzeugt das magnetische Wechselfeld Wirbelströme, deren Intensität kaum von der Frequenz der Spannung $U_S$ der Sendespule abhängt. Die induzierte Spannung in der Empfängerspule schwankt im Takt von $U_S(t)$. Aufgrund der Energieverluste im Metallstück liegt jedoch der Betrag der in der Empfängerspule induziert Spannung stets unter den entsprechenden Werten, die ohne das Metallstück festzustellen wären.

</details>

</details>

![Diagramme](https://www.leifiphysik.de/sites/default/files/2018/12/image/warensicherung_aufgabe_bild_4.svg)<!--  style="max-width=200px" -->

---

- e) Beim Bezahlvorgang werden die Etiketten an der Kasse kurz einem magnetischen Wechselfeld $$B(t)=5,8\,\mathrm{\mu T}\cdot\sin(2\pi\cdot 16\,\mathrm{MHz}\cdot t)$$ ausgesetzt. <br> <br> Bestimme aus Abb. 1 (im Original hat das "Quadrat" der äußeren Windung die Kantenlänge 30 mm und das Quadrat der inneren Windung die Kantenlänge 22 mm)  näherungsweise die mittlere Querschnittsfläche sowie die Windungszahl der zweilagigen Schwingkreisspule.<br> <br> Berechne damit den Maximalwert der darin induzierten Spannung. <br><br>  Begründe, dass das Etikett deaktiviert wird.

<p style="margin-left:10%">

@rangeQuiz2($N_{sp}$, 14 , .)

@rangeQuiz2($A_{sp}$, 6.8e-4, m² )

@rangeQuiz2($\hat{U}_{ind}$, 5.5, V )

</p>


<details style="margin-left:10%">

<summary> @color(__Lösungshinweise__, blue) </summary>

> __Für die Windungszahl__ können Sie Abb. 1 nutzen und die Windungszahl zählen. Achten Sie darauf, dass die Spule doppellagig ist.
> 
> __Für die Querschnittsfläche__ nutzen Sie die mittle Seitenlänge der Spule.
>
> Nutzen Sie __für die Induktionsspannung__ das Induktionsgesetz (LB 8).
>
> Überprüfen Sie, ob die induzierte Spannung die Grenzwerte überschreitet.

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

> ![Abi18_SK_Lsg_e](https://diversewolken.ddns.net/nextcloud/index.php/s/wonHnPGescAe4YE/download)

</details>

</details>

## 9. 13. Simulation eines idealen Schwingkreises


Für die Simulation eines idealen Schwingkreises wird die Simulationssoftware Moebius verwendet

__A. Formelgrundlage für die Simulation__

> 1. Spannung am Kondensator
>
> $$ U_C = \frac{Q}{C} $$
>
> 2. Maschenregel (Spannungsgleichheit an Kondensator und Spule)
>
> $$ U_L = - U_C $$
>
> 3. Spannung an einer Spule 
> 
> $$ U_L = L \cdot \frac{\mathrm{d}I}{\mathrm{d}t} $$
>
> 4. Ladung und Stromstärke
> 
> $$ I = \frac{\mathrm{d}Q}{\mathrm{d}t} $$


> @color(__Erstellen Sie aus diesen Gleichungen den Simulationscode. Nutzen Sie die Hinweise wenn nötig.__, blue)


<details>

<summary> __B. Hinweise zum Simulationscode__  </summary>

- Gleichung 1. können wir direkt verwenden

- Gleichung 2. können wir direkt verwenden

- Gleichung 3. muss nach $\mathrm{d}I$ umgestellt werden

- Gleichung 4. muss nach $\mathrm{d}Q$ umgestellt werden

- aktualisieren Sie anschließend die Ladung ($Q=Q+\mathrm{d}Q$), die Stromstärke ($I=I+\mathrm{d}I$) und die Zeit ($t=t+\mathrm{d}t$)

</details>


---
<details>

<summary> __C. Hinweise: Hinweise zu den Anfangsbedingungen (t=0)__ </summary>

- Wählen Sie für Ihre erste Simulation als Kapazität $C=0,1\,\mathrm{F}$ und als Induktivität $L=1\,\mathrm{H}$. 

- Als Startwert für die Ladung können Sie $Q=1\,\mathrm{C}$ verwenden. 

- Nutzen Sie $\mathrm{d}t = 0,001$ bei $5000$ Wiederholungen.

</details>

---

<details>

<summary>__D. Überprüfung der Simulation__</summary>

- ermitteln Sie die Periodendauer für Ihren Schwingkreis aus der Thomson'schen Schwingungsgleichung (siehe 9.11).

<p style="margin-left:10%">

@rangeQuiz2($T$,1.987,s)

</p>

- vergleichen Sie die Periodendauer mit Ihrer Simulation

<details style="margin-left:5%">

<summary> Lösung $U_C(t)$ </summary>

![Lsg_Schwingkreis_C0.1_L1_Q1](https://diversewolken.ddns.net/nextcloud/index.php/s/KZw5b5P6swPGC76/download)

</details>

</details>


---

<details>

<summary> __E: Lösung Code__ </summary>

``` 

PROGRAMM: (IdealerSchwingkreis)
Uc=Q/C
UL=-Uc

dI = UL/L*dt
dQ=I*dt

Q=Q+dQ
I=I+dI
t=t+dt


```

</details>

---

<details>

<summary> __F: Realer Schwingkreis__ </summary>

Bei einem realen Schwingkreis wird der elektrische Widerstand $R$ des Kabels berücksichtigt. Als Ersatzschaltbild können Sie folgende Simulation mit einem Widerstand $R=0,5\,\Omega$ ($C=0,1\,\mathrm{F}$, $L=1\,\mathrm{H}$) betrachten. Mit dem _Reset Button_ starten Sie die Simulation von vorn (der Kondensator erhält eine initiale Spannung von $10\,\mathrm{V}$).

@color(Aufgabe: Ergänzen Sie den Einfluss eines ohmschen Widerstands in Ihrem Simulationscode., blue)

??[Schwingkreis-C0.1-L1-R0.5](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l5YCcyWrQDhAZnQJmgOwBsuArHmACxbKRGUiUEikuQsCmAtGGAFABjELnSYqDEZiyQGDGBC4wmlRJSLoaM4qWpZw7eXwA22dA3GmG0ueBCLoRMDXQFEWMBtK4CHqHwDuwqLglFZmIXJ8AE5BUjKW2PEG0KR8APZQ+rg2lJCIYskQ7LiZWHxAA)

</details>



## Entwicklung Leistungen 12Ph2

![Ergebnisse_12LK1](https://diversewolken.ddns.net/nextcloud/index.php/s/osbmD6jHeg77cEo/download)

{{1}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend |
| ---- | ---- | ---- |
| 11/LK1 | 7.9 | 8.07 |
| 11/KA1 | 6.3 | 8.27 |
| 11/EX1 | 11.9| 8.47 |
| 11/KA2 | 7.7 | 8.67 |
| 11/LK2 | 8.8 | 8.87 |
| 11/KA3 | 8.7  | 9.07 |
| 11/KA4 | 9.1 | 9.27 | 
| 11/EX2 | 10.5 | 9.47 |
| 12/LK1  | 8.9 | 9.67 |
*********



{{2}}
*************

<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Note"
     data-transpose
-->
|	|LK1	|KA1	|KA2	|LK2	|KA3	|KA4 | EX2 | LK3 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|1	|6	|2	|5	|8	|10	|7 | 10 | 5 |
|2	|6	|5	|4	|8	|9	|9 | 11 | 5 |
|3	|9	|6	|9	|6	|10	|11 |11 | 11 |
|4	|9	|8	|10	|9	|5	|6 | 8  | 8 |
|5	|6	|3	|4	|5	|7	|5 | 8  | 6 |
|6	|8	|6	|8	|6	|6	|8 | 8  | 7 |
|7	|9	|3	|7	|11	|12	|14 |9  | 11 |
|8	|7	|3	|7	|7	|5	|8 | 12 | 8 |
|9	|3	|4	|6	|8	|10	|2 | 12 | 9 |
|10	|9	|3	|9	|11	|8	|10 |9  | 12 |
|11	|13	|12	|15	|15	|14	|14 |15 | 13 |
|13	|11	|7	|9	|10	|10	|12 |14 | 10 |
|14	|11	|12	|14	|15	|15	|15 |14 | 14 |
|15	|9	|12	|6	|8	|3	|9 | 10 | 5 |

*************

## 9. 14. Berechnungen an einem schwach gedämpften Schwingkreis

Für eine schwachte Dämpfung kann die Schwingung an einem gedämpften Schwingkreis mit der Formel:


> $ Q(t) = \hat{Q} \cdot \cos(\omega\,t) \cdot e^{-\delta\,t} $


in guter Näherung beschrieben werden. Hierbei beschreibt der Faktor $\delta$ die Dämpfung, hervorgerufen durch den elektrischen Widerstand $R$:

> $ \delta = \frac{R}{2L}$

Die (leicht veränderte) Kreisfrequenz $\omega$ für den schwach gedämpften Fall wird ermittelt mit

> $ \omega = \sqrt{\omega_0^2-\delta^2}$ mit $\omega_0 = \sqrt{\frac{1}{L\cdot C}}$


---

1. Erfragen Sie bei der Lehrkraft eine Spule und einen Kondensator. Ermitteln Sie folgende Werte anhand der Angaben auf den Bauelementen.

<p style="margin-left:10%">

@rangeQuiz2($C$,20e-6,F)

@rangeQuiz2($R$,19,$\Omega$)

</p>

2. Die Spule wird mit einem O-förmigen Eisenkern genutzt. Der aufgedruckte Wert gilt allerdings ohne Eisenkern. Um die Induktivität zu ermitteln wurde an die Spule eine Wechselspannung mit Netzfrequenz angeschlossen. Dabei wurden folgende Werte für Spannung und Stromstärke ermittelt. <br><br> $U_\sim = 7\,\mathrm{V}$ <br> $I_\sim = 0,01\,\mathrm{A}$ <br> <br> Ermitteln Sie aus diesen Angaben die Induktivität der Spule mit O-förmigem Eisenkern. Ermitteln Sie ebenfalls die magnetische Permeabilität des Eisenkerns.

<p style="margin-left:10%">

@rangeQuiz2($L$, 2.23 ,H)

@rangeQuiz2($\mu_r$, 97 , .)

</p>

<details style="margin-left:10%">

<summary> Hinweis Induktivität </summary>

Nutzen Sie die Formel für den Wechselstromwiderstand $Z$ einer Spule in einem Wechselstromkreis (s. Kapitel 8.1.4).

</details>

---

4. Weiterhin wird eine Ladespannung gegeben: <br><br> $U_0 = 7\,\mathrm{V}$ <br><br> Ermitteln Sie aus den gegebenen Werten die folgenden Größen der Schwingung.

<p style="margin-left:10%">

@rangeQuiz2($\hat{Q}$,0.00014,C)

@rangeQuiz2($T$, 41.96e-3 ,s)

@rangeQuiz2($\omega_0$,149.73,$\mathrm{\frac{1}{s}}$)

@rangeQuiz2($\delta$,4.27,$\mathrm{\frac{1}{s}}$)

_Hinweis: Für eine schwache Dämpfung, wie es in diesem Beispiel der Fall ist, gilt $\omega\approx\omega_0$._

</p>

---


5. Geben Sie die ermittelten Werte in Ihre Simulation ein. Lassen Sie sich den $U(t)$-Graph am Kondensator für das Zeitintervall 0-100ms ausgeben. <br> Wählen Sie $\mathrm{d}t$ so, dass sie 10'000 Zeitschritte simulieren. <br> Erstellen Sie ein PDF Dokument aus Ihrer Simulation, benennen Sie das PDF um und laden Sie Ihr Simulationsergebnis [hier hoch](https://diversewolken.ddns.net/nextcloud/index.php/s/z89P4CzGHWXjaHt). <br> @color(Lassen Sie sich Ihre Ergebnis ausdrucken und fügen Sie die Simulation Ihren Unterlagen hinzu., blue)


<details style="margin-left:10%">

<summary> Lösung </summary>

![LösungSimulation](https://diversewolken.ddns.net/nextcloud/index.php/s/kX7qNxFqGTkM8i7/download)
</details>


---

6. (*)Zeichnen Sie mit Geogebra die Funktion $U(t)$ mit den gegebenen Werten. Vergleichen Sie die mathematische Beschreibung mit der Simulation. <br> <br> [Geogebra-U(t)](https://www.geogebra.org/classic/c66r2prv)

<details style="margin-left:10%">

<summary> Lösung </summary>

<iframe src="https://www.geogebra.org/classic/kb4kwfgq?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

</details>

## 9. 15. Experiment: Schwach gedämpfter Schwingkreis

<p style="color:blue">

Nehmen Sie experimentell die Spannungsfunktion $U(t)$ für einen gedämpften Schwingkreis auf. <br> <br> __Machen Sie sich zu Ihrem Experiment Notizen.__ <br> <br>

</p>

1. Bauen Sie den Schaltkreis anhand des Schaltplans auf. <br> ![Schaltkreis-Schwingkreis](https://diversewolken.ddns.net/nextcloud/index.php/s/Wy3j3A8ekemEy3e/download)

2. Ergänzen Sie das Cassy-Messgerät zur Bestimmung der Spannungsfunktion. <br> @color(Lassen Sie sich Ihren Schaltkreis abnehmen., red)

3. Verbinden Sie einen Laptop mit dem WLan des Cassy-Messgerätes.

3. Entnehmen Sie aus Ihrer Simulation die gesamte Messzeit. Stellen Sie die Messzeit ein und wählen Sie ebenfalls ein sinnvolles Messintervall und eine sinnvolle Triggereinstellung zum Start der Messung.

4. Nehmen Sie mit Hilfe des Cassy-Messgerätes die gedämpfte Schwingung auf.

5. Erstellen Sie ein PDF aus Ihrer Messung und benennen Sie das PDF mit Ihrem Namen. Laden Sie das PDF [hier hoch](https://diversewolken.ddns.net/nextcloud/index.php/s/z89P4CzGHWXjaHt) (Laptop muss mit dem Internet verbunden werden). <br> @color(Lassen Sie sich Ihre Ergebnis ausdrucken und fügen Sie Ihr experimentelles Ergebnis Ihren Unterlagen hinzu., blue).

6. Vergleichen Sie die Simulation mit der Messung.

## 9. 16 Vergleich von Simulation und Experiment - Gedämpfter Schwingkreis

{{0-1}}
*********
<p class="newspaper">

__Messung__

![U-t-Messung](https://diversewolken.ddns.net/nextcloud/index.php/s/a4aQqEHPEXq8Gok/download)

<p class="cb">

__Simulation__

![U-t-Simulation](https://diversewolken.ddns.net/nextcloud/index.php/s/RiZ6J7HssJfMff9/download)

</p>

</p>
*********

{{1}}
*********
![U-t-Sim-Mes](https://diversewolken.ddns.net/nextcloud/index.php/s/cDAtBsYj7GaZLr2/download)
*********

__Vergleich:__

{{2}}
***********
- gedämpfte Schwingung ist in beiden Fällen sichtbar, Periodendauer wird von der Simulation zu Beginn gut wiedergegeben
***********

{{3}}
***********
- Dämpfung ist im Experiment deutlich größer als in Simulation

     -> d.h. Amplitude der Messung nimmt stärker ab, als erwartet
***********

{{4}}
***********
- Periodendauer scheint sich während der Messung zu verringern, was bei der Simulation nicht zu beobachten ist
***********

__Deutung der Beobachtung:__

{{5}}
***********
- tatsächliche Dämpfung wird von der Simulation nicht berücksichtigt

- zeitliche Abhängigkeit der Größen L bzw. C möglich (L und/oder C sinken)
***********

__Physikalische Erklärung:__

{{6}}
***********
- ?? -> bitte mal nachdenken
***********

### Übung Schwach Gedämpfter Schwingkreis (LEIFI)

Im Unterricht soll der zeitliche Verlauf der Spannung in einem elektromagnetischen Schwingkreis aufgezeichnet werden. Dafür stehen unter anderem ein Kondensator mit der Aufschrift $C=40\,\mathrm{µF}$, eine Spule der Induktivität $L=630\,\mathrm{H}$, eine Gleichspannungsquelle, ein Schalter sowie ein geeignetes Spannungsmessgerät zur Verfügung.

<p style="margin-left:5%">

a) Zeige, dass für den Schwingkreis eine Periodendauer von $T=1\,\mathrm{s}$ zu erwarten ist. 

<details>

<summary> Lösung </summary>

![Loesung_a](https://diversewolken.ddns.net/nextcloud/index.php/s/5Ngo4qfT6CabSSf/download)

</details>

---

b) Aus der Messung erhält man den abgebildeten Spannungsverlauf.

![Spannungsverlauf](https://www.leifiphysik.de/sites/default/files/2018/12/image/reale_elektromagnetische_schwingung_bild_1.svg)

Bestimme mithilfe des Diagramms einen möglichst genauen Wert für die im Versuch aufgetretene Periodendauer. [zur Kontrolle: $T=0,95\,\mathrm{s}$]

<details>

<summary> Lösung </summary>

![Loesung_b](https://diversewolken.ddns.net/nextcloud/index.php/s/qwn4cr7PnjfYrJd/download)

</details>

---

c) Ein Schüler vermutet, dass der ohmsche Widerstand $R$ der Spule für die Abweichung zwischen den beiden Werten verantwortlich ist. Er findet in einer Formelsammlung für die Frequenz $f$ eines gedämpften elektromagnetischen Schwingkreises die Formel

$$f= \frac{1}{2\pi}\sqrt{\frac{1}{L\cdot C}-\Big(\frac{R}{2L}\Big)^2}$$

Die im Versuch verwendete Spule hat einen Widerstand von $R=280\,\Omega$.

Zeige rechnerisch, dass der Unterschied zwischen den Werten nicht auf den Spulenwiderstand zurückgeführt werden kann.

<details>

<summary> Lösung </summary>

![Loesung_c](https://diversewolken.ddns.net/nextcloud/index.php/s/pLBtBCiD4CyYiiM/download)

</details>

---

d) Bei nochmaliger Betrachtung des Kondensators stellt der Schüler fest, dass für die Kapazität eine Abweichung von bis zu 10% angegeben ist.

Überprüfe durch Rechnung, ob damit die Abweichung des experimentellen Werts von der theoretischen Schwingungsdauer erklärt werden kann.

<details>

<summary> Lösung </summary>

![Loesung_d](https://diversewolken.ddns.net/nextcloud/index.php/s/TEHDXdo4x4s2woG/download)

</details>

</p>

# LB 10 - Mechanische und Elektromagnetische Wellen


__Motivation:__

{{0-1}}
*************
??[Binogi-Wellen](https://app.binogi.de/l/wellen)
*************

{{1}}
*************
<iframe src="https://www.geogebra.org/classic/sn4xvwsj?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
*************

{{2}}
*********
> Eine @color(mechanische Welle, orange) ist die Ausbreitung eines Schwingungszustands von einem Ort im Raum zu einem anderen. 
>
>> Sie ist eine zeitlich __und räumlich__ periodische Änderung physikalischer Größen
>
> - Vorraussetzung sind __gekoppelte Schwinger__
>
> - eine Welle transportiert __Energie aber keine Masse__
>
> - die einzelnen schwingenden Teilchen bewegen sich ausschließlich um ihre Gleichgewichtslage
*********


## 10. 1. Arten mechanischer Wellen

<p class="newspaper3">

Längswellen (Longitudinalwellen)

__Beispiel:__ Schallwellen

> Schwingungsrichtung und Ausbreitungsrichtung stimmen überein.

<p class="cb">

Querwellen (Transversalwellen)

__Beispiel:__ Seilwellen, Erdbebenwellen

> Schwingungsrichtung und Ausbreitungsrichtung verlaufen senkrecht zueinander

<p class="cb">

Oberflächenwellen (Kreiswellen)

__Beispiel:__ Wasserwellen

> Teilchen führen kreisförmige Bewegung aus. Es wirken Kohäsionskräfte (Oberflächenspannung) und die Schwerkraft

</p>

</p>

</p>

<p style="color:blue">

__Beobachtung:__

1. Betrachten Sie die laufende Welle. Wechseln Sie zwischen Transversalwelle und Logitudinalwelle und beobachten Sie die Schwingung der Teilchen.

2. Ändern Sie die Amplitude und beobachten Sie die Welle. 

3. Verschieben Sie den Schieberegler ganz nach rechts und betrachten Sie die eingefrorene Welle.

<iframe src="https://www.geogebra.org/classic/cdyxv6pt?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

</p>

## 10. 2. Eigenschaften mechanischer Wellen

@color(_Tipp: Nutze für diese Übersicht eine eigene Seite_, orange)


{{0-1}}
************
__Diagrammdarstellung__: 

Wir stellen die **zeitliche Bewegung** eines einzelnen Oszillators (d.h. ein schwingendes Teilchen) mit einem **$y$-$t$-Diagramm** dar und die **räumliche Ausbreitung** mit einem **$y$-$x$-Diagramm**.

---

<p class="newspaper3">

> **Wellenlänge $\lambda$**


<p class="cb">

> **Frequenz $f$**

<p class="cb">

> **Ausbreitungsgeschwindigkeit $v$**


</p>

</p>

</p>

---

> __Wellenausbreitungsgleichung__

---

> __(*) Wellengleichung $y(x, t)$ einer harmonischen Welle:__

************


{{1}}
************
__Diagrammdarstellung__: 

Wir stellen die **zeitliche Bewegung** eines einzelnen Oszillators (d.h. ein schwingendes Teilchen) mit einem **$y$-$t$-Diagramm** dar und die **räumliche Ausbreitung** mit einem **$y$-$x$-Diagramm**.

---

<p class="newspaper">

> __$y(x)$-Diagramm__
>
> Für einen **bestimmten Zeitpunkt** ($t =$ konstant) wird dargestellt, **welche Lage die Gesamtheit der Oszillatoren** hat.
>
> __Wellengleichung $y(x)$ einer harmonischen Welle:__
>
> $$ \boxed{y(x) = y_{max} \cdot \sin\big(\frac{2\pi}{\lambda}\cdot x\big)}$$

<p class="cb">

> __$y(t)$-Diagramm__
>
> Für einen **bestimmten Ort** ($x =$ konstant) wird dargestellt, wie sich der betreffende Oszillator in **Abhängigkeit von der Zeit** bewegt.
>
> __Wellengleichung $y(t)$ einer harmonischen Welle:__
>
> $$ \boxed{y(t) = y_{max} \cdot \sin\big(\frac{2\pi}{T}\cdot t\big)}$$


</p>

</p>

---
************

{{2}}
************
<p class="newspaper">

![y-x-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/gJp99q4HHbZ7z8e/download)

<p class="cb">

![y-t-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/wfReL2Xbc5iGoXs/download)

</p>

</p>

---
************


{{3}}
************
<p class="newspaper3">

> **Wellenlänge $\lambda$**
>
> Die Wellenlänge ist der minimale Abstand zwischen zwei Oszillatoren, die sich im gleichen Schwingungszustand befinden.  
> Das ist auch der Abstand zwischen zwei benachbarten **Wellenbergen** oder **Wellentälern**.  

<p class="cb">

> **Frequenz $f$**
>
> Die Frequenz $f$ beschreibt die Anzahl an Schwingungen eines schwingende Teilchens pro Sekunde.
>
> Es gilt weiterhin: $f=\frac{1}{T}$

<p class="cb">

> **Ausbreitungsgeschwindigkeit $v$**
>
> Die Ausbreitungsgeschwindigkeit einer Welle ist die Geschwindigkeit, mit der sich eine bestimmte Phase im Raum ausbreitet.  

</p>

</p>

</p>

---

<p class="newspaper3">

> **Formelzeichen:** $\lambda$  
>
> **Einheit:** [1 m]

<p class="cb">

> **Formelzeichen:** $f$  
>
> **Einheit:** Hertz $[1\,\mathrm{Hz}=1\,\mathrm{\frac{1}{s}]}$

<p class="cb">

> **Formelzeichen:** $v$  
>
> **Einheit:** $[1\,\mathrm{\frac{m}{s}}]$

</p>

</p>

</p>

---
************


{{4}}
************
> __Wellenausbreitungsgleichung__ (Zusammenhang zwischen $\lambda$, $f$ und $v$:):
>
> $$ \boxed{v = \lambda \cdot f}$$

---
************

{{5}}
************
> __(*) Wellengleichung $y(x, t)$ einer harmonischen Welle:__
>
> Die Auslenkung $y$ einer in +x Richtung laufenden Welle lässt sich zu jedem Zeitpunkt $t$ und an jedem Ort $x$ mit der Wellengleichung angeben:
>
> $$ \boxed{y(x,t) = y_{max} \cdot \sin\Big( \frac{2\pi}{\lambda}\cdot x-\frac{2\pi}{T}\cdot t\Big)}$$
************


### Aufgaben zur Charakterisierung von Wellen

<iframe src="https://www.geogebra.org/classic/nc2tbcdm?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

__Die folgenden Aufgaben beziehen sich auf die Transversalwelle in Starteinstellung:__

1. Wenn Sie den Schieberegler_Animation_ ganz nach links bewegen, friert die Welle zeitlich ein. Ermitteln Sie die Wellenlänge der Transversalwelle. Ermitteln Sie ebenfalls die Amplitude.

<p style="margin-left:10%">

@rangeQuiz2($\lambda$,10,m)

@rangeQuiz2($y_{max}$,1.5,m)

</p>

2. Ermitteln Sie die Periodendauer $T$ und daraus die Frequenz $f$ und die Kreisfrequenz $\omega$ der Welle. Nutzen Sie dafür die eingefrorene Welle und den Schieberegler _Zeit_ im oberen Teil der Animation.

<p style="margin-left:10%">

@rangeQuiz2($T$,10,s)

@rangeQuiz2($f$,0.1,Hz)

@rangeQuiz2($\omega$,0.628,$\mathrm{\frac{1}{s}}$)

</p>

3. Wählen Sie die korrekte Wellengleichung $y(t)$ für den Ort $s=0\,\mathrm{m}$. <br> _Hinweis: Beobachten Sie den Schwinger am Ort $s=0\,\mathrm{m}$ und beschreiben Sie dessen zeitliche Bewegung._

<p style="margin-left:10%">

[[ ( $y(t) = 1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ ) | $y(t) = 1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | $y(t) = -1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | $y(t) = -1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ ]]

</p>

4. Wählen Sie die korrekte Wellengleichung $y(x)$ für den Zeitpunkt $t=0\,\mathrm{s}$. <br> _Hinweis: Frieren Sie die Welle zum Zeitpunkt $t=0\,\mathrm{s}$ ein und beschreiben Sie deren räumlichen Verlauf._

<p style="margin-left:10%">

[[ $y(x) = 1,5\,\mathrm{m}\cdot\sin(2\pi\cdot 0,1\,\mathrm{\frac{1}{m}}\cdot x)$ | $y(x) = 1,5\,\mathrm{m}\cdot\cos(2\pi\cdot0,1\,\mathrm{\frac{1}{m}}\cdot x)$ | ($y(x) = -1,5\,\mathrm{m}\cdot\sin(2\pi\cdot0,1\,\mathrm{\frac{1}{m}}\cdot x)$) | $y(x) = -1,5\,\mathrm{m}\cdot\cos(2\pi\cdot0,1\,\mathrm{\frac{1}{m}}\cdot x)$ ]]

</p>

5. Ermitteln Sie die Ausbreitungsgeschwindigkeit der Welle.

<p style="margin-left:10%">

@rangeQuiz2($v$,1, $\mathrm{\frac{m}{s}}$)

</p>

6. [Quiz zu mechanischen Wellen](https://www.leifiphysik.de/mechanik/mechanische-wellen/aufgabe/quiz-zu-mechanischen-wellen)

7. Die Gleichung für eine harmonische Welle sei gegeben durch <br> $$ y(x,t) = 0,03\,\mathrm{m}\cdot\sin\Big(2,2\,\mathrm{\frac{1}{m}}\cdot x-3,5\,\mathrm{\frac{1}{s}}\cdot t\Big) $$ <br> Ermitteln Sie Amplitude, Wellenlänge, Frequenz, Periodendauer und Ausbreitungsgeschwindigkeit.

<p style="margin-left:10%">

@rangeQuiz2($y_{max}$,0.03,m)

@rangeQuiz2($\lambda$,2.86,m)

@rangeQuiz2($f$,0.556,Hz)

@rangeQuiz2($T$,1.8,s)

@rangeQuiz2($v$,1.59, $\mathrm{\frac{m}{s}}$)

</p>


## 10. 3. Darstellung der Wellenausbreitung mit Wellenfront und Wellennormale

Zur Darstellung der Ausbreitung von Wellen nutzen man __Wellenfronten__ und @color(__Wellennormale__,red)

<p class="newspaper">

{{1}}
************
![WellenfrontWellenNormale](https://diversewolken.ddns.net/nextcloud/index.php/s/sPE2gzAdfqJqdjk/download "Links: Kreisförmige Wellenfront (z.B. Steinwurf in Wasser) | Rechts: Ebene Welle (z.B. Licht)")
************

<p class="cb">

{{4}}
*****************
__Die Wellenfronten__ sind Stellen maximaler Auslenkung (Wellenberge). Ihr Abstand voneinander ist gleich der Wellenlänge $\lambda$.

@color(Die Wellennormale, red) steht immer senkrecht auf der Wellenfront und gibt die Ausbreitungsrichtung der Welle an.
*****************

</p>

</p>

---

<p class="newspaper">

{{2}}
************
Kreisförmige Wellenfront (z.B. Steinwurf ins Wasser)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+4+668+0.00390625%0As+2+257+265+0+0.233333+0+10+100+1+0%0A)
************

<p class="cb">

{{3}}
************

Ebene Welle (z.B. Lichtausbreitung)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+0+569+0.048828125%0AS+2+0+1+511+1+0+0.466666+0+10+100+1+0%0A)
************

</p>

</p>

## 10. 4. Huygens'sche Prinzip

> Jeder Punkt einer Wellenfront ist seinerseits wieder Ausgangspunkt für @color(kreis- bzw. kugelförmige Elementarwellen, red)

{{1}}
*************
![Huygernssches-Prinzip](https://diversewolken.ddns.net/nextcloud/index.php/s/zE2kb4mDwinM5M2/download)


-> [Simulation-Ausbreitung-Kreiswelle-EbeneWelle](https://www.leifiphysik.de/mechanik/mechanische-wellen/ausblick/huygenssches-prinzip-zur-beschreibung-von-mechanischen-wellen)
*************


### Aufgabenstellung zur Selbsständigen Präsentation

<p style="color:blue">

Aufgabe: 

1. Wählen Sie eines der folgenden Themen aus.

2. Erarbeiten Sie sich das Wellenphänomen.

3. Stellen Sie das Wellenphänomen dem Auditorium in einem kurzen Beitrag vor. Nutzen Sie die bereitgestellte Simulation um den Sachverhalt zu verdeutlichen.

4. Lösen Sie die Aufgabe allein oder gemeinsam mit dem Auditorium.


</p>

<p class="newspaper3">

__Reflexion:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/GK.12_2025_2026/Praesentationen_Wellen/Reflexion.md#1)

<p class="cb">

__Brechung:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/GK.12_2025_2026/Praesentationen_Wellen/Brechung.md#1)

<p class="cb">

__Beugung:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/GK.12_2025_2026/Praesentationen_Wellen/Beugung.md#1)

</p>

</p>

</p>



## 10. 5. Reflexion

__Definition:__ Trifft eine Welle auf eine ebene Oberfläche, dann wird sie __reflektiert__. Es gilt das __Reflexionsgesetz__:

{{1}}
**********
<p class="newspaper">

> 1. Bei der Reflexion von Wellen sind der Einfallswinkel $\alpha$ und der @color(Reflexionswinkel $\alpha'$, red) gleich groß. 
>
> 2. Die Wellennormalen der einfallenden und reflektierten Wellen liegen in einer Ebene.

<p class="cb">

![Reflexion_Welle](https://diversewolken.ddns.net/nextcloud/index.php/s/bkBpwMGem3rXEx6/download)

</p>

</p>
**********

{{2}}
**********
??[Fendt-Reflexion](https://www.walter-fendt.de/html5/phde/refractionhuygens_de.htm)
**********

{{3}}
**********
<p style="color:blue">

Aufgaben:

1. In einem Wellenkanal läuft eine Wasserwelle auf eine glatte, senkrechte Wand zu. Welche Beobachtung macht man nach der Reflexion?

     - [[ ]] Die Welle verschwindet vollständig an der Wand.  
     - [[x]] Die Welle wird reflektiert und läuft in entgegengesetzter Richtung zurück.  
     - [[ ]] Die Welle ändert ihre Frequenz und läuft mit anderer Geschwindigkeit zurück.  
     - [[ ]] Die Welle läuft durch die Wand hindurch und setzt sich dahinter fort.

2. Eine Welle läuft auf eine Wand zu und wird reflektiert. Dabei beobachtet man bei der reflektierten Welle eine Winkel von 35° zwischen der Wellennormalen und der Wand. Nennen Sie den Einfallswinkel.

<p style="margin-left:10%">

@rangeQuiz2($\alpha$, 55 ,°)

</p>


</p>
**********


## 10. 6. Brechung


__Definition:__ Trifft eine Welle unter einem Einfallswinkel $\alpha\neq 0$ auf eine @color(__ebene Grenzfläche__, darkgreen) zweier Stoffe, in denen sie sich mit unterschiedlicher @color(Geschwindigkeit, red) ausbreitet, dann ändert sie ihre Ausbreitungsrichtung. Sie wird @color(gebrochen, red). Es gilt das __Brechungsgesetz__:

---

{{1}}
**********
<p class="newspaper">

Beim Übergang von einem Stoff (1) in einen anderen Stoff (2) gilt das __Brechungsgesetz__.

$$\boxed{\dfrac{\sin\alpha}{\sin\beta} = \dfrac{v_1}{v_2}}$$

wobei

<p style="margin-left:5%">

     $\alpha$ .. Einfallswinkel

     $\beta$ .. Brechungswinkel

     $v_1,\,v_2$ .. Ausbreitungsgeschwindigkeiten

</p>

<p class="cb">

![Brechung_Welle](https://diversewolken.ddns.net/nextcloud/index.php/s/3awXew9HRi54nyd/download)

</p>

</p>
**********

{{2}}
**********
??[Fendt-Reflexion](https://www.walter-fendt.de/html5/phde/refractionhuygens_de.htm)
**********


{{3}}
**********
<p style="color:blue">

Aufgaben:

1. Markieren Sie physikalisch sinnvolle Aussagen.

     - [( )] Wenn eine Welle auf eine Grenzfläche fällt, wird sie immer gebrochen.
     - [(x)] Wenn eine Welle auf eine Grenzfläche fällt, wird sie immer gebrochen, wenn der Einfallswinkel $\alpha\neq 0^\circ$

2. Ermitteln Sie den Brechungswinkel für den Übergang eines Lichtstrahls von  Luft nach Plexiglas. Die Lichtgeschwindigkeit in Luft beträgt $300'000\,\mathrm{\frac{m}{s}}$ und in Plexiglas $200'000\,\mathrm{\frac{m}{s}}$. Der Einfallswinkel beträgt 35°.

<p style="margin-left:10%">

@rangeQuiz2($\beta$, 22.48 ,°)

</p>


</p>
**********

## 10. 7. Beugung

Definition: Trifft eine Welle auf einen Spalt oder eine Kante, so sind die betreffenden Stellen nach _Huygens Prinzip_ Ausgangspunkt von Elementarwellen. Damit breitet sich eine Welle auch in den __Schattenraum__ aus.

---

<p class="newspaper3">

{{1}}
********
![Welle-Beugung](https://diversewolken.ddns.net/nextcloud/index.php/s/M9eEFxFCjRATLt2/download)
********

<p class="cb">

{{2}}
********
__Kante:__

??[Simulation-Kante](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+489+1.5625e-8%0Aw+0+255+132+514+132%0AS+2+0+1+511+1+0+1.399998+0+10+100+1+0%0Aw+0+511+-5+511+131%0A)
********

<p class="cb">

{{3}}
********
__Spalt:__

??[Simulation-Spalt](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+578+1.5625e-8%0AS+2+0+1+511+1+0+2.2166635+0+10+100+1+0%0A203+0+-57+145+577+145+1+20+10%0A)
********

</p>

</p>

</p>


{{4}}
**********
<p style="color:blue">

Aufgaben:

1. Markieren Sie physikalisch sinnvolle Aussagen.

     - [( )] Beugung von Licht ist mit dem Modell des Lichtstrahls erklärbar.
     - [(x)] Beugung ist ein Phänomen, dass sich nur mit der Welleneigenschaft des Lichts erklären lässt.

2. Eine Wasserwelle trifft auf eine schmale Spaltöffnung in einer Wand im Wellenkanal. Was beobachtet man hinter der Öffnung?

     - [[ ]] Die Welle läuft völlig ungestört geradeaus weiter, ohne sich zu verändern.  
     - [[x]] Die Wellen breiten sich nach der Öffnung halbkreisförmig in den Raum dahinter aus.  
     - [[ ]] Die Welle wird vollständig von der Wand absorbiert.  
     - [[ ]] Die Welle verschwindet und es entsteht nur noch stehendes Wasser. 

</p>
**********


### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)


## 10. 8. Interferenz

{{0}}
***********
!?[LEIFI-Wellen](https://diversewolken.ddns.net/nextcloud/index.php/s/NeMj4nWBfqDXMWj/download)
***********

{{1}}
***********
> __Prinzip der ungestörten Überlagerung:__ Wellen durchdringen sich gegenseitig, ohne sich selbst oder einander zu verändern

> Die __Überlagerung__ oder __Superposition__ harmonischer Wellen wird als @color(Interferenz, red) bezeichnet. Diese hängt vom __Gangunterschied__ der inteferierenden Wellen ab.
>
> Umgangssprachlich: _"Interferenz ist die Addition der jeweiligen Auslenkungen"_

<p style="margin:5%;color:blue">

Wir untersuchen die Interferenz von Wellen grafisch als auch mathematisch.

??[Geogebra-Interferenz-LK](https://www.geogebra.org/m/sd49erad)

</p>

---
***********

{{2}}
***********
<p class="newspaper3">

__Grafische Darstellung__

<p class="cb">

_Spezialfälle_

<p class="cb">

__Mathematische Beschreibung__

</p>

</p>

</p>

---

<p class="newspaper3">

![Konstruktive_Interferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/b788bF9RP233a38/download)

<p class="cb">

__Konstruktive Interferenz:__ Die Wellen überlagern sich derart, dass sich die Auslenkungen $y_1(x)$ und $y_2(x)$ addieren, es kommt zur Verstärkung der @color(resultierenden Welle, blue).

> __Der Gangunterschied beträgt eine Wellenlänge $\boxed{\lambda}$ <br> (oder ein Vielfaches $\boxed{n\cdot\lambda}$)__

<p class="cb">

$\green{y_1(x) = \hat{y_1}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\red{y_2(x) = \hat{y_2}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\blue{y_{ges}(x) = (\hat{y_1}+\hat{y_2})\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$


</p>

</p>

</p>

---

<p class="newspaper3">

![Destruktive_Interferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/WW2xPJiWLXGHd2D/download)

<p class="cb">

__Destruktive Interferenz:__ Die Wellen überlagern sich derart, dass sich die Auslenkungen $y_1(x)$ und $y_2(x)$ subtrahieren, es kann zur Auslöschen der @color(resultierenden Welle, blue) kommen.

> __Der Gangunterschied beträgt <br> $\boxed{\frac{\lambda}{2}}$ (bzw. $\boxed{\frac{\lambda}{2} + n \cdot \lambda}$)__

<p class="cb">

$\green{y_1(x) = \hat{y_1}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\red{y_2(x) = -\hat{y_2}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\blue{y_{ges}(x) = (\hat{y_1}-\hat{y_2})\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$


</p>

</p>

</p>

---

***********

## 10. 8. Interferenz

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Grafische Darstellung__

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

_Spezialfälle_

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Mathematische Beschreibung__

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Konstruktive_Interferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/b788bF9RP233a38/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Konstruktive Interferenz:__ Die Wellen überlagern sich derart, dass sich die Auslenkungen $y_1(x)$ und $y_2(x)$ addieren, es kommt zur Verstärkung der @color(resultierenden Welle, blue).

> __Der Gangunterschied beträgt eine Wellenlänge $\boxed{\lambda}$ <br> (oder ein Vielfaches $\boxed{n\cdot\lambda}$)__

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

$\green{y_1(x) = \hat{y_1}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\red{y_2(x) = \hat{y_2}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\blue{y_{ges}(x) = (\hat{y_1}+\hat{y_2})\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Destruktive_Interferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/WW2xPJiWLXGHd2D/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Destruktive Interferenz:__ Die Wellen überlagern sich derart, dass sich die Auslenkungen $y_1(x)$ und $y_2(x)$ subtrahieren, es kann zur Auslöschen der @color(resultierenden Welle, blue) kommen.

> __Der Gangunterschied beträgt <br> $\boxed{\frac{\lambda}{2}}$ (bzw. $\boxed{\frac{\lambda}{2} + n \cdot \lambda}$)__

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">


$\green{y_1(x) = \hat{y_1}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\red{y_2(x) = -\hat{y_2}\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

$\blue{y_{ges}(x) = (\hat{y_1}-\hat{y_2})\cdot\sin(\frac{2\pi}{\lambda}\cdot x)}$

</div>

</section>

## 10. 9. Stehende Wellen

[StehendeWellen-Geogebra](https://www.geogebra.org/m/wcqzrbnh)

> Wenn sich Wellen nur __in einem begrenzten Gebiet__ ausbreiten können (wie auf den Saiten einer beidseitig eingespannten Klavierseite), treten an beiden Enden Reflexionen auf. Dadurch kommt es zu einer Überlagerung von einlaufenden und reflektierten Wellen, die sich in entgegensetzter Richtung bewegen. Abhängig von der Begrenzung (Saitenlänge $ℓ$) gibt es bestimmte Frequenzen (Wellenlängen), bei denen die Wellen __stationäre Schwingungsmuster__ ausbilden. Diese heißen __Stehende Wellen__.

<p class="newspaper">

![StehendeWellenAufEinerSeite](https://diversewolken.ddns.net/nextcloud/index.php/s/9qCpdFZJ8zQixd9/download)

<p class="cb">

> Eine __stehende Wellen__ kennzeichnet sich durch __Bäuche (B)__ (verstärkte Schwingung) und __Knoten (K)__ (keine Schwingung).
>
> Eine __(eindimensionale)__ stehende Welle kann auftreten, wenn die Ausdehung $ℓ$ ein Vielfaches der halben Wellenlänge $\frac{\lambda}{2}$ ist.
>
> $$ \boxed{ℓ = n \cdot \frac{\lambda}{2}} \,\,\,n=1,2,3...$$
>
> Man nennt die zugehörigen Schwingungen die __$n$-te Harmonische__.

</p>

</p>

![Stehende-WellenGitarre](https://diversewolken.ddns.net/nextcloud/index.php/s/nERJCb4RJEyjYji/download)

### Übungsaufgaben zu Wellenphänomenen

#### Übung 1 - Welleneigenschaften

<p class="newspaper">

![Phy10_LB_42_Aufgabe_2](https://diversewolken.ddns.net/nextcloud/index.php/s/Bx6NGaj2z63TtFM/download)

<p class="cb">

<details>

<summary> Lösung </summary>

- die Schwingung beginnt an einem Ausgangspunkt (hier z.B. linke Pendel)
- durch die Kopplung der einzelnen Pendel regt das erste Pendel das Zweite an und gibt somit mechanische Energie weiter
- das zweite Pendel wiederum regt das dritte Pendel an usw. 
- auf diese Weise wird zwar Energie, aber keine Materie transportiert

</details>

</p>

</p>

---


<p class="newspaper">

![Phy10_LB_42_Aufgabe_4](https://diversewolken.ddns.net/nextcloud/index.php/s/xC8zPGjBriw4mL6/download)

<p class="cb">

@rangeQuiz2($\hat{y}$,1.667 ,mm)

@rangeQuiz2($\lambda$,0.6 ,m)

@rangeQuiz2($T$, 0.002 ,s)

@rangeQuiz2($f$, 500 ,Hz)

</p>

</p>

<details>

<summary> Lösungsweg Aufgabe 4 </summary>

<iframe src="https://diversewolken.ddns.net/pdfjs/web/viewer.html?file=https://diversewolken.ddns.net/nextcloud/index.php/s/wTgm6wH49e645Gk/download"
        width="100%" 
        height="400px">
</iframe>

</details>

---

<p class="newspaper">

![Phy10_LB_42_Aufgabe_5](https://diversewolken.ddns.net/nextcloud/index.php/s/oHA9JEFt3oLrick/download)

<details>

<summary> _Lösungshinweis_ </summary>

Recherchieren Sie in Ihrer Formelsammlung die Schallgeschwindigkeit in Luft bei 20°C._

@rangeQuiz2($v_{S}$,434, $\mathrm{\frac{m}{s}}$)

</details>

<p class="cb">

@rangeQuiz2($T$, 1.9 , ms)

@rangeQuiz2($\lambda$, 0.658 ,m)

</p>

</p>

#### Übung 2 - Wellenphänomene

Ordne den folgenden Abbildungen das Wellenphänomen zu.

<iframe src="https://learningapps.org/watch?v=p29hwaena25" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

#### Übung 3 - Stehende Wellen

1. Die $60\,\mathrm{cm}$ lange H-Saite einer Gitarre schwinge mit $247\,\mathrm{Hz}$. <br> 

1. 1. Nennen Sie die Art der Wellen, mit der die Saite schwingt.

<p style="margin-left:5%">

[[ (Transversalwelle) | Longitudinalwelle | Kreiswelle ]]

</p>

1. 2. Ermittlen Sie die Ausbreitungsgeschwindigkeit der Transversalwelle auf der Saite. 

<p style="margin-left:5%">

@rangeQuiz2($v$,296,$\mathrm{\frac{m}{s}}$)

</p>

1. 3. Die Saite überträgt die Schwingung auf die Luft. Nennen Sie die Art der Welle von Schall in Luft.

<p style="margin-left:5%">

[[ Transversalwelle | (Longitudinalwelle) | Kreiswelle ]]

</p>


1. 4. Die G-Saite einer Violine ist $30\,\mathrm{cm}$ lang. Wenn Sie ohne Griff (d.h. ohne Saitenverkürzung) gespielt wird, schwingt sie mit einer Frequenz von $196\,\mathrm{Hz}$. <br> Als nächst höhere Schwingungsmoden folgen die Violinennoten a($220\,\mathrm{Hz}$), h ($247\,\mathrm{Hz}$), c ($262\,\mathrm{Hz}$) und d ($294\,\mathrm{Hz}$). <br> Ermitteln Sie den Abstand vom Saitenende, an dem der Finger aufgesetzt werden muss, damit diese Noten gespielt werden können.

<p style="margin-left:10%">

@rangeQuiz2(a: $s_a$,3.27,$\mathrm{cm}$)

@rangeQuiz2(h: $s_h$,6.19,$\mathrm{cm}$)

@rangeQuiz2(c: $s_c$,7.56,$\mathrm{cm}$)

@rangeQuiz2(d: $s_d$,10,$\mathrm{cm}$)


<details>

<summary> _Lösungshinweis_ </summary>

Die Wellenlänge der Grundschwingung einer beidseitig eingespannten, unverkürzten Saite (Note g) ist $\lambda_G=2ℓ$. Man kann nun die Ausbreitungsgeschwindigkeit der Welle $v$ auf der Saite ermitteln.

@rangeQuiz2($v=\lambda_g \cdot f_g$,117.6,$\mathrm{\frac{m}{s}}$)

Somit ergibt sich für die Wellenlänge der Grundschwingung der verkürzten Saite mit der Note a die Wellenlänge

@rangeQuiz2($\lambda_a = \frac{v}{f_a}$,53.45,$\mathrm{cm}$)

Da die Grundschwingung der Saite der halben Wellenlänge $\lambda_a$ entspricht, muss die Saite 3,28 cm verkürzt werden

</details>

</p>

## 10. 10. Begründung des Relfexionsgesetzes mit dem Huygens'schen Prinzip

![RG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/oNFR69QaAyscHcM/download)

![RG_TB2](https://diversewolken.ddns.net/nextcloud/index.php/s/nAGqm7nxZKQ3WRo/download)

### Konstruktion der Reflexion mit Geogebra

??[Reflexionsgesetz_Grundeinstellungen](https://www.geogebra.org/m/drjnyjee)

### Übungsaufgaben

1. In einer Wellenwanne läuft eine Wasserwelle von einem seichten Bereich in ein Gebiet mit tieferem Wasser unter dem Einfallswinkel von 45° und einem Brechungswinkel von 60°. Bestimmen Sie die Geschwindigkeit im flachen Teil, wenn sie im tiefen Teil $25\,\mathrm{\frac{cm}{s}}$ beträgt.<br><br> _Hinweis: Die Ausbreitungsgeschwindigkeit von Wasserwellen folgt näherungsweise derm Zusammenhang $v\sim\sqrt{h}$, wobei h die Wassertiefe ist._

<p style="margin-left:10%">

@rangeQuiz2($v_{flach}$,20.4,$\mathrm{\frac{cm}{s}}$)

</p>

2. Wasserwellen bewegen sich in tiefem Wasser mit der Geschwindigkeit $v_1=35\,\mathrm{\frac{cm}{s}}$. Sie treffen unter dem Winkel $60\,^\circ$ auf die Grenzlinie zu einem flacheren Teil, wo sie sich mit $v_2=24\,\mathrm{\frac{cm}{s}}$

2. 1. Berechnen Sie den Brechungswinkel.

<p style="margin-left:10%">

@rangeQuiz2($\beta$,20.05,$^\circ$)

</p>

2. 2. Die Wellenlänge im tieferen Teil beträgt $\lambda_1=1,7\,\mathrm{cm}$. Berechnen Sie die Wellenlänge im flacheren Teil. Geben Sie ebenfalls die Frequenzen $f_1$ und $f_2$ an.

<p style="margin-left:10%">

@rangeQuiz2($\lambda_2$,1.17,cm)

@rangeQuiz2($f_1$,20.6,Hz)

@rangeQuiz2($f_2$,20.6,Hz)

</p>

## 10. 11. Begründung des Brechungsgesetzes mit dem Huygens'schen Prinzip

![BG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/FitcjCLbt8ecfCW/download)



### Aufgaben zu Wellen

1. Geben Sie an, welche Aussagen richtig sind:

     <!-- data-solution-button="3" -->
     [[X]] Jede Wellerscheinung ist mit der Übertragung von Energie, aber nicht mit dem Transport von Stoff verknüpft.  
     [[ ]] Wird die Frequenz von Schallwellen bei sonst gleichen Bedingungen erhöht, erhöht sich auch deren Wellenlänge.  
     [[ ]] Die Ausbreitungsgeschwindigkeit mechanischer Wellen hängt ausschließlich und allein von der Intensität ihrer Anregung ab.  
     [[X]] Mechanische Wellen können als Transversal- oder Longitudinalwellen auftreten.  
     [[ ]] Bei mechanischen Longitudinalwellen schwingen Teilchen senkrecht zur Ausbreitungsrichtung der Welle.  

---

2. Eine eindimensionale Seilwelle der Frequenz $0,8\,\mathrm{Hz}$, der Amplitude $12\,\mathrm{cm}$ und der Wellengeschwindigkeit $2\,\mathrm{m/s}$ breitet sich in x-Richtung aus. Die Welle startet zum Zeitpunkt $t=0$ an einem Seilende ($x=0$).

2. 1. Ermitteln Sie die Zeit, wann das  beginnt das Seilteilchen bei $x=2\,\mathrm{m}$ zu schwingen beginnt.


<p style="margin-left:10%">

@rangeQuiz2($t$,1,s)

</p>

2. 2. Ermitteln Sie die Auslenkung, welche das Seilteilchen bei $x=1\,\mathrm{m}$ nach $3\,\mathrm{s}$ besitzt.

<p style="margin-left:10%">

@rangeQuiz0($y$,0,cm)

<details>

<summary> _Lösung_ </summary>

![Lsg_2_2](https://diversewolken.ddns.net/nextcloud/index.php/s/RLrnBznYZFbsGGp/download)

</details>

</p>

---

3. Auf einem linearen Wellenträger breitet sich eine transversale Welle vom Ursprung eines Koordinatensystems in Richtung der positiven x-Achse mit der Geschwindigkeit $c=0,5\,\mathrm{m/s}$ aus. Der Erreger schwingt sinusförmig mit $10\,\mathrm{Hz}$ und beginnt zur Zeit $t=0$ mit einer Bewegung nach oben. Die Amplitude beträgt $1\,\mathrm{cm}$.

3. 1. Ermitteln Sie Wellenlänge und Schwingungsdauer.


<p style="margin-left:10%">

@rangeQuiz2($\lambda$,5,cm)

@rangeQuiz2($T$,0.1,s)

<details>

<summary> _Lösung_ </summary>

![Lsg_3_1](https://diversewolken.ddns.net/nextcloud/index.php/s/nzELxH4RGGWzsrL/download)

</details>

</p>

3. 2. Ermitteln Sie die Zeit, wann die Welle den Ort $x=0,2\,\mathrm{m}$ erreicht hat.

<p style="margin-left:10%">

@rangeQuiz2($t$,0.4,s)



<details>

<summary> _Lösung_ </summary>

![Lsg_3_2](https://diversewolken.ddns.net/nextcloud/index.php/s/XprpMejgsPbffET/download)

</details>

</p>

3. 3. Zeichnen Sie ein Momentanbild $y(x)$ der Welle zur Zeit $t=0,18\,\mathrm{s}$.


<p style="margin-left:10%">

<details>

<summary> _Lösung_ </summary>

![Lsg_3_3](https://diversewolken.ddns.net/nextcloud/index.php/s/bBrjopKFCdNrXes/download)

</details>

</p>

---

4. Eine Welle, trifft in einem Winkel von 40° auf eine Grenzfläche. Im ersten Medium ist die Wellengeschwindigkeit doppelt so hoch, wie im zweiten Medium. Ermitteln Sie den Brechungswinkel ausschließlich unter durch eine Konstruktion mit Zirkel und Lineal.

<p style="margin-left:10%">

@rangeQuiz20($\beta$,20,$^\circ$)

<details>

<summary> _Lösunghinweise_ </summary>

1. Zeichnen Sie zunächst die Grenzfläche und die Wellennormale, die in einem Winkel von 40° auf die Grenzfläche fällt. 

2. Zeichnen sie eine Wellenfront und verlängern sie die Wellenfront bis zur Grenzfläche (Schnittpunkt A -> siehe 10.11). 

3. Ermitteln Sie mit dem Zirkel den Abstand der Wellenfront von der Grenzfläche entlang der Wellennormale (Abstand Punkte B & B')

4. Da die Welle im zweiten Medium nur die halbe Geschwindigkeit hat, wie im ersten Medium, müssen Sie diese Strecke halbieren. Legen Sie den Zirkel auf die halbe Streckenlänge an.

5. Ziehen Sie um den Punkt A im zweiten Medium einen Halbkreis mit dem Radius des halben Abstands der Strecke $\overline{BB'}$

6. Um den Schnittpunkt der neuen Wellenfront mit dem gezeichneten Halbkreis zu ermitteln, zeichnen Sie einen Thaleskreis über der Strecke $\overline{AB'}$. Der Schnittpunkt zwischen dem Halbkreis aus 5. und dem Thaleskreis markiert einen Punkt der neuen Wellenfront (Punkte A').

7. Verbinden Sie die Punkte A' und B' zu einer neuen Wellenfront im Medium zwei.

8. Ermitteln Sie aus der Lage dieser Wellenfront den Brechungswinkel.

<details>

<summary> _Lösung_ </summary>

![Lsg_4](https://diversewolken.ddns.net/nextcloud/index.php/s/j9A9WoDsmDp22CP/download)

</details>

</details>

</p>



### Entwicklung Leistungen 12Ph2

![Ergebnisse_12LKA1](https://diversewolken.ddns.net/nextcloud/index.php/s/7AQEiYWeiiwRSnp/download)

{{1}}
*********
<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Durchschnitt"
-->
| Test | Durchschnittsnote | Trend |
| ---- | ---- | ---- |
| 11/LK1 | 7.9 | 8.05 |
| 11/KA1 | 6.3 | 8.23 |
| 11/EX1 | 11.9| 8.41 |
| 11/KA2 | 7.7 | 8.59 |
| 11/LK2 | 8.8 | 8.77 |
| 11/KA3 | 8.7 | 8.95 |
| 11/KA4 | 9.1 | 9.13 | 
| 11/EX2 | 10.5 | 9.31 |
| 12/LK1  | 8.9 | 9.49 |
| 12/KA1  | 9.5 | 9.67 |
*********



{{2}}
*************

<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="Bewertung"
     data-ylabel="Note"
     data-transpose
-->
|	|LK1	|KA1	|KA2	|LK2	|KA3	|KA4 | EX2 | LK3 | KA5 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |  :---: |
|1	|6	|2	|5	|8	|10	|7 | 10 | 5 |  8|
|2	|6	|5	|4	|8	|9	|9 | 11 | 5 |  10|
|3	|9	|6	|9	|6	|10	|11 |11 | 11 | 12|
|4	|9	|8	|10	|9	|5	|6 | 8  | 8 |  8|
|5	|6	|3	|4	|5	|7	|5 | 8  | 6 |  7|
|6	|8	|6	|8	|6	|6	|8 | 8  | 7 |  8|
|7	|9	|3	|7	|11	|12	|14 |9  | 11 | 8|
|8	|7	|3	|7	|7	|5	|8 | 12 | 8 |  6|
|9	|3	|4	|6	|8	|10	|2 | 12 | 9 |  7|
|10	|9	|3	|9	|11	|8	|10 |9  | 12 | 11|
|11	|13	|12	|15	|15	|14	|14 |15 | 13 | 14|
|13	|11	|7	|9	|10	|10	|12 |14 | 10 | 12|
|14	|11	|12	|14	|15	|15	|15 |14 | 14 | 15|
|15	|9	|12	|6	|8	|3	|9 | 10 | 5 |  7|

*************



## 10. 12. Das Doppelspalt-Experiment

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> __Beschreibung:__ Beim Doppelspaltexperiment schickt man @color(kohärentes, orange), einfarbiges Licht (z.B. Laserlicht) durch zwei nahe beieinander liegende Spalte, den sogenannten Doppelspalt. Das Licht fällt auf einen hinter dem Doppelspalt liegenden Schirm.
>
> {1}{__Beobachtung:__ Auf dem Schirm entsteht ein Muster aus vertikalen hellen und dunklen Streifen.}
>
> {2}{__Erklärung:__ An den beiden Spalten entstehen laut dem huygen'schen Prinzip neue Elementarwellen. Diese Wellen überlagern (__interferieren__) sich und bilden beim Auftreffen auf einem Beobachtungsschirm ein Interferenzmuster aus hellen und dunklen Bereichen. ->[DoppelSpalt-Simulation](https://falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+578+1.5625e-8%0AS+2+0+1+511+1+0+1.633331+0+10+100+1+0%0A203+0+-60+54+574+54+2+6+15%0A)}

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

{0-1}{![Doppelspalt_KeinSchirm](https://diversewolken.ddns.net/nextcloud/index.php/s/c8TRSPoriw65AC9/download "Prinzipskizze des Doppelspalt-Experiments")}

{1}{![Doppelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/PWMnf2JX4xiXamx/download "Prinzipskizze des Doppelspalt-Experiments")}

</div>

</section>

---

{{3}}
*********
> __Schlussfolgerung:__
>
> Das Muster auf dem Schirm ist nur durch Beugung und Interferenz, d.h. also durch Wellenerscheinungen, erklärbar: <br> => @color(Licht besitzt Welleneigenschaften, orange).

---
*********



{{4}}
*********
> __Eigenschaften von Lichtwellen:__

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{5}}
*********
1. bei einer Lichtwelle schwingt das <span style="color:orange">***elektrische und das magnetische Feld.***</span>

2. eine Lichtwelle benötigt @color(***kein Medium***, orange) (anders als z.B. Schall[Luft], Wasserwellen[Wasser]) zur Ausbreitung. 

3. Licht ist eine @color(***Transversalwelle***, orange). 

4. Das elektromagnetische Feld @color(***transportiert Energie***, orange).
*********

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{6}}
*********

5. Die Ausbreitungsgeschwindigkeit (Lichtgeschwindigkeit) im Vakuum beträgt 

$$\boxed{c = 300.000 \dfrac{km}{s}}$$

6. Für die Lichtgeschwindigkeit in einem Medium gilt:

$$\boxed{c_{Medium} < 300.000 \dfrac{km}{s}}$$

*********

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{7}}
*********
6. Es gilt die Wellenausbreitungsgleichung: <br> $$ \boxed{c = \lambda \cdot f}$$ <br> Die Wellenlänge $\lambda$ der Lichtwelle bestimmt die <span style="color:orange">***Lichtfarbe***</span>.
*********

</div>

</section>


*********


## 10. 13. Bestimmung der Wellenlänge des Lichts am Doppelspalt

<section class="flex-container">

<div class="flex-child-3" style="min-width: 300px; margin-bottom: -10px">

{0-1}{![Doppelspalt1](https://diversewolken.ddns.net/nextcloud/index.php/s/CjeoRm63RYeerPN/download)<!-- style="width:100%" -->}
{1-2}{![Doppelspalt2](https://diversewolken.ddns.net/nextcloud/index.php/s/MgaPdZqPbmTWGLp/download)<!-- style="width:100%" -->}
{2-3}{![Doppelspalt3](https://diversewolken.ddns.net/nextcloud/index.php/s/QaNR3Q4A8JfSsfA/download)<!-- style="width:100%" -->}
{3-4}{![Doppelspalt4](https://diversewolken.ddns.net/nextcloud/index.php/s/sAMqHnH3omTsE9W/download)<!-- style="width:100%" -->}
{4}{![Doppelspalt5](https://diversewolken.ddns.net/nextcloud/index.php/s/rR93K2CqrPDwTDR/download)<!-- style="width:100%" -->}


</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

{{1}}
***************
1. Auf dem Schirm entsteht ein @color(***Interferenzmuster***, green).
***************

{{2}}
***************
2. Die Spalte haben den Abstand $\blue{d}$, der Schirm hat vom Spalt den Abstand $\blue{e}.$
***************

{{3}}
***************
3. Im Punkt __A__ beobachten wir konstruktive Interferenz, wir nennen es @color(***Interferenz-Maximum***, green). Dieses Maximum ergibt sich aus der Überlagerung der Elementarwellen aus den Spalten $s_1$ und $s_2$.
***************

{{4}}
***************
4. Für konstruktive Interferenz muss der Gangunterschied $\purple{\Delta s}$ einem Vielfachen der Wellenlänge entsprechen. <br> $$ \purple{\Delta s= k \cdot \lambda} \hspace{1cm}\mathrm{mit}\,\,k=1,\,2,..$$
***************

{{5}}
***************
5. Im rechtwinkligen Dreieck $\triangle S_1 S_2 P$ gilt:

$$ \dfrac{\purple{\Delta s}}{\blue{d}} = \boxed{\dfrac{\purple{k\cdot\lambda}}{\blue{d}} = \sin(\alpha) }$$

***************

{{6}}
***************
6. Im rechtwinkligen Dreieck $\triangle M O A$ gilt:

$$ \boxed{\tan(\alpha) = \blue{\dfrac{a}{e}}}$$

***************

</div>

</section>

{{6}}
***************
> Da wird die Größen $\blue{d,\,e}$ und $\blue{a}$ @color(__messen__, blue) können, lässt sich mit dem __Doppelspalt-Experiment__ die @color(Wellenlänge $\lambda$, purple) des Laserlichts bestimmen.

---
***************

{{7}}
***************
<section class="flex-container">

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

__Experimentelle Messwerte:__ 

> $d$ = <input type="number" default="0" min="0" max="10" id="d" size="5"> m <br> <br> $a$ = <input type="number" default="0" min="0" max="10" id="a" size="5"> m <br> <br> $e$ = <input type="number" default="1" min="0" max="10" id="e" size="5">m

@color(_Hinweis: Dezimalzahlen mit "."_, gray)

</div>

<div class="flex-child-3" style="min-width: 300px; margin-bottom: -10px">

__Ermittlung der Wellenlänge:__

{{8}}
***************
> $\tan{\alpha} = \dfrac{a}{e} \hspace{0.5cm}\Rightarrow\hspace{0.5cm}\alpha = \tan^{-1}\Big(\dfrac{a}{e}\Big) = $ <script input="button">
    let d = document.getElementById("d").value;
    let a = document.getElementById("a").value;
    let e = document.getElementById("e").value;
    Math.round(Math.atan(a/e)*180/Math.PI*1000)/1000
</script> °
***************

{{9}}
***************
Für das erste Interferenz-Maximum ($k=1$) gilt:

> $ \lambda = d \cdot \sin\alpha \approx $ <script input="button">
    let d = document.getElementById("d").value;
    let a = document.getElementById("a").value;
    let e = document.getElementById("e").value;
    Math.round(d*Math.sin(Math.atan(a/e))/1e-9)
</script> nm $\hspace{1cm}\big[\mathrm{nm}=10^{-9}\mathrm{m}\big]$
***************


</div>

</section>

***************

### Aufgaben zum Thema _Licht als Welle_

1. Die Lichtgeschwindigkeit im Vakuum beträgt etwa $3 \cdot 10^8 \, \mathrm{\frac{m}{s}}$. Berechne die Frequenz von grünem Licht mit einer Wellenlänge von 500 nm.

<p style='margin-left:10%'>

@rangeQuiz2($f$,6e14,Hz)

</p>

---

2. Zwei enge Spalte deren Abstand 1,5 mm beträgt werden mit Licht einer Natriumdampflampe (Wellenlänge 589 nm) beleuchtet. Auf einem Schirm in 3 Metern Entfernung werden Interferenzstreifen beobachtet. Berechnen Sie den Abstand der Streifen.

<p style='margin-left:10%'>

@rangeQuiz2($a$,1.18,mm)

</p>

<details style='margin-left:10%'>

<summary> Lösungshinweis </summary>

Achten Sie auf die Nutzung der Standardeinheit _Meter_ für alle Längenangaben.

</details>

---

3. Auf ein optisches Gitter mit der Gitterkonstante $4,00\cdot10^{-6}\,\mathrm{m}$ (_wie Doppelspalt mit Abstand $d$ zu behandeln_) fällt Licht der Wellenlänge $694\,\mathrm{nm}$ senkrecht ein. Das Interferenzbild wird auf einem $2\,\mathrm{m}$ entfernten ebenen Schirm beobachtet, der parallel zum Gitter steht.

3. 1. Berechnen Sie den Abstand $x$ der auf dem Schirm sichtbaren Maxima erster Ordnung.

<p style='margin-left:10%'>

@rangeQuiz2($x$,0.7,m)

<details>

<summary> Lösungshinweis </summary>

Der Abstand der Maxima ist doppelt so groß, wie der Abstand des ersten Maximums vom mittleren Punkt (__O__).

</details>

</p>

3. 2. Überprüfen Sie, bis zu welcher Ordnung Maxima überhaupt beobachtet werden können.

<p style='margin-left:10%'>

@rangeQuiz2($k$,5,.)

</p>

<details style='margin-left:10%'>

<summary> Lösungshinweis1 </summary>

Überlegen Sie, welcher Winkel $\alpha$ für die Beobachtung einer Interferenz hinter einem Beugungsgitter maximal sinnvoll ist.

</details>

<details style='margin-left:10%'>

<summary> Lösungshinweis 2 </summary>

Ein Winkel $\alpha$ von über 90° ist nicht beobachtbar. Überprüfen Sie, dem wievielten Maximum dieser Winkel entspricht.

</details>


## 10. 14. Interferenz am Beugungsgitter

<section class="flex-container">

<div class="flex-child-3" style="min-width: 300px; margin-bottom: -10px">

{0-1}{![Gitter1](https://diversewolken.ddns.net/nextcloud/index.php/s/GMq4Sf9ikwojNzn/download)<!-- style="width:100%" -->}
{1-2}{![Gitter2](https://diversewolken.ddns.net/nextcloud/index.php/s/EDFRkcpcaE4Pn9C/download)<!-- style="width:100%" -->}
{2-3}{![Gitter3](https://diversewolken.ddns.net/nextcloud/index.php/s/cF9KjeQkzS9Efy4/download)<!-- style="width:100%" -->}
{3-4}{![Gitter4](https://diversewolken.ddns.net/nextcloud/index.php/s/pcWt3TfDmLCN4pH/download)<!-- style="width:100%" -->}
{4-5}{![Gitter5](https://diversewolken.ddns.net/nextcloud/index.php/s/ag8fSHexziD8WXZ/download)<!-- style="width:100%" -->}
{5-6}{![Gitter6](https://diversewolken.ddns.net/nextcloud/index.php/s/bnZMewH3qSqd7Ja/download)<!-- style="width:100%" -->}
{6-7}{![Gitter7](https://diversewolken.ddns.net/nextcloud/index.php/s/X8FjKjwoxSDX7FX/download)<!-- style="width:100%" -->}
{7}{![Gitter8](https://diversewolken.ddns.net/nextcloud/index.php/s/4igXLgZHtQ6nN6e/download)<!-- style="width:100%" -->}

</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

{{7}}
***************
1. Es gelten die Formeln wie beim Doppelspalt

$$ \boxed{ \sin(\alpha) = \dfrac{\purple{k\cdot\lambda}}{\blue{b}}  } \hspace{.5cm} \boxed{\tan(\alpha) = \blue{\dfrac{a}{e}}}$$
***************

{{8}}
***************
2. Eigenschaften des Interferenzbildes am Gitter

<p style="margin-left:5%">

- Maxima sind schärfer abgegrenzt als beim Doppelspalt

- zwischen den Maxima ist die Lichtintensität sehr gering (Auslöschung)

</p>
***************

{{9}}
***************
3. __Kleinwinkelnäherung__ <br> <br> Wenn der Beobachtungswinkel $\alpha \leq 5^\circ$  beträgt, dann gilt in guter Näherung $$ sin(\alpha) = \tan(\alpha)$$ und die Formeln (1.) vereinfachen sich zu $$ \boxed{\dfrac{\purple{k\cdot\lambda}}{\blue{b}} = \blue{\dfrac{a}{e}}} $$ wobei das Maximum $\purple{k}$-ter Ordnung betrachtet wird.

***************
</div>

</section>

<!-- style="display:none" -->
<div style="display:block" id="fooBar">
__Aufgabenstellung:__ 

- Erarbeiten Sie sich selbstständig die Grundlagen zum Thema: _Interferenz am Beugungsgitter_. 

- Nutzen Sie dafür (je nach Vorliebe) __Metzler__ S. 304-305 oder __Duden__ S. 413-414.

- Achten Sie darauf, dass Sie die Beschreibung eines Beugungsgitters notiert haben, das Beugungsmuster verstanden haben und die zugehörigen Berechnungsformeln notiert haben.

- Bearbeiten Sie anschließend die experimentelle Aufgabe sowie die Abituraufgabe
</div>


### Experimentelle Aufgabe zum optischen Gitter

<p style="color:blue">

__Aufgabenstellung:__ 

Ihnen wird ein optisches (Transmissions-)Gitter mit unbekannter Gitterkonstante $b$ ausgehändigt. Nutzen Sie das Experiment _Interferenz am optischen Gitter_ um die Gitterkonstante $b$ zu ermitteln.

- Zeichnen Sie sich eine Skizze Ihres Versuchsaufbaus. Tragen Sie in Ihre Skizze die zum messenden Größen ein.

- Notieren Sie die Berechnungsformeln zur Ermittlung der Gitterkonstante

- Bestimmen Sie die Gitterkonstante für zwei Wellenlängen einfallenden Lichtes (roter und grüner Laser)

- Notieren Sie sich Ihre Messwerte und überprüfen Sie die Übereinstimmung der ermittelten Gitterkonstante für die beiden Laserfarben

</p>

<p style='margin-left:10%'>

__Ergebnis-Überprüfung:__

@rangeQuiz20($g$,12.5e-6,m)

</p>


### Abituraufgabe zum optischen Gitter

> In einem Experiment fällt das Infrarotlicht einer Fernbedienung senkrecht auf ein Gitter mit 600 vertikalen Spalten pro Millimeter. Eine Handy-Kamera wird auf einem Halbkreis um das Gitter geführt (siehe Abbildung 1). Sie registriert dabei die Intensität des Infrarotlichts. Der Winkel zwischen den beiden Maxima erster Ordnung beträgt 70°.

![Abituraufgabe_Messaufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/NomQLdczLDTFp4m/download "Abbildung 1: Messaufbau")

1. 1. Erläutere mithilfe einer Skizze, dass Maxima der Intensität nachgewiesen werden können.

<details style='margin-left:10%'>

<summary> Lösungshinweise </summary>

Das optische Gitter hat 600 vertikale Spalte. Die Spalte sind Ausgangspunkte einer Elementarwelle, die sich, je nach Gangunterschied $\Delta s$, unterschiedlich überlagern. Immer wenn der Gangunterschied ein ganzzahliges Vielfaches der Wellenlänge ist, kommt es zur konstruktiven Interferenz, es tritt also ein
Maximum auf. Vorraussetzung für den Versuch ist ebenfalls, dass der Abstand zwischen Gitter und Schirm viel größer ist als der Gangunterschied. Überlege dir, ob das der Fall ist.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Lsg_1_1](https://diversewolken.ddns.net/nextcloud/index.php/s/E4WRpeyCePddaqD/download "Hinweis: Die Gitterkonstante wird hier mit g bezeichnet.")

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

Das optische Gitter hat 600 vertikale Spalte. Jeder Punkt, der von der Wellenfront erreicht wird, ist Ausgangspunkt einer Elementarwelle. Diese interferieren miteinander und es ergeben sich, je nach Gangunterschied $\Delta s$, Maxima und Minima. Immer wenn der Gangunterschied ein ganzzahliges Vielfaches der Wellenlänge ist, kommt es zur konstruktiven Interferenz, es tritt also ein Maximum auf.

Vorraussetzung für den Versuch ist ebenfalls, dass der Abstand zwischen Gitter und Schirm, in diesem Fall Gitter und Handy, viel größer ist als der Gangunterschied. So können die Wellen, welche zur Interferenzr am
Ort der Kamera beitragen, als parallel betrachtet werden. Da dies der Fall ist, kann Interferenz stattfinden und somit können auch Maxima registriert werden.


</div>

</section>

</details>

---

1. 2. Berechne die Wellenlänge des Infrarotlichts.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda$,956,nm)

</p>

<details style='margin-left:10%'>

<summary> Lösungshinweise </summary>

Du sollst die Wellenlänge des Infrarotlichtes berechnen. Dazu brauchst du zum einen den Winkel $\alpha$ zwischen dem Maximum nullter Ordnung und dem erster Ordnung. Es ist gegeben, dass zwischen den beiden Maxima
erster Ordnung ein Winkel von 70° zu messen ist. Demnach beträgt der gesuchte Winkel genau die Hälfte, also $\alpha=35°$. Es ist außerdem die Gitterkontante $g$ gesucht: In der Aufgabenstellung wird beschrieben, dass das Gitter 600 Spalte pro Millimeter hat. Mit dieser Angabe kannst du $g$ bestimmen.

<p>

@rangeQuiz2($g$,1.667e-6,m)

</p>

Der Beugungswinkel $\alpha_k$ in Abhängigkeit von der Wellenlänge und dem Maximum $k$-ter Ordnung wird durch folgende Formel beschrieben: $\sin(\alpha_k)=\frac{k\cdot\lambda}{g}$.

Durch Einsetzen und Umformen erhältst du die gesuchte Größe.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Du sollst die Wellenlänge $\lambda$ des Infrarotlichtes berechnen. Dazu brauchst du zum einen den Winkel $\alpha$ zwischen dem Maximum nullter Ordnung und dem erster Ordnung. Es ist gegeben, dass zwischen den beiden Maxima erster Ordnung ein Winkel von 70° beträgt. Demnach gilt: $\alpha_1=35^\circ$. Es ist außerdem die Gitterkontante $g$ gesucht: In der Aufgabenstellung wird beschrieben, dass das Gitter 600
Spalte pro Millimeter hat. Somit ergibt sich für :

$$ g = \frac{1}{600}\cdot 10^{-3}\,\mathrm{mm} = 1,67\cdot 10^{-6} m$$

Der Beugungswinkel $\alpha_k$ in Abhängigkeit von der Wellenlänge $\lambda$ wird durch folgende Formel beschrieben:

$$\sin(\alpha_k)=\frac{k\cdot\lambda}{g}$$

Durch Einsetzen uns umstellen erhältst du 

$$\lambda \approx 956\,\mathrm{nm}$$

</details>

---

> Der Versuch wird mit einem Gitter von 1200 Spalten pro Millimeter wiederholt.

1. 3. Begründe, weshalb man außer dem Maximum nullter Ordnung keine Maxima höherer Ordnung registriert.


<details style='margin-left:10%'>

<summary> Lösungshinweise </summary>

In diesem Versuchsaufbau kann der Beobachtungswinkel gegenüber dem Maximum nullter Ordnung höchstens 90° betragen. Überprüfe, ob der geforderte nötige Gangunterschied bei einem Winkel von 90° für eine konstruktive Interferenz erreicht werden kann.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Im Grenzfall des Winkels $\alpha=90^\circ$ entspricht der Gangunterschied $\Delta s$ genau der Gitterkonstante $g$. Im vorliegenden Beispiel ist die Gitterkonstante $g=833\,\mathrm{nm}$ __kleiner__ als die Wellenlänge $\lambda=956\,\mathrm{nm}$. Somit kann keine konstruktive Interferenz erreicht werden und ein Maximum erster Ordnung ist nicht zu beobachten.

</details>

---

1. 4. Bestimme die Anzahl der vertikalen Spalte pro Millimeter, die ein Gitter mindestens haben müsste, damit nur das Maximum nullter Ordnung zu registrieren ist.

<p style='margin-left:10%'>

@rangeQuiz2($n$,1046,Striche pro Millimeter)

</p>

<details style='margin-left:10%'>

<summary> Lösunghinweise </summary>

Der hier gefragte Grenzfall erfordert, dass die Gitterkonstante genau der Wellenlänge entspricht.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Der hier gefragte Grenzfall erfordert, dass die Gitterkonstante genau der Wellenlänge entspricht.

$$ g=\lambda= 956\,\mathrm{nm}$$

Dies entspricht

$ n = \frac{1}{\lamda} \ 10^3 = 1046 $ Striche pro Millimeter

</details>

---

> Weißes Licht des Wellenlängenbereichs von $420\,\mathrm{nm}$ bis $780\,\mathrm{nm}$ fällt senkrecht auf ein Gitter. Auf einem parallel hinter dem Gitter angebrachten Schirm sind  mehrere Spektren und ein weißer Streifen zu sehen.

2. 1. Erläutere diesen Sachverhalt.

<details style='margin-left:10%'>

<summary> Lösunghinweis </summary>

Überprüfe, an welcher Stelle der weiße Strich zu sehen ist. Es sollte einem Maximum entsprechen.

Auch die Spektren sind Maxima. Allerdings liegen die Maxima hier abhängig von der Wellenlänge an unterschiedlicher Position.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Der weiße Strich entspricht dem Maximum nullter Ordnung. Da die Position des Maximums nullter Ordnung unabhängig von der Wellenlänge ist, fallen hier die Maxima aller Wellenlängen aufeinander und es entsteht ein weißer Streifen.

Die Spektren entstehen am Ort der Maxima erster und höherer Ordnung.

Für größere Wellenlängen ist der Abstand der Maxima nullter und erster Ordnung $a$ größer als für kleine Wellenlängen.

</details>

---

> Das Spektrum erster Ordnung wird ab einem minimalen Beugungswinkel von $4,50^\circ$ beobachtet.

2. 2. Ermittle die Gitterkonstante.

<p style='margin-left:10%'>

@rangeQuiz2($g$,5.35e-6,m)

</p>

<details style='margin-left:10%'>

<summary> Lösunghinweis </summary>

Die näher am Maximum nultter Ordnung liegenden Maxima haben die kleinsten Wellenlängen. Der Rand des Spektrums gehört als zur kleinst möglichen Wellenlänge. Nutze diese, um die Gitterkonstante zu ermitteln.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Die kleinste Wellenlänge ist $420\,\mathrm{nm}$. Wenn der zugehörige Winkel $\alpha=4,50^\circ$ beträgt, ergibt sich als Gitterkonstante:

$$ g = \frac{\lambda}{\sin\alpha} = 5,35\cdot 10^{-6}\,\mathrm{m}$$

</details>

---

2. 3. Zeige, dass die Spektren erster und zweiter Ordnung voneinander getrennt sind.


<details style='margin-left:10%'>

<summary> Lösunghinweis </summary>

Damit die Spektren von einander getrennt sind, muss das Maximum zweiter Ordnung der kleinsten Wellenlänge unter einem größeren Winkel auftreten, als das Maximum erster Ordnung der größten Wellenlänge.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Das Maximum erster Ordnung, dass am weitesten von der Mitte entfernt ist, gehört zur größten Wellenlänge, d.h. $780\,\mathrm{nm}$. Es erscheint unter dem Winkel:

$$\alpha_1(780\,\mathrm{nm}) = \frac{780\,\mathrm{nm}}{g} = 8,38^\circ$$

Das Maximum zweiter Ordnung, dass am nächsten an der Mitte liegt, gehört zur kleinsten Wellenlänge, d.h. $420\,\mathrm{nm}$. Es erscheint unter dem Winkel:

$$\alpha_2(420\,\mathrm{nm}) = \frac{2\cdot420\,\mathrm{nm}}{g} = 9,03^\circ$$

Da $\alpha_1(780\,\mathrm{nm}) < \alpha_2(420\,\mathrm{nm})$ sind die Spektren getrennt.

---

Alternativ kann man argumentieren, dass die größte Wellenlänge ($780\,\mathrm{nm}$) kleiner ist als die doppelte kleinste Wellenlänge ($2\cdot420\,\mathrm{nm}$) und somit der zugehörige Winkel in der Formel

$$ \sin\alpha=\frac{k\cdot\lambda}{g} $$

für $780\,\mathrm{nm}$ kleiner ist als für $2\cdot420\,\mathrm{nm}$, da $\sin$ eine stetige Funktion ist.

</details>

---

2. 4. Berechne die Wellenlänge im Spektrum zweiter Ordnung, ab der sich die Spektren zweiter und dritter Ordnung überlappen.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_2$,630,nm)

</p>

<details style='margin-left:10%'>

<summary> Lösunghinweis </summary>

Das Spektrum der dritten Ordnung reicht in das Spektrum der zweiten Ordnung hinein. Die kleinste Wellenlänge ($420\,\mathrm{nm}$) definiert den Winkel $\alpha_3(420\,\mathrm{nm})$, bei welchem das Spektrum der dritten Ordnung beginnt. Überprüfe nun, welcher Wellenlänge im Spektrum zweiter Ordnung dieser Winkel entspricht.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Der kleinstmögliche Winkel des Spektrums dritter Ordnung $\alpha_3(420\,\mathrm{nm})$ ist gleich dem Winkel der gesuchten Wellenlänge im Spektrum zweiter Ordnung $\alpha_2(\lambda_2)$. Selbiges gilt natürlich auch für den Sinus dieser beiden Winkel.

$$ \sin\alpha_3(420\,\mathrm{nm}) = \sin\alpha_2(\lambda_2)$$

Der Sinus jedes Winkels kann über die Formel für das Interferenzmaximum berechnet werden $\sin\alpha=\frac{k\cdot\lambda_2}{g}.$ Eingesetzt für die beiden diskutierten Winkel ergibt sich

$$ \frac{3\cdot420\,\mathrm{nm}}{g}=\frac{2\cdot\lambda_2}{g} $$

Daraus ergibt sich

$$ \lambda_2 = 630\,\mathrm{nm} $$

</details>

## 10. 15. Interenz am Einzelspalt

{{2}}
*************
<section class="flex-container">

<div class="flex-child-2" style="min-width: 400px; margin-bottom: -10px">

![Einzelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/obZ2NPnD2TyRds8/download)<!-- style="width:100%"-->

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">


__Beschreibung:__ Beträgt der Gangunterschied $\Delta s$ zwischen den beiden Randstrahlen gerade $\lambda$, dann kann man zu jedem Strahl aus dem Lichtbündundel der @color(__einen Hälfte__, green) einen Strahl aus dem Bündel der @color(__anderen Hälfte__, purple) finden, dessen Gangunterschied gerade $\frac{\lambda}{2}$ beträgt.Es kommt folglich zu einer Auslöschung aller Wellen.

> Für das **erste Minimum** gilt: $$ \boxed{\sin\alpha=\frac{\lambda}{d}}$$
>
> Für das **erste Maximum** gilt: $$ \boxed{\sin\alpha=\frac{(2k+1)\frac{\lambda}{2}}{d}}$$ <br> _Hinweis: Die Nebenmaxima (d.h. $k\neq0$) sind beim Einzelspalt von sehr geringer Intensität._

</div>

</section>
*************

<iframe src="https://diversewolken.ddns.net/moodle/h5p/embed.php?url=https%3A%2F%2Fdiversewolken.ddns.net%2Fmoodle%2Fpluginfile.php%2F3413%2Fmod_h5pactivity%2Fpackage%2F0%2FEinzelspalt.h5p&amp;component=mod_h5pactivity" name="h5player" width="100%" height="800px"
   allowfullscreen="allowfullscreen" class="h5p-player w-100 border-0"
   style="height: 800px;" id="68ffc5eee8fae68ffc5eee8fb01-h5player">
</iframe><script src="https://diversewolken.ddns.net/moodle/h5p/h5plib/v124/joubel/core/js/h5p-resizer.js"></script>

{{1}}
*************

> -> [Simulation-LEIFI](https://www.leifiphysik.de/optik/beugung-und-interferenz/grundwissen/einzelspalt)
*************


## 10. 16. Intereferenz an dünnen Schichten

[Lernvideo-Interferenz-Dünne-Schichten](https://www.leifiphysik.de/optik/beugung-und-interferenz/grundwissen/interferenz-duennen-schichten)

### Aufgaben zu Interferenz an dünnen Schichten

1. [Quiz-Zur-Interferenz-An-Dünner-Schicht](https://www.leifiphysik.de/optik/beugung-und-interferenz/grundwissen/interferenz-duennen-schichten)

---

2. ![Interferenz-An-Dünner-Schicht](https://diversewolken.ddns.net/nextcloud/index.php/s/b2tedQNXs4LAHdT/download) Auf einer Wasseroberfläche schwimmt eine dünne Ölschicht. Das Wasser habe einen Brechungsindex $n_{H_2O}=1,333$, das Öl habe einen Brechungsindex von $n_{Öl}=1,2$.

2. 1. Erläutern Sie, warum das Öl auf der Pfütze bei Tageslicht in verschiedenen Farben schimmert.

2. 2. Ermitteln Sie den Winkel $\alpha$, unter welchem blaues Licht der Wellenlänge $440\,\mathrm{nm}$ destruktive Interferenz erfährt, wenn die Ölschicht eine Dicke von $600\,\mathrm{nm}$ besitzt. <br><br> _Hinweis: Der Gangunterschied der beiden Lichtstrahlen kann für eine dünne Schicht mit der Formel <br> $$ \Delta s = 2\cdot d\cdot\sqrt{n_{Öl}^2-sin^2(\alpha)} $$ ermittelt werden._

<p style='margin-left:10%'>

@rangeQuiz2($\alpha$,50.75,$^\circ$)

</p>

<details style='margin-left:10%'>

<summary> Lösungshinweise </summary>

Überlegen Sie, welche Bedingung für den Gangunterschied $\Delta s$ gilt, damit destruktive Interferenz auftritt.

[Lösungsvideo](https://www.youtube.com/watch?v=-0CPyBhD70o)

</details>


## 10. 17. Polarisation von Licht

[Experimentelle-Deutung-der-Polarisation](https://youtu.be/eYguAcvjN2o)

 
## 10. 18. Das Spektrum elektromagnetischer Wellen

![Wikipedia-Spektrum](https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/Electromagnetic_spectrum_-de_c.svg/1920px-Electromagnetic_spectrum_-de_c.svg.png)


{{1}}
****************
<iframe src="https://learningapps.org/watch?v=pgqf50hd225" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

_Bitte anschließend stichpunktartig übernehmen_
****************

## 10. 19. Interferometer

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Prinzipskizze:__

![Skizze-Interferometer](https://diversewolken.ddns.net/nextcloud/index.php/s/wjbdfpxRgZ5n6jx/download "Interferometer nach dem klassischen Beispiel von _Michelson und Morley_.")

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__

{{1}}
*************
> Interferometer sind Geräte, mit denen man Längenunterschiede sehr exakt bestimmen kann.
*************
{{2}}
*************
> Das einfallende Licht wird durch einen halbdurchlässigen Spiegel geteilt und legt dann zwei Wege $s_1$ und $s_2$ zurück.
*************
{{3}}
*************
> Das an den Spiegeln 1 und 2 reflektierte Licht gelangt zum Schirm. Der Gangunterschied $\Delta s = s_1 - s_2$ bewirkt eine Interferenz auf dem Schirm.
*************

</div>

</section>

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

{{6}}
**********
__Messwerte:__

| | | |
| $\lambda$ in nm | $f$ in $10^{14}\,$Hz | $U_g$ in V | $E_{kin}=U\cdot e$ in eV |
| 365 | | | |
| 405 | | | |
| 436 | | | |
| 546 | | | |
| 577 | | | |

@color(_Bereite die Tabelle vor. Ermittle bereits die zugehörigen Frequenzen._, blue)
**********

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
> Die Energie eines Photons
*********