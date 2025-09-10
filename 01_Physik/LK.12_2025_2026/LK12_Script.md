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
> Bei einem schwingenden System kann eine @color(periodische äußere Anregung, red) dem System permanent Energie zuführen. Die äußere Anregung erfolgt dabei mit rregerfrequenz $f_E$. Die Frequenz des frei schwingenden Systems wird als  @color(Eigenfrequenz, red) $f_0$ bezeichnet. Eine solche äußere Anregung nennt man @color(erzwungene Schwingung, red).
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

- Gleichung 3. muss nach $\mathrm{d}t$ umgestellt werden

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