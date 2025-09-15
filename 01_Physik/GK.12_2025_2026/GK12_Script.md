<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://cmscollege.ac.in/wp-content/uploads/2024/01/physics_image.webp

import: https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/settings.md

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

mode: presentation

-->


# GK Physik 12 2025/2026
<!-- 
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg 
-->

![WhyPhysics](https://cmscollege.ac.in/wp-content/uploads/2024/01/physics_image.webp)

@uhr

# LB VI Schwingungen

![Schwingungen](https://cmscollege.ac.in/wp-content/uploads/2024/01/physics_image.webp)

## (optional) Definition eines periodischen Vorgangs

!?[Motivationsvideo](https://diversewolken.ddns.net/nextcloud/index.php/f/719652/downlaod)

{{1}}
************
> Definition: Wir beobachten eine Größe $B$. Der Wert von B zum Zeitpunkt t wird mit $B(t)$ bezeichnet. Wir nennen B eine <span style="color:orange">***periodische Größe***</span>, wenn sich die Werte von B nach einer bestimmten Zeit T wiederholen.
Es soll gelten:

> $$ B(t) = B(t+T) $$ <br> _In Worten: Der Wert von B zum Zeitpunkt t ist genauso groß, wie der Wert von B zum Zeitpunkt t+T._

> <span style="color:red">***T heißt Periodendauer ***</span> von B
************

## 1. Beschreibung einer mechanischen Schwingung

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
> $$v(t) = v_{max} \cdot \cos(\omega \cdot t)$$
>
> $$a(t) = -a_{max} \cdot \sin(\omega \cdot t)$$


<p style="color:blue">

Aufgabe*: Ermittle für eine harmonische Schwinung aus dem Zusammenhang $y(t)$ die Ausdrücke für $v_{max}$ und $a_{max}$. Es gilt:

$v(t) = \frac{\mathrm{d}y}{\mathrm{d}t}$ und $a(t) = \frac{\mathrm{d}v}{\mathrm{d}t}$

<details>

<summary> Lösung </summary>

$$v_{max} = y_{max} \cdot \omega$$

$$a_{max} = y_{max} \cdot \omega^2$$

__Lösungsweg: Ableitung bilden__

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

## 2. Der Federschwinger

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

### Aufgaben zu 2. 1. Schwingungen

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

### Wiederholung Schwingungen

!?[LEIFI-Schwingungen](https://www.youtube.com/watch?v=hm_df3Oa_f8)

## 3. Definition mechanische Schwingung

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

$\Rightarrow$ B) Diskutieren Sie, welche Messgröße in Ihrem Setup die wesentliche Fehlerquelle ist. *Schätzen Sie dazu den absoluten Fehler der Messung begründet ein.

$\Rightarrow$ C) Überlegen Sie, wie auftretende Messfehler möglichest gering halten können. Schlagen Sie dazu geeignete Messungen vor und vermeiden Sie Aussagen wie: _Einfach genauer messen_.

---

Vergleichen Sie Ihre Überlegungen hier.

<details style="margin-left:10%">

<summary> Hinweise zum 1. Experiment </summary>

A) Mit Hilfe der Proportionalität zwischen Federdehnung $s$ und wirkender Kraft $F$ $$F=D \cdot s$$ lässt sich die Federkonstante D bestimmen. Dazu muss ein Massestück mit bekannter Masse $m$ genutzt werden. Die wirkende Kraft ist dann die Gewichtskraft $F_g$. Gemessen wird die Federdehnung $s$.

B) Da die Masse $m$ als sehr genau bekannt angenommen werden kann, ist die wesentliche Fehlerquelle die Messung der Federdehnung $s$. *Je nach Massband und Ablesemethode sollte man hier von einer Ungenauigkeit der Längenmessung von ca. 1-2mm ausgehen.

C)  Ist die Federdehnung nur sehr gering (d.h. mit einer sehr kleinen Masse), so ist der relative Fehler deutlich größer. Je stärker sich die Feder dehnt, desto geringer ist die Auswirkung der Ungenauigkeit. @color(Achtung: Feder nicht überdehnen., red)

</details>

     ---

<details style="margin-left:10%">

<summary> Hinweise zum 2. Experiment </summary>

A) Mit Hilfe einer Schwingung der Feder mit einem angehängten Massestück kann die Federkonstante bestimmt werden. Dazu muss die Schwingungsdauer $T$ ermittelt werden.

B) Da die Masse $m$ als sehr genau bekannt angenommen werden kann, ist die wesentliche Fehlerquelle die Messung der Periodendauer $T$. *Durch die Reaktionszeit des Menschen kann der zufällige Messfehler der Zeitmessung auf etwa $0,3s$ abgeschätzt werden.

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

$\Rightarrow$ E) Vergleichen Sie die Ergebnisse Ihrer beiden Messmethoden miteinander.

$\Rightarrow$ F*) Schätzen Sie für jede Ihrer Messungen den zufälligen Fehler ab. Vergleichen Sie die Größe beider Fehler miteinander. Schlussfolgern Sie daraus auf die Genauigkeit beider Messmethoden.


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


### Aufgaben zur Schwingung

Ein vertikaler Federschwinger besteht aus einer Feder mit der Federkonstante D = 2,5 N/m und einem angehängten Körper mit der Masse m = 0,10 kg. Der Abstand zwischen den Umkehrpunkten des schwingenden Körpers beträgt s = 10 cm.

- a)  Skizzieren Sie das y-t-Diagramm für mindestens eine Periode. Geben Sie eine Schwingungsgleichung mit den speziell vorgegebenen Werten an.

<details style="margin-left:5%">

<summary> Lösung a) </summary>

![Lsg_9.3_a](https://diversewolken.ddns.net/nextcloud/index.php/s/Ger7Mg4LraekEGn/download)

</details>

---

- b) Geben Sie für den Zeitpunkt t = 0,10 s die Elongation an.

<details style="margin-left:5%">

<summary> Lösung b) </summary>

![Lsg_9.3_a](https://diversewolken.ddns.net/nextcloud/index.php/s/LFxTxsAtHFTj5pg/download)

</details>

---

- c)  Geben Sie eine Möglichkeit an, wie durch Veränderung der gegebenen Größen die Frequenz des Oszillators halbiert werden kann. Begründen Sie Ihre Antwort.

<details style="margin-left:5%">

<summary> Lösung c) </summary>

![Lsg_9.3_c](https://diversewolken.ddns.net/nextcloud/index.php/s/2SyNqYTKqoRxHe4/download)

</details>

---

- d*) Ermitteln sie die maximale Geschwindigkeit des Massestücks. Geben Sie jeweils auch die zugehörigen Zeitpunkte an.

<details style="margin-left:5%">

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

</details>

---

- e) Entscheiden Sie für die folgenden Beispiele, ob es sich dabei um eine Schwingung (nach Definition handelt) oder nicht. Begründen Sie Ihre Aussage in jedem Fall.

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

## 4. Energieumwandlungen bei Schwingungen

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

{{4}}
***********
<p style="margin-left:10%">
@color(Wählen Sie die richtigen Aussagen. Nutzen Sie im Zweifel die Simulation., blue)

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

</p>
***********

## 5. Grundlagen Elektromagnetischer Schwingkreis

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

{{4}}
**********
     -> [PHeT-Simulation-AC-Circut](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac-virtual-lab/latest/circuit-construction-kit-ac-virtual-lab_all.html?locale=de)
**********

{{5}}
**********
__Energiebetrachtung:__

> In einem idealen Schwingkreis schwingt die Energie zwischen dem [[ elektrischen ]] Feld des Kondensators ([[ elektrische ]] Energie) und dem magnetischen Feld der Spule ([[ magnetische ]] Energie). Die Summe aus elektrischer und magnetischer Energie ist zu jedem Zeitpunkt [[ konstant ]]
**********

{{6}}
**********
__Periodendauer:__

> Die Periodendauer in einem idealen Schwingkreis wird durch die _Thomson'sche Schwingungsgleichung_ berechnet
>
> $$ T = 2\pi \sqrt{L\cdot C} $$
**********

{{7}}
**********
<p style="color:blue">

Erstellen Sie mit Hilfe der Simulation einen Schwingkreis, den Sie über einen Wechselschalter mit einer Batterie aufladen können.

1. Fügen Sie in die Simulation ein Spannungsdiagramm ein und messen Sie die Spannung vor und hinter dem Kondensator.

2. Fügen Sie in die Simulation eine Stopuhr ein. Ermitteln Sie mit Hilfe der Stopuhr und der angezeigten Schwingung die Periodendauer.

<p style="margin-left:10%">

@rangeQuiz20($T$, 4.44 ,$s$)

</p>

3. Wenn Sie den Kondensator bzw. die Spule anklicken, so werden Ihnen die Werte für $C$ bzw. $L$ angezeigt. Ermittlen Sie nun aus diesen Werten die Periodendauer mit Hilfe der _Thomson'schen Schwingungsgleichung_. Ermitteln Sie auch die Frequenz der Schwingung.

<p style="margin-left:10%">

@rangeQuiz2($T$, 4.443 ,$s$)

@rangeQuiz2($f$, 0.225 ,$Hz$)

</p>

4. Verändern Sie Ihren Schwingkreis derart, dass eine Frequenz von 1 Hz auftritt. Geben Sie das Produkt aus $L$ und $C$ an.

<p style="margin-left:10%">

@rangeQuiz2($C\cdot L$, 0.025 ,$s$)

</p>

</p>
**********


### Inputvideo zu 5.1

!?[Input-Video-5-1](https://youtu.be/R3blqyJjkV0)

### 5. 1. Eigenschaften idealer und realer Schwingkreise

-> [Simulation-Schwingkreis-Fendt](https://www.zum.de/ma/fendt/phde/oscillatingcircuit_de.htm)

> Bei einem @color(idealen,red) Schwingkreis ist die Summe aus elektrischer und magnetischer Energie konstant (Energieerhaltung).

> Bei einem @color(realen,red) Schwingkreis treten [[ Verluste ]] auf. Dabei wird die vorhandene elektrische und magnetische Energie in [[ Wärmenergie ]] umgewandelt. Der Grund für die Verluste ist der elektrische [[ Widerstand ]] der Bauelemente.


-> [PHeT-Simulation-AC-Circut](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac-virtual-lab/latest/circuit-construction-kit-ac-virtual-lab_all.html?locale=de)

<p style="color:blue;margin-left:10%">

Nutzen Sie für die folgende Aufgabe die Simulation:

1. Erstellen Sie einen idealen Schwingkreis. Der Kondensator soll zunächst mit 10V aufgeladen werden. Ergänzen Sie dazu zwei Schalter und eine Batterie (anklicken -> 10V).

---

2. Ändern Sie die Induktivität der Spule zu $2 H$ und die Kapazität des Kondensators zu $0,2 F$. Berechnen Sie die Frequenz der Schwingung.

<p style="margin-left:10%">

@rangeQuiz2($f$,0.2516,$Hz$)

</p>

---

3. Ergänzen Sie die Messung eines Spannungs-Zeit-Diagramms und bauen Sie einen elektrischen Widerstand ein. Klicken Sie auf den Widerstand und stellen Sie diesen auf $0\Omega$. Sie haben (immer noch) einen idealen Schwingkreis. Starten Sie die Aufnahme und vergleichen Sie Ihren Schwingkreis mit der Lösung.

<details style="margin-left:10%">

<summary> Lösung </summary>

![GedSk-Lsg3](https://diversewolken.ddns.net/nextcloud/index.php/s/D9yikcAirXjNECT/download)

</details>

---

4. ![SK-Pause](https://diversewolken.ddns.net/nextcloud/index.php/s/BRKdbFoA3AeXk5A/download) __Pausieren Sie nun Ihre Simulation.__

---

4. Öffnen Sie den rechten Schalter, schließen Sie den linken Schalter und laden Sie den Kondensator so wieder auf. Die Spannungsanzeige sollte bei 10V liegen. Klicken Sie auf den ohmschen Widerstand und stellen Sie den Wert $0,7\Omega$ ein.

5. Sie haben nun einen realen (gedämpften) Schwingkreis. Starten Sie Ihre Simulation erneut und beobachten Sie das Verhalten der Spannungsamplitude. Vergleichen Sie dieses Verhalten mit der Amplitude einer gedämpften mechanischen Schwingung (siehe 4.)



6. Pausieren Sie nun Ihre Simulation erneut. Laden Sie Ihren Kondensator durch Schließen des linken Schalters auf (die Spannung sollte 10V anzeigen). Öffnen Sie den Ladeschalter anschließend wieder.

7. Beobachten Sie nun, auf welchen Spannungswert die Amplitude nach einer vollständigen Schwingung fällt. Starten Sie dazu Ihre Simulation und notieren Sie den Wert $U_1=U(T)$ nach einer Periodendauer.

<p style="margin-left:10%">

@rangeQuiz2($U_1$,5,$V$)

</p>

8. Skizzieren Sie den qualitativen Verlauf U(t) eines gedämpften Schwingkreises in Ihre Aufzeichnungen.

9. Der Spannungsverlauf $U(t)$ eines _schwach_ gedämpften Schwingkreises kann mit der Formel $$ U(t) = U_0 \cdot e^{-k\cdot t} \cdot \cos(\omega t)$$ beschrieben werden, wobei $k$ die Dämpfung darstellt. Ermitteln Sie aus dem Ergebnis der Aufgabe 7. den Dampfungsfaktor.

<p style="margin-left:10%">

@rangeQuiz2($k$,0.1744,$\frac{1}{s}$)

</p>

<details style="margin-left:10%">

<summary> Lösungshinweise </summary>

Aus Aufgabe 7. ergibt sich die Spannung nach genau einer Periodendauer $U(T)=5V$. Nach genau einer Periodendauer ist $cos(\omega \cdot T)=1$. Somit vereinfacht sich die Formel für U(T) an diesem Punkt zu

$$ U(T) = U_0 \cdot e^{-k\cdot T}$$

Nutzen Sie den Solver Ihres CAS um den Wert für k zu ermitteln.

<details style="margin-left:10%">

<summary> Lösung </summary>

$$ Solve(5 = 10 \cdot e^{-x\cdot 3.974}, x)$$

$$ k \approx 0.174 \frac{1}{s}$$

</details>

</details>


</p>

### Aufgaben zu idealen und realen Schwingern

1. Eine Feder wird vertikal befestigt, mit einer Masse beschwert und vertikal ausgelenkt. Nun wird die Schwingungsdauer bestimmt. Der gleiche Versuch ( gleiche Feder, gleiche Masse) wird (in Gedanken) auf dem Mond durchgeführt. Wie ändert sich die Schwingungsdauer?

     [(x)] Gar nicht, da in der Gleichung für die Schwingungsdauer einer Feder der Ort des Versuches keinen Einfluß hat.
     [( )] Sie wird größer, da bei der Bestimmung der Federkonstante die Gewichtskraft Einfluß hat. Diese nimmt auf dem Mond ab und damit wird die Federkonstante größer
     [( )] Die Schwingungsdauer kann größer oder kleiner werden. Das hängt von der Auslenkung zu Beginn des Versuchs ab.

<details style="margin-left:10%">

<summary> Hinweise zur Lösung </summary>

Die Schwingungsdauer einer Feder ist von der Federkonstante D und der anhängenden Masse m abhängig. $T=2\cdot\pi\cdot\sqrt{\frac{m}{D}}$.
Die Federkonstante ist eine Größe, die nur von der Feder abhängt, nicht von dem Ort, an dem sich die Feder befindet. Die Masse ist ebenfalls überall gleich.

</details>

---

2. Ein Federpendel mit der Federkonstante $5,0 \frac{N}{m}$ führt harmonische Schwingungen aus. Das Diagramm stellt den Zusammenhang zwischen der Geschwindigkeit und der Zeit dar.

     ![Federschwinger-Diagramm](https://physikaufgaben.de/bild/a992_2.jpg) 

2. 1. Bestimmen Sie die Periodendauer und die Frequenz der Schwingung.

<p style="margin-left:10%">

@rangeQuiz2($T$,0.4,$s$)

@rangeQuiz2($f$,2.5,$Hz$)

</p>

---

2. 2. Ermitteln Sie die ersten beiden Zeitpunkte, an dem der Körper seine maximale Auslenkung von der Ruhelage erreicht.

<p style="margin-left:10%">

@rangeQuiz0($t_1$,0,$s$)

@rangeQuiz2($t_2$,0.2,$s$)

</p>

<details style="margin-left:10%">

<summary> Hinweise zur Lösung </summary>

Der Körper erreicht seine maximale Auslenkung, wenn die Geschwindigkeit gleich Null ist.

</details>

---

2. 3. Ermitteln Sie die Masse des schwingenden Körpers.

<p style="margin-left:10%">

@rangeQuiz2($m$, 0.02 ,$kg$)

</p>

<details style="margin-left:10%">

<summary> Hinweise zur Lösung </summary>

Mit Hilfe der Periodendauer und der Federkonstante lässt sich mit der Formel $T=2\pi\sqrt{\frac{m}{D}}$ die Masse ermitteln.

</details>

---

2. 4. Zeichnen Sie qualitativ ein Diagramm mit der Zeit auf der x-Achse in dem Sie sowohl den Graph $v(t)$ als auch den Graph $y(t)$ eintragen.

<details style="margin-left:10%">

<summary> Lösung </summary>

![Lsg_2-4](https://physikaufgaben.de/bild/a992_3.jpg)

</details>

---

2. 5. Ermitteln Sie die maximale Auslenkung des Systems. Nutzen Sie dazu die Zusammenhänge für $y_{max}$ aus $v_{max}$ aus Teil _1. Beschreibung einer mechanischen Schwingung_.

<p style="margin-left:10%">

@rangeQuiz2($y_{max}$, 0.0095 ,$m$)

</p>

<details style="margin-left:10%">

<summary> Hinweise zur Lösung </summary>

In der Aufgabe aus _1. Beschreibung einer mechanischen Schwingung_ wurde gezeigt, dass

$$y(t) = y_{max} \cdot \sin(\omega\cdot t)$$

$$v(t) = v_{max} \cdot \cos(\omega\cdot t)$$

$$a(t) = a_{max} \cdot -\sin(\omega\cdot t)$$

wobei

$$v_{max} = y_{max} \cdot \omega$$

$$a_{max} = y_{max} \cdot \omega^2$$

gilt. Nutzen Sie den Ausdruck für $v_max$ zur Bestimmung von $y_{max}$.

<details style="margin-left:10%">

<summary> Lösung </summary>

$$v_{max} = y_{max} \cdot \omega$$

mit $\omega=\frac{2\pi}{T}$ ergibt

$$ y_{max} = \frac{v_{max}\cdot T}{2\pi} = 9.55\cdot 10^{-3} m $$

</details>

</details>

---

3. Bei jeder (realen) mechanischen Schwingung wird Energie durch Reibung an die Umgebung abgegeben. Im Experiment wird der Schwingungsverlauf bei laminarer Reibung des Federpendels in Wasser aufgenommen. Die Federkonstante beträgt $D=10\frac{N}{m}$.

     ![Aufgabe-Gedaempfte-Schwingung](https://diversewolken.ddns.net/nextcloud/index.php/s/gYaziaBmrreoNbF/download)

     Der Graph kann näherungsweise durch die Gleichung $s(t)=\hat{s}\cdot e^{-k\cdot t}\cdot \cos(\omega\cdot t)$ beschrieben werden. Bestimmen Sie aus dem Graphen die Größen $\hat{s}$, $k$, $\omega$ und $f$.

<p style="margin-left:10%">

@rangeQuiz2($\hat{s}$, 0.04 ,$m$)

@rangeQuiz2($k$, 0.575 ,$\dfrac{1}{s}$)

@rangeQuiz2($\omega$, 12.566 ,$\dfrac{1}{s}$)

@rangeQuiz2($f$, 2 ,$Hz$)

</p>

## 6. Mechanische Wellen

__Motivation:__

{{0-1}}
*************
!?[Binogi-Wellen](https://app.binogi.de/l/wellen)
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


### 6. 1. Arten mechanischer Wellen

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

### 6. 2. Eigenschaften mechanischer Wellen

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

3. Wählen Sie die korrekte Wellengleichung $y(t)$ für den Ort $x=0\,\mathrm{m}$.

<p style="margin-left:10%">

[[ $y(t) = 1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | $y(t) = 1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | ($y(t) = -1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$) | $y(t) = -1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ ]]

</p>

4. Wählen Sie die korrekte Wellengleichung $y(x)$ für den Zeitpunkt $t=0\,\mathrm{s}$.

<p style="margin-left:10%">

[[ $y(x) = 1,5\,\mathrm{m}\cdot\sin(0,1\,\mathrm{\frac{1}{m}}\cdot x)$ | $y(x) = 1,5\,\mathrm{m}\cdot\cos(0,1\,\mathrm{\frac{1}{m}}\cdot x)$ | ($y(x) = -1,5\,\mathrm{m}\cdot\sin(0,1\,\mathrm{\frac{1}{m}}\cdot x)$) | $y(x) = -1,5\,\mathrm{m}\cdot\cos(0,1\,\mathrm{\frac{1}{m}}\cdot x)$ ]]

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