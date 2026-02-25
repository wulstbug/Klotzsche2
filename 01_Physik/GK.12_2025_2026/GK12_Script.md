<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://cmscollege.ac.in/wp-content/uploads/2024/01/physics_image.webp

import: https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/settings.md

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

# LB VI Schwingungen und Wellen

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

## Checkliste zur LK


__Checkliste zur 1. LK __

- Beschreibung einer harmonischen mechanischen Schwingung y(t), v(t), a(t) und Ermittlung der Maximalgeschwindigkeit / Beschleunigung

- Mechanische Schwingung am Beispiel des Federschwingers, Grundannahmen für harmonische Schwingung, Periodendauer, Begriffe der mechanischen Schwingung (z.B. Elongation, Amplitude)

- Verständnis des Messens einer Periodendauer am Beispiel des Federschwingers

- Energieumwandlungen bei mechanischen Schwingungen

- realer/idealer mechanischer Schwinger

- Aussagen zu mechanischen Schwingungen einschätzen

- Grundlagen des elektrischen Schwingkreises (Energieumwandlungen)

- Eigenschaften des elektrischen Schwingkreises (Periodendauer, idealer/realer Schwingkreis)

- Vergleich / Gemeinsamkeiten & Unterschieder mechanischer Schwinger / Schwingkreis


## 6. (Teil 1) Mechanische Wellen

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


#### Aufgaben zur Charakterisierung von Wellen

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

### 6. 3. Darstellung der Wellenausbreitung mit Wellenfront und Wellennormale

Zur Darstellung der Ausbreitung von Wellen nutzt man __Wellenfronten__ und @color(__Wellennormale__,red)

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

### 6. 4. Huygens'sche Prinzip

> Jeder Punkt einer Wellenfront ist seinerseits wieder Ausgangspunkt für @color(kreis- bzw. kugelförmige Elementarwellen, red)

{{1}}
*************
![Huygernssches-Prinzip](https://diversewolken.ddns.net/nextcloud/index.php/s/zE2kb4mDwinM5M2/download)


-> [Simulation-Ausbreitung-Kreiswelle-EbeneWelle](https://www.leifiphysik.de/mechanik/mechanische-wellen/ausblick/huygenssches-prinzip-zur-beschreibung-von-mechanischen-wellen)
*************


#### Aufgabenstellung zur Selbsständigen Präsentation

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


### 6. 5. Reflexion

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


### 6. 6. Brechung


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

### 6. 7. Beugung

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

??[Simulation-Kante](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+489+1.5625e-8%0Aw+0+260+133+515+133%0AS+2+0+1+511+1+0+1.399998+0+10+100+1+0%0A)
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


#### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)

### 6. 8. Interferenz

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

***********

### 6. 9. Stehende Wellen

<iframe src="https://www.geogebra.org/classic/wcqzrbnh?embed" width="100%" height="600px" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

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

![StehendeWellenGitarre](https://diversewolken.ddns.net/nextcloud/index.php/s/nERJCb4RJEyjYji/download)

#### Übungsaufgaben zu Wellenphänomenen

##### Übung 1 - Welleneigenschaften

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

##### Übung 2 - Wellenphänomene

Ordne den folgenden Abbildungen das Wellenphänomen zu.

<iframe src="https://learningapps.org/watch?v=p29hwaena25" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

##### Übung 3 - Stehende Wellen

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

## 6. (Teil II) Elektromagnetische Wellen

### 6. 10. Das Doppelspalt-Experiment

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
6. Es gilt die Wellenausbreitunggleichung: <br> $$ \boxed{c = \lambda \cdot f}$$ <br> Die Wellenlänge $\lambda$ der Lichtwelle bestimmt die <span style="color:orange">***Lichtfarbe***</span>.
*********

</div>

</section>


*********

### 6. 11. Bestimmung der Wellenlänge des Lichts am Doppelspalt

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

#### Aufgaben zum Thema _Licht als Welle_

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


### 6. 12. Interferenz am Beugungsgitter

> [Video: Ausführliche Erklärung zur Interferenz am Gitter](https://www.youtube.com/watch?v=FedzH3QNptQ&t=201s)

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


#### Experimentelle Aufgabe zum optischen Gitter

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

@rangeQuiz20($b$,12.5e-6,m)

</p>


#### Abituraufgabe zum optischen Gitter

> In einem Experiment fällt das Infrarotlicht einer Fernbedienung senkrecht auf ein Gitter mit 600 vertikalen Spalten pro Millimeter. Eine Handy-Kamera wird auf einem Halbkreis um das Gitter geführt (siehe Abbildung 1). Sie registriert dabei die Intensität des Infrarotlichts. Der Winkel zwischen den beiden Maxima erster Ordnung beträgt 70°.

![Abituraufgabe_Messaufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/NomQLdczLDTFp4m/download "Abbildung 1: Messaufbau")

1. 1. Erläutere mithilfe einer Skizze, wie an einem optischen Gitter Maxima der Intensität unter einem bestimmten Beobachtungswinkel aufgezeichnet werden können.

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
erster Ordnung ein Winkel von 70° zu messen ist. Demnach beträgt der gesuchte Winkel genau die Hälfte, also $\alpha=35°$. Es ist außerdem die Gitterkontante $b$ gesucht: In der Aufgabenstellung wird beschrieben, dass das Gitter 600 Spalte pro Millimeter hat. Mit dieser Angabe kannst du $b$ bestimmen.

<p>

@rangeQuiz2($b$,1.667e-6,m)

</p>

Der Beugungswinkel $\alpha_k$ in Abhängigkeit von der Wellenlänge und dem Maximum $k$-ter Ordnung wird durch folgende Formel beschrieben: $\sin(\alpha_k)=\frac{k\cdot\lambda}{b}$.

Durch Einsetzen und Umformen erhältst du die gesuchte Größe.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Du sollst die Wellenlänge $\lambda$ des Infrarotlichtes berechnen. Dazu brauchst du zum einen den Winkel $\alpha$ zwischen dem Maximum nullter Ordnung und dem erster Ordnung. Es ist gegeben, dass zwischen den beiden Maxima erster Ordnung ein Winkel von 70° beträgt. Demnach gilt: $\alpha_1=35^\circ$. Es ist außerdem die Gitterkontante $g$ gesucht: In der Aufgabenstellung wird beschrieben, dass das Gitter 600
Spalte pro Millimeter hat. Somit ergibt sich für :

$$ b = \frac{1}{600}\cdot 10^{-3}\,\mathrm{mm} = 1,67\cdot 10^{-6} m$$

Der Beugungswinkel $\alpha_k$ in Abhängigkeit von der Wellenlänge $\lambda$ wird durch folgende Formel beschrieben:

$$\sin(\alpha_k)=\frac{k\cdot\lambda}{b}$$

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

$$ b=\lambda= 956\,\mathrm{nm}$$

Dies entspricht

$ n = \frac{1}{\lamda} \ 10^3 = 1046 $ Striche pro Millimeter

</details>

---

> Weißes Licht des Wellenlängenbereichs von $420\,\mathrm{nm}$ bis $780\,\mathrm{nm}$ fällt senkrecht auf ein Gitter. Auf einem parallel hinter dem Gitter angebrachten Schirm sind mehrere Spektren und ein weißer Streifen zu sehen.

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

@rangeQuiz2($b$,5.35e-6,m)

</p>

<details style='margin-left:10%'>

<summary> Lösunghinweis </summary>

Die näher am Maximum nultter Ordnung liegenden Maxima haben die kleinsten Wellenlängen. Der Rand des Spektrums gehört als zur kleinst möglichen Wellenlänge. Nutze diese, um die Gitterkonstante zu ermitteln.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

Die kleinste Wellenlänge ist $420\,\mathrm{nm}$. Wenn der zugehörige Winkel $\alpha=4,50^\circ$ beträgt, ergibt sich als Gitterkonstante:

$$ b = \frac{\lambda}{\sin\alpha} = 5,35\cdot 10^{-6}\,\mathrm{m}$$

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

$$\alpha_1(780\,\mathrm{nm}) = \frac{780\,\mathrm{nm}}{b} = 8,38^\circ$$

Das Maximum zweiter Ordnung, dass am nächsten an der Mitte liegt, gehört zur kleinsten Wellenlänge, d.h. $420\,\mathrm{nm}$. Es erscheint unter dem Winkel:

$$\alpha_2(420\,\mathrm{nm}) = \frac{2\cdot420\,\mathrm{nm}}{b} = 9,03^\circ$$

Da $\alpha_1(780\,\mathrm{nm}) < \alpha_2(420\,\mathrm{nm})$ sind die Spektren getrennt.

---

Alternativ kann man argumentieren, dass die größte Wellenlänge ($780\,\mathrm{nm}$) kleiner ist als die doppelte kleinste Wellenlänge ($2\cdot420\,\mathrm{nm}$) und somit der zugehörige Winkel in der Formel

$$ \sin\alpha=\frac{k\cdot\lambda}{b} $$

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

Der Sinus jedes Winkels kann über die Formel für das Interferenzmaximum berechnet werden $\sin\alpha=\frac{k\cdot\lambda_2}{b}.$ Eingesetzt für die beiden diskutierten Winkel ergibt sich

$$ \frac{3\cdot420\,\mathrm{nm}}{b}=\frac{2\cdot\lambda_2}{b} $$

Daraus ergibt sich

$$ \lambda_2 = 630\,\mathrm{nm} $$

</details>

#### Vorbereitungsaufgaben zum Praktikum - _Licht als Welle_

1. ![SVG-OptischesGitter](https://diversewolken.ddns.net/nextcloud/index.php/s/m5xBAtFZpnZ95yi/download)<!-- style="max-width:300px"--> Paralleles weißes Licht (Frequenzintervall: $3{,}747 \cdot 10^{14} \, \mathrm{Hz} \leq f \leq 7{,}495 \cdot 10^{14} \, \mathrm{Hz}$) einer Glühlampe trifft senkrecht auf ein optisches Gitter. Das Interferenzbild wird auf einen $1{,}00 \, \mathrm{m}$ entfernten Schirm projiziert. Links und rechts vom Maximum $0$. Ordnung wird für die $1.$ Ordnung ein vollständig kontinuierliches Farbspektrum sichtbar.

1. 1. Berechnen Sie für die Grenzen des Frequenzintervalls die zugehörigen Wellenlängen und ordnen Sie diesen die Farben Rot und Violett zu.

<p style='margin-left:10%'>

__Untere Grenze:__ 

<p style='margin-left:5%'>

@rangeQuiz2($\lambda_u$,800.64,nm)

Farbe: [[ (rot) | violett ]]

</p>

__Obere Grenze:__ 

<p style='margin-left:5%'>

@rangeQuiz2($\lambda_o$, 400.27,nm)

Farbe: [[ rot | (violett) ]]

</p>

</p>

<details style='margin-left:10%;color:blue'>

<summary> Lösungshinweise </summary>

Überprüfen Sie mit Hilfe Ihrer Aufzeichnungen, welche Gleichung für Wellen die Frequenz und die Wellenlänge beinhaltet. Nutzen Sie für die fehlende Größe der Gleichung den Wert im Vakuum. Nutzen Sie die Formelsammlung für die Zuordnung der Farben. 

</details>

<details style='margin-left:10%;color:blue'>

<summary> Lösung </summary>

Nutzen Sie die Wellenausbreitungsgleichung und die Lichtgeschwindigkeit im Vakuum um die Wellenlänge zu berechnen. 


$$ \lambda_u = \frac{c}{f_u} = \frac{3\cdot 10^8\,\mathrm{\frac{m}{s}}}{3{,}747 \cdot 10^{14} \, \mathrm{Hz}} = 800,64\,\mathrm{nm}$$

und

$$ \lambda_o = \frac{c}{f_o} = \frac{3\cdot 10^8\,\mathrm{\frac{m}{s}}}{7{,}495 \cdot 10^{14} \, \mathrm{Hz}} = 400,27\,\mathrm{nm}$$



Nutzen Sie anschließend die Formelsammlung (S. 65) um den Wellenlängen die Farben zuzuordnen.

</details>

---

1. 2. Der Abstand des Maximums $1.$ Ordnung für das Licht der größten Frequenz von der Mitte des Maximums $0.$ Ordnung beträgt genau $10{,}0 \, \mathrm{cm}$. <br> Überprüfen Sie, ob für diese Messergebnisse die _Kleinwinkelnäherung_ angewendet werden kann (Bründung erforderlich).

<p style='margin-left:10%'>

_Kleinwinkelnäherung_ kann [[ angewendet | (nicht angewendet) ]] werden.

</p>

<details style='margin-left:10%; color:blue'>

<summary> Lösungshinweise </summary>

Ermitteln Sie den Winkel $\alpha$. 

<p style='margin-left:10%'>

@rangeQuiz2($\alpha$,5.71,°)

</p>

Recherchieren Sie in Ihren Unterlagen, welcher Bedingung der Winkel genügen muss, damit die _Kleinwinkelnäherung_ angewendet werden darf.

</details>

<details style='margin-left:10%; color:blue'>

<summary> Begründung </summary>

Der Winkel $\alpha$ beträgt in diesem Experiment: $$\alpha = \tan^{-1}\big(\frac{a}{e}\big)=\tan^{-1}\big(\frac{0.1\,\mathrm{m}}{1\,\mathrm{m}}\big)= 5,7^\circ$$

Als Regel gilt: Wenn $\alpha<5^\circ$ kann die Kleinwinkelnäherung angewendet werden. Das ist hier nicht der Fall.

</details>

---


1. 3. Berechnen Sie anschließend die Gitterkonstante (unter Nutzung der Angaben aus 1.2.) und die Breite eines solchen Spektrums.

<p style='margin-left:10%'>

@rangeQuiz2($b$,4.02,µm ->Gitterkonstante)

@rangeQuiz2($B$,0.103,m ->Breite des Spektrums)

</p>


<details style='margin-left:10%; color:blue'>

<summary> Lösungshinweise </summary>

Nutzen Sie für die Gitterkonstante den in Aufgabe 1. 2. ermittelten Winkel $\alpha=5,71\,^\circ$, um mit der Wellenlänge $\lambda_o$ (1. 1.) die Gitterkonstante zu berechnen.

Für die größere Wellenlänge $\lambda_u$ (kleinere Frequenz) befindet sich das Maximum 1. Ordnung in einem anderen Abstand vom Maximum 0. Ordnung. Der Abstand der beiden Maxima erster Ordnung ergibt die Breite des Spektrums.

</details>

<details style='margin-left:10%; color:blue'>

<summary> Lösung $b$ </summary>

Der Winkel $\alpha$ beträgt in diesem Experiment: $$\alpha = 5,71^\circ$$

Die zur größten Frequenz gehörende Wellenlänge beträgt $$ \lambda_o = 400\,\mathrm{nm}$$

Mit der Formel $\sin\alpha=\frac{\lambda}{b}$ ergibt sich die Gitterkonstante $b$ zu:

$$ b = \frac{\lambda}{\sin\alpha} = \frac{400\cdot10^{-9}\,\mathrm{m}}{\sin(5,71^\circ)} = 4,02\cdot10^{-6}\,\mathrm{m}=4,02\,\mathrm{\mu m} $$

</details>

<details style='margin-left:10%; color:blue'>

<summary> Lösung $B$ </summary>

Für das rote Licht ($\lambda_u=800\,\mathrm{nm}$) ergibt sich der Winkel $\alpha$ zu

$$\alpha=\sin^{-1}\big(\frac{\lambda_u}{b}\big) = \sin^{-1}\big(\frac{800\cdot 10^{-9}\,\mathrm{m}}{4,02\cdot10^{-6}\,\mathrm{m}}\big) = 11.49\,^\circ$$

Bei einem Schirmabstand von $e=1\,\mathrm{m}$ ergibt sich der Abstand des ersten Maximums $a$ zu 

$$ a = \tan\alpha\cdot e = 0,203\,\mathrm{m}$$

Das Farbspektrum erstreckt sich vom Maximum des violetten Lichts bis zum Maximum des roten Lichts und ist somit

$$B = 0,203\,\mathrm{m}-0,1\,\mathrm{m}=0,103\,\mathrm{m}$$

breit.

</details>

---

1. 4. *Ermitteln Sie den prozentualen Fehler $\frac{\Delta b}{b}$ bei der Berechnung der Gitterkonstante $b$ zwischen der exakten Lösung (siehe Aufgabe 1. 3.) und der Berechnung mittels _Kleinwinkelnäherung_. Interpretieren Sie Ihr Ergebnis.

<p style='margin-left:10%'>

@rangeQuiz20($\frac{\Delta b}{b}$,0.5,%)

</p>


<details style='margin-left:10%; color:blue'>

<summary> Lösungshinweise </summary>

Ermitteln Sie die Gitterkonstante $b_{KW}$ mit den Angaben aus 1. 2., wenn Sie die _Kleinwinkelnäherung_ $\sin\alpha=\tan\alpha$ anwenden. <br> Nutzen Sie das Ergebnis für $b$ aus Aufgabe 1. 3. <br> Ermitteln Sie anschließend die Abweichung mit $\Delta b = b - b_{KW}$ und ermitteln Sie die prozentuale Abweichung:

$$ \frac{\Delta b}{b} $$

</details>

<details style='margin-left:10%; color:blue'>

<summary> Lösung $ \frac{\Delta b}{b} $ </summary>

Wenn man für die Angaben $\lambda_o = 400\,\mathrm{nm}$, Schirmabstand $e=1\,\mathrm{m}$ und Abstand $a=0,1\,\mathrm{m}$ die _Kleinwinkelnäherung_ ($\sin\alpha=\tan\alpha$):

$$\dfrac{\lambda}{b_{KW}} = \dfrac{a}{e}$$

ansetzt, ergibt sich für $b_{KW}$ der Wert:

$$ b_{KW} = \dfrac{\lambda\cdot e}{a} = 4\,\mathrm{\mu m}$$

Und der prozentuale Unterschied

$$ \frac{\Delta b}{b} = \frac{b - b_{KW}}{b} = \frac{0,02\,\mathrm{\mu m}}{4\,\mathrm{\mu m}} = 0.5 \,\mathrm{\%}$$

Der Fehler, welcher bei der Berechnung der Gitterkonstante durch _Kleinwinkelnäherung_ gemacht wird liegt im Sub-Prozentbereich und ist somit sehr klein.

</details>

## 6. 13. Das Spektrum elektromagnetischer Wellen

![Wikipedia-Spektrum](https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/Electromagnetic_spectrum_-de_c.svg/1920px-Electromagnetic_spectrum_-de_c.svg.png)

<iframe src="https://learningapps.org/watch?v=pgqf50hd225" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

_Bitte anschließend stichpunktartig übernehmen_

## Einstein's Rede zur Funkausstellung 1930

??[RedeEinstein](https://collections.ushmm.org/search/catalog/irn1004136)


### Checkliste für Klausur 12/1__

__Schwingungen:__

- Beschreibung mechanischer Schwingungen mit Hilfe der physikalischen Größen

- zugehörige Gleichungen für harmonische Schwingungen in sin und cos-Form

- Zusammenhänge der Größen y(t), v(t), a(t)

- Anwendung der Grundlagen/physikalischen Beschreibungen auf das Beispielsystem Federschwinger, Periodendauer

- Bedingungen für harmonische Schwingungen

- Energieumwandlungen bei mechanischen Schwingungen / Energieerhaltung, auch am Beispiel Federschwinger

- Grundlagen des elektromagnetischen Schwingkreises, Aufbau, schwingende physikalische Größen, Energieumwandlungen, Thomson'sche Schwingungsgleichung

__Wellen:__

- Beschreibung von mechanischen Wellen als sich im Raum ausdehnende Schwingungen, zeitliche und örtliche Darstellung als Gleichung und in Diagramm-Form

- Arten und Eigenschaften mechanischer Wellen, Darstellung von Wellen mit Wellenfront und Wellennormale

- Wellenphänomene (Reflexion, Beugung, Brechung, Interferenz) und deren Erklärung mit Hilfe des Huygens'schen Prinzips, stehende Wellen

- Wellengleichungen und Wellenausbreitungsgleichung

- Licht als elektromagnetische Welle, Eigenschaften von Lichtwellen, Experimente zur Interferenz mit elektromagnetischen Wellen am Doppelspalt und optischem Gitter




# LB VII - Einführung in die Quantenphysik

![Schrödingers-Katze](https://static.wixstatic.com/media/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg/v1/fill/w_740,h_493,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/56b499_f968ac3986d649a09a223676e4292365~mv2.jpg)

## Lesch's Kosmos - Einführung in die Quantenphysik

!?[Wie funktioniert Quantenmechanik? Quantenphysik erklärt Teil 1 | Harald Lesch | Terra X Lesch & Co](https://www.youtube.com/watch?v=cWf1OUVUObw)

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

### Video zum Photoeffekt

!?[Photoeffekt-Video](https://www.youtube.com/watch?v=Xm8LAEA7Gy8)

## 7. 2. Experiment: Der äußere lichtelektrische Effekt (Photoeffekt)

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

## 7. 3. Die Gegenfeldmethode beim Photoeffekt

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Versuchsaufbau:__

![Gegenfeldmethode-Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/w3iQGHQEGejyTt8/download)

</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__


{{1}}
*************
- eine Metallelektrode (Kathode) wird mit monochromatischem Licht beleuchtet}
*************


{{2}}
*************
- werden Elektronen aus dem Metall herausgelöst, so erhalten sie eine kinetische Energie $E_{kin}$
*************

{{3}}
*************
- aufgrund der emitierten Elektronen kann man zwischen Kathode und Anode einen elektrischen Stromfluss $I$ beobachten
*************

{{4}}
*************
- legt man zwischen Kathode und Anode eine __Gegenspannung__ $U_g$ an, so werden die Elektronen durch $U_g$ abgebremst, sie erhalten durch die Spannung die kinetische Energie $U \cdot e$ ($e$ .. Elementarladung)
*************

{{5}}
*************
- wählt man $U_g$ gerade so groß, dass kein Strom mehr zwischen Kathode und Anode fließt, so entspricht die zugeführte Energie $U\cdot e$ gerade der kinetischen Energie der Elektronen
*************

</div>

</section>


{{6-7}}
**********************
__Messwerte:__

| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $10^{-19}\mathrm{J}$ |
| 365 | | | |
| 405 | | | |
| 436 | | | |
| 546 | | | |
| 577 | | | |
**********************

{{7-8}}
**********************
__Messwerte:__

| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $10^{-19}\mathrm{J}$ |
| 365 | 8.22 | | |
| 405 | 7.41 | | |
| 436 | 6.88 | | |
| 546 | 4.49 | | |
| 577 | 5.20 | | |
**********************

{{8-9}}
**********************
__Messwerte:__

| | | |
| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $10^{-19}\mathrm{J}$ |
| 365 | 8.22 | 1.61 | 2.58 |
| 405 | 7.41 | 1.32 | 2.11 |
| 436 | 6.88 | 1.16 | 1.86 |
| 546 | 4.49 | 0.52 | 0.83 |
| 577 | 4.20 | 0.46 | 0.74 |
**********************


<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

{{9}}
**********************
__Messwerte:__


| $\lambda$ in $\mathrm{nm}$  | $f$ in $10^{14}\,$$\mathrm{Hz}$  | $U_g$ in $\mathrm{V}$ | $E_{kin}=U_g\cdot e$ in $10^{-19}\mathrm{J}$ |
| 365 | 8.22 | 1.61 | 2.58 |
| 405 | 7.41 | 1.32 | 2.11 |
| 436 | 6.88 | 1.16 | 1.86 |
| 546 | 4.49 | 0.52 | 0.83 |
| 577 | 4.20 | 0.46 | 0.74 |
**********************

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

{{9}}
**********************
__Diagramm f(E):__

<!--
     data-show
     data-title=""
     data-type="scatter"
     data-xlabel="f in 10¹⁴ Hz"
     data-ylabel="E in 10⁻¹⁹ J"
     data-xlim="0,10"
     data-ylim="-3,3"
-->
| f  | E |
| :---:| :---:|
| 8.22 | 2.58 |
| 7.41 | 2.11 |
| 6.88 | 1.86 |
| 4.49 | 0.83 |
| 4.20 | 0.74 |
**********************

</div>

</section>

{{6-9}}
**********************
<p style="color:blue">
0. _Bereite die Tabelle vor. Ermittle bereits die zugehörigen Frequenzen._

1. _Ergänze die gemessenen Daten $U_g$ für die verschiedenen Wellenlängen und berechne $E_{kin}$._ 

2. _Zeichne ein Diagramm der $E_{kin}(f)$._

3. _Zeichne eine geeignete Ausgleichsgerade und ermittle den Anstieg $h = \frac{\Delta E_{kin}}{\Delta f}$._
</p>
**********************


## 7. 3. Die Gegenfeldmethode beim Photoeffekt (SuS)

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

---

__Einsteinsche Geraden:__

![EinsteinscheGeraden](https://diversewolken.ddns.net/nextcloud/index.php/s/ETDwWWQqHPkBkxs/download)

---

__Anstieg der Einstein'schen Geraden:__

![AnstiegEinsteinscheGeraden](https://diversewolken.ddns.net/nextcloud/index.php/s/A9RwrenXmgbaady/download)

---

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

[[x]] Je kurzwelliger das Licht (oberhalb der Grenzfrequenz), desto höher ist die kinetische Energie der ausgelösten Elektronen.
[[ ]] Wird die Intensität des Lichts verstärkt, erhöht sich die Geschwindigkeit der herausgelösten Elektronen.
[[x]] Die Energie des Lichtes ist von der Frequenz abhängig.
[[ ]] Die Grenzfrequenz hängt vom Licht ab.
[[ ]] Das Plancksche Wirkungsquantum hängt vom verwendeten Katodenmaterial ab.
[[x]] Erhöht man die Intensität des Lichts (oberhalb der Grenzfrequenz), erhöht man auch die Anzahl der ausgelösten Elektronen.


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

3. Albert Einstein bekam im Jahre 1921 den Physiknobelpreis für die Erklärung des Photoeffektes, bei dem unter bestimmten Bedingungen Elektronen aus einer Metalloberfläche austreten, wenn diese mit Licht bestrahlt wird. Mit Hilfe der Gegenspannungsmethode kann z.B. der Zusammenhang zwischen der Frequenz des eingestrahlten Lichtes und der maximalen Geschwindigkeit der ausgelösten Elektronen bestimmt werden. Welches Diagramm stellt den Zusammenhang zwischen den beiden Größen am besten dar? <br> ![Diagramme_Photoeffekt](https://physikaufgaben.de/bild/a1044_1.jpg)

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

4. [Bitte anklicken: Verständnisfragen-Photoeffekt-KI-Gestützt](http://10.102.1.3:3001/?q=Stelle%20mir%20f%C3%BCnf%20Verst%C3%A4ndnisfragen%20zum%20Thema%20Photoeffekt,%20d.h.%20Experimentprinzip,%20Gegenfeldmethode,%20Berechnung%20des%20planckschen%20Wirkungsquantums,%20Licht%20als%20Teilchen.%20Stelle%20mir%20die%20Fragen%20einzeln%20nacheinander.%20Bewerte%20meine%20Antwort%20im%20Anschluss%20auf%20einer%20Skala%20von%200%20bis%2010.%20Mein%20Niveau%20ist%20Grundkurs%20Klasse%2012%20Physik.%20Gib%20mir%20am%20Schluss%20der%205%20Fragen%20ein%20Gesamtfeedback%20auf%20meine%20Antworten.)

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


### Welle -> Teilchen , Teilchen -> Welle

> [LESCH-Quantenphysik-Teilchenwellen](https://youtu.be/cWf1OUVUObw?t=493)

## 7. 5. Elektroneninterferenz am Doppelspalt

> Ein Elektronenstrahl wird auf einen Doppelspalt (oder ein Gitter) gerichtet, dahinter befindet sich ein Schirm, der auftrefende Elektronen sichtbar macht. ([Anschauung](https://youtu.be/ZdO4ERBrgnw?t=225))

{{1}}
*******
[Erklärungsvideo](https://youtu.be/M8MuyfjtUFU?t=39), [Anschauungsvideo](https://youtu.be/3ohjOltaO6Y?t=127)
*******

{{2}}
*******
Im Jahr 1924 schlug der französche Physiker _Victor Louis de Broglie_ vor, jedem Teilchen eine Wellenlänge zuzuordnen, genannt __de Broglie Wellenlänge__

> Die **_de-Broglie_ Wellenlänge**
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

1. ![LB S.66 Aufgabe 4](https://diversewolken.ddns.net/nextcloud/index.php/s/i2afaYAZ3qGGHNa/download)

<p style="margin-left:10%">

a)

- [[ ]] Es treten keine Elektronen aus dem Metall aus 
- [[ ]] Es treten weniger Elektronen aus dem Metall aus 
- [[ ]] Es treten ungefähr genauso viele Elektronen aus dem Metall aus
- [[x]] Es treten mehr Elektronen aus dem Metall aus
- [[ ]] Die maximale kinetische Energie der Elektronen sinkt 
- [[x]] Die maximale kinetische Energie der Elektronen bleibt gleich
- [[ ]] Die maximale kinetische Energie der Elektronen steigt

b)

- [[ ]] Es treten keine Elektronen aus dem Metall aus 
- [[ ]] Es treten weniger Elektronen aus dem Metall aus 
- [[x]] Es treten ungefähr genauso viele Elektronen aus dem Metall aus
- [[ ]] Es treten mehr Elektronen aus dem Metall aus
- [[ ]] Die maximale kinetische Energie der Elektronen sinkt 
- [[ ]] Die maximale kinetische Energie der Elektronen bleibt gleich
- [[x]] Die maximale kinetische Energie der Elektronen steigt

</p>

---

2. ![LB S.67 Aaufgabe 13](https://diversewolken.ddns.net/nextcloud/index.php/s/dM8dxnfXqzx9Xro/download)

<p style="margin-left:10%">

a)

<p style='margin-left:10%'>

__In der Einheit Elektronenvolt:__

@rangeQuiz2($E_{kin}$,200000,eV)

__In der Einheit Joule:__

@rangeQuiz2($E_{kin}$,3.2e-14,J)

</p>

<details style='margin-left:10%'>

<summary> Lösungsweg </summary>

Die kinetische Energie, die das Proton erhält, kann mit der Formel $E_{kin}=U\cdot q$ ermittelt werden.

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

$E_{kin}= 200000\,\mathrm{V} \cdot e = 200000\,\mathrm{eV}$

$E_{kin}= 200000\,\mathrm{V} \cdot 1,602\cdot10^{-19}C = 3,2\cdot10^{-14}\,\mathrm{J}$

</details>

b)

<p style='margin-left:10%'>

__Endergebnis Wellenlänge:__

@rangeQuiz2($\lambda$,6.41e-14,m)

</p>

<details style='margin-left:10%'>

<summary> Lösungsweg </summary>

Für die kinetische Energie $E_{kin}=\frac{1}{2}\cdot m \cdot v^2$ ermittelt werden. Die de-Broglie Wellenlänge wird dann mit der Geschwindigkeit und der Protonenmasse ermittelt.

__Zwischenergebnis Elektronengeschwindigkeit:__

@rangeQuiz2($v$,6.19e6,$\mathrm{\frac{m}{s}}$)

</details>

<details style='margin-left:10%'>

<summary> Lösung </summary>

$ v = \sqrt{\frac{2\cdot E_{kin}}{m_p}} = 6.19 \cdot 10^{6}\mathrm{\frac{m}{s}}$

$\lambda = \frac{h}{m_p\cdot v} = 6,41 \cdot 10^{-13}\,\mathrm{m}$

</details>


</p>

---

3. [Bitte anklicken: Verständnisfragen-Elektronenbeugung-KI-Gestützt](http://10.102.1.3:3001/?q=Heute%20wurde%20die%20de%20Broglie%20Wellenl%C3%A4nge%20von%20Elektronen%20am%20Beispiel%20des%20Beugungsmusters%20von%20Elektronen%20an%20einem%20Doppelspalt%20erkl%C3%A4rt.%20Dabei%20sind%20sowohl%20einzelne%20Auftreffpunkte%20der%20Elektronen%20sichtbar,%20als%20auch%20ein%20Streifenmuster,%20wenn%20man%20eine%20h%C3%B6here%20Zahl%20an%20Elektronen%20beobachtet.%20Stelle%20mir%20drei%20Verst%C3%A4ndnisfragen%20zum%20Welle%20Teilchendualismus%20am%20Beispiel%20der%20Elektronenbeugung%20am%20Doppelspalt.%20Stelle%20mir%20die%20Fragen%20eine%20nach%20der%20anderen%20und%20warte%20auf%20meine%20Antwort.%20Bewerte%20meine%20Antworten%20jeweils%20auf%20einer%20Skala%20von%200%20bis%2010.%20Gib%20mir%20die%20M%C3%B6glichkeit%20meine%20Antwort%20zu%20verbessern%20oder%20zur%20n%C3%A4chsten%20Frage%20zu%20wechseln.%20Das%20Niveau%20ist%20dabei%20Grundkurs%20Physik.)

4. ![LB S. 67 Aufgabe 14](https://diversewolken.ddns.net/nextcloud/index.php/s/TdRPmigwdPg6y9j/download)


## 7. 6. Einzelphotoneninterferenz am Doppelspalt

{{1}}
****************
<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


Reduziert man bei einem Doppelspalt-Experiment die Lichtintensität, so lässt sich nachweisen, dass sich im Versuchsaufbau zu einem Zeitpunkt lediglich ein Photon befindet.

{{2}}
*************
<p style="color:blue">

Bestimmen Sie für einen Laser der Wellenlänge 650 nm die maximale Lichtleistung, damit sich in der Aperatur der Länge $ℓ=1\,\mathrm{m}$ lediglich 1 Photon befindet.

<details style='margin-left:10%'>

<summary> Lösungshinweis </summary>

Bestimmen Sie die Energie eines Photons. Ermitteln Sie Flugzeit eines Photons. Passen Sie nun die Lichtleistung so an, dass die Zeit, zwischen zwei ausgesandten Photonen größer ist als die Flugzeit.

</details>

</p>

*************

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/bgosKyRYWKax9zX/download)

</div>

</section>
****************

{{3}}
******************
__Lösung:__

> - Energie eines Photons
>
> $$ E_{ph} = \frac{h\cdot c}{\lambda} = 3,06 \cdot 10^{-19} \,\mathrm{J} $$
>
> - Flugzeit durch die Apperatur
>
> $$ t = \frac{ℓ}{c} = 3,33 \cdot 10^{-9}\,\mathrm{s} $$
>
> - Maimale Lichtleistung
>
> $$ P_{L} = \dfrac{E_{ph}}{t} = 9,18 \cdot 10^{-11} W$$

******************


{{4}}
******************
__Beobachtungen auf dem Schirm:__

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

Für dieses Experiment wird ein photographischer Schirm genutzt. Jedes auftreffende Photon hinterlässt einen hellen Fleck. Wird das Experiment mit wenigen Photonen durchgeführt (a), so ergibt sich eine scheinbar zufällige Verteilung der Photonen. 

> Der Ort des Auftreffens ist für das einzelne Photon @color(nicht vorhersagbar, red) (@color(nicht determiniert, red)).

Eine größere Anzahl von Photonen (b+c) hinterlässt auf dem Schirm ein Bild, welches einem Interferenzmuster (d) ähnelt

> Die @color(Zufallsverteilung, red) für eine große Anzahl an Photonen ist @color(vorherbestimmt, red) (@color(determiniert, red)).

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Einzelphotoneninterferenz](https://diversewolken.ddns.net/nextcloud/index.php/s/Hpjzn7WP4Eb9eWA/download)

</div>

</section>

******************


### Übungsaufgabe zu Elektronen als Quantenobjekte

> a) [KI-Aufgabe-Gemeinsamkeiten-Unterschiede-Elektronen-Photonen](http://10.102.1.3:3001/?q=Im%20Grundkurs%20Physik%20wurde%20das%20Interferenzbild%20einzelner%20Elektronen%20und%20einzelner%20Photonen%20besprochen.%20Stelle%20mir%20auf%20der%20Grundlage%20des%20Welle-Teilchen-Dualismus%20von%20Elektronen%20und%20Photonen%20f%C3%BCnf%20Verst%C3%A4ndnisfragen%20zu%20Gemeinsamkeiten%20und%20Unterschieden%20von%20Elektronen%20und%20Photonen.%20Stelle%20mir%20die%20Fragen%20eine%20nach%20der%20anderen%20und%20warte%20auf%20meine%20Antwort.%20Hilf%20mir%20durch%20die%20Fragen%20diese%20Unterschiede%20herauszuarbeiten.%20Gib%20mir%20zu%20jeder%20meiner%20Antworten%20Feedback.%20Gehe%20dabei%20Kleinschrittig%20vor.%20Vernachl%C3%A4ssige%20Effekte%20der%20relativistischen%20Geschwindigkeit.%20Achte%20darauf,%20dass%20das%20Niveau%20Gymnasium%20Grundkurs%20Klasse%2012%20nicht%20%C3%BCberschreitet.)


---

Nehmen Sie für die folgenden Aufgaben an, dass sich Elektronen mit einer Geschwindigkeit von $v = 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$ bewegen.

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

Die kinetische Energie $E_{kin} = \frac{1}{2} m_e v^2$, welche die Elektronen durch die Geschwindigkeit $v$ besitzen, muss gleich der elektrischen Energie $E_{el} = e \cdot U$ sein, die durch die Beschleunigungsspannung $U$ gewonnen wurde.

Nutze die Gleichung: $$E_{el} = E_{kin} \Rightarrow e \cdot U = \frac{1}{2} m_e v^2$$

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Zur Berechnung wird die Beziehung $U = \frac{m_e v^2}{2 \cdot e}$ verwendet.

Dabei wird die Geschwindigkeit $v = 8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1}$ (aus den vorherigen Teilaufgaben), die Elektronenmasse $m_e \approx 9,109 \cdot 10^{-31} \, \text{kg}$ und die Elementarladung $e \approx 1,602 \cdot 10^{-19} \, \text{C}$ eingesetzt.

$$U = \frac{9,109 \cdot 10^{-31} \, \text{kg} \cdot (8,1 \cdot 10^7 \, \text{m} \cdot \text{s}^{-1})^2}{2 \cdot 1,602 \cdot 10^{-19} \, \text{C}}$$

$$\mathbf{U \approx 18653 \, \text{V}}$$

</details>

---

> d) Die Elektronen werden nun durch ein Gitter mit der Gitterkonstanten $b = 10 \, \text{pm}$ geschickt. Ermitteln Sie den Abstand $s_k$ des ersten ($k=1$) und des zweiten ($k=2$) Maximums vom Maximum Nullter Ordnung. <br> Der Abstand des Schirms vom Gitter beträgt 6 cm.

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

---

> e) Mit Photonen soll an dem Aufbau ein identisches Interferenzmuster erzeugt werden. Geben Sie die Wellenlänge und die Energie der Photonen an. Ordnen Sie die Photonen einem Strahlungs-Bereich zu.

<p style='margin-left:10%'>

@rangeQuiz2( $\lambda_{ph}$, 8.98e-12, $\text{m}$)

@rangeQuiz2( $E_{ph}$, 2.21e-14, $\text{J}$)

<!-- data-solution-button="off" -->
[[ Terahertzstrahlung | Infrarotstrahlung | sichtbares Licht | ultraviolettes Licht | (Röntgenstrahlung) | (Gammastrahlung) ]]

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Wenn der Versuchsaufbau identisch ist, hängt die Ausprägung des Interferenzmusters nur von einer Eigenschaft der einfallenden Welle ab. Überprüfen Sie diese Eigenschaft bei den Elektronen.

Die Energie der Photonen ermittelt sich aus der Beziehung $E_ph = h \cdot f$.

Ermitteln Sie mit Hilfe des Spektrums elektromagnetischer Wellen der Bereich für die vorliegenenden Photonen.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

Die entscheidende Eigenschaft ist genau die Wellenlänge. Die Wellenlänge der Elektronen ist laut Aufgabe b) $8,98\cdot10^{-12}\,\mathrm{m}$. Somit muss die Wellenlänge der Photonen ebenfalls diesen Wert haben.

$E_ph = h \cdot f = \dfrac{h \cdot c}{\lambda} = 2,21 \cdot 10^{-14} J$.

$\approx9\cdot10^{-12} m$ fallen in den Bereich zwischen Röntgenstrahlung und Gammastrahlung.

</details>

## 7. 7. Das Unschärfeprinzip / die Heißenberg'sche Unschärferelation

> Bei einer __Messung__ von Ort ($x$) und Impuls $p=m\cdot v$ eines quantenmechanischen Teilchens, können beide Größen nicht __gleichzeitig__ mit einer beliebigen Genauigkeit $\Delta x$ bzw. $\Delta p$ ermittelt werden. Die maximale Beobachtungsgenauigkeit beträgt: $$ \boxed{\Delta x \cdot \Delta p \geq \dfrac{h}{4\pi}} $$ Hierbei ist $\Delta x$ die __Ortsunschärfe__ und $\Delta p$ die __Impulsunschärfe__.
>
>> _Umgangssprachlich: Je genauer ich den Ort eines Teilchens bestimme, desto größer wird die Unsicherheit in der Geschwindigkeitsbestimmung (Impulsbestimmung)_
>
> Dieselbe gleichzeitige Unbestimmtheit ergibt sich bei einer Messung von _Energie_ und _Zeit_ als $$ \boxed{\Delta E \cdot \Delta t \geq \dfrac{h}{4\pi}}$$ Hierbei ist $\Delta E$ die Energieunschärfe und $\Delta t$ die Zeitunschärfe.

### Übungen zur LK

Eine Photokathode (im Vakuum) besteht aus dem Material Calcium.

1. Ermitteln Sie die Auslösearbeit in der Einheit eV und in der Einheit J.

<p style='margin-left:10%'>

@rangeQuiz2($W_A$,2.87,$\mathrm{eV}$)

@rangeQuiz2($W_A$,4.6e-19,$\mathrm{J}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Schlagen Sie die Werte in der Formelsammlung nach. Ermitteln Sie die Auslösearbeit in der Einheit J mit der Umrechnung $1,6\cdot 10^{-19}$.

</details>

---

2. [KI-Aufgabe-Auslösearbeit](http://10.102.1.3:3001/?q=Das%20Niveau%20ist%20Grundkurs%20Physik,%20Klasse%2012.%20Stelle%20mir%20folgende%20Frage%20und%20bewerte%20meine%20Antwort%20auf%20einer%20Skala%20von%200%20bis%2010.%20Hilf%20mir%20meine%20Antwort%20zu%20verbessern,%20wenn%20ich%20das%20m%C3%B6chte.%20Die%20Frage%20lautet:%20Erl%C3%A4utere%20die%20Bedeutung%20der%20Ausl%C3%B6searbeit%20beim%20Photoeffekt.%20Stelle%20mir%20nur%20die%20Frage,%20gib%20mir%20zu%20Anfang%20noch%20keine%20Hinweise.)

---

3. [KI-Aufgabe-Oranges-Licht](http://10.102.1.3:3001/?q=Das%20Niveau%20ist%20Grundkurs%20Physik,%20Klasse%2012.%20Stelle%20mir%20folgende%20Frage%20und%20bewerte%20meine%20Antwort%20auf%20einer%20Skala%20von%200%20bis%2010.%20Hilf%20mir%20meine%20Antwort%20zu%20verbessern,%20wenn%20ich%20das%20m%C3%B6chte.%20Die%20Frage%20lautet:%20Eine%20Photokathode%20besteht%20aus%20Calcium,%20es%20hat%20eine%20Ausl%C3%B6searbeit%20von%202,87eV.%20Entscheiden%20Sie,%20ob%20oranges%20Licht%20Elektronen%20aus%20dem%20Metall%20herausl%C3%B6sen%20kann%20oder%20nicht.%20Begr%C3%BCnden%20Sie%20Ihre%20Antwort.%20Stelle%20mir%20zun%C3%A4chst%20nur%20diese%20Frage,%20gib%20mir%20noch%20keine%20Tipps%20oder%20hilfen.%20Hinweise:%20Die%20Ausl%C3%B6searbeit%20wird%20mit%20W_A%20bezeichnet.)

---

4. Die Photokathode wird nun mit ultraviolettem Licht bestrahlt, die Wellenlänge des Lichts beträgt 350 nm. Ermitteln Sie die maximale kinetische Energie der austretenden Elektronen. Ermitteln Sie auch die Geschwindigkeit dieser Elektronen

<p style='margin-left:10%'>

@rangeQuiz2($E_{kin_max}$, 1.08e-19 ,$\mathrm{J}$)

@rangeQuiz2($v_{max}$, 4.87e5 ,$\mathrm{\frac{m}{s}}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Nutzen Sie Energiebilanz beim Photoeffekt um die maximale kinetische Energie der Elektronen zu ermitteln.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis 2 </summary>

Die Energiebilanz lautet:

$$ E_{ph} = h \cdot f = E_{kin, max} + W_A $$

Wenn Sie $E_{kin, max}$ ermittelt haben, können Sie die Formel für die kinetische Energie nutzen, um die Geschwindigkeit zu ermitteln.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis 3 </summary>

Die kinetische Energieformel lautet $E_{kin} = \frac{1}{2} \cdot m \cdot v^2$.

</details>

---

5. Zeichnen Sie die Einstein'sche Gerade für das Material Calcium in ein Diagramm $E_{kin-max}(f)$. Verwenden Sie auf der y-Achse für die kinetische Energie die Einheit eV und auf der x-Achse für die Frequenz die Einheit $10^{14}\,\mathrm{Hz}$.

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Um die Einstein'sche Gerade zu zeichnen benötigen Sie zwei Datenpunkte. Beide haben Sie bereits in den Aufgaben 1. und 4. ermittelt.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis 2 </summary>

Die Auslösearbeit ist der (negative) Schnittpunkt der Geraden mit der y-Achse. Der zweite Punkt ist die Elektronenenergie bei einer Wellenlänge von 350 nm (siehe Aufgabe 4). Rechnen Sie noch die Wellenlänge in Frequenz um und verbinden Sie die Punkte.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

Die Auslösearbeit ist der (negative) Schnittpunkt der Geraden mit der y-Achse. Der zweite Punkt ist die Elektronenenergie bei einer Wellenlänge von 350 nm (siehe Aufgabe 4). Rechnen Sie noch die Wellenlänge in Frequenz um und verbinden Sie die Punkte.

</details>

---

6. [KI-Aufgabe-deBroglieWellenlänge](http://10.102.1.3:3001/?q=Das%20Niveau%20ist%20Grundkurs%20Physik,%20Klasse%2012.%20Stelle%20mir%20folgende%20Frage%20und%20bewerte%20meine%20Antwort%20auf%20einer%20Skala%20von%200%20bis%2010.%20Hilf%20mir%20meine%20Antwort%20zu%20verbessern,%20wenn%20ich%20das%20m%C3%B6chte.%20Die%20Frage%20lautet:Erl%C3%A4utere%20die%20Bedeutung%20der%20de-Broglie%20Wellenl%C3%A4nge%20f%C3%BCr%20massebehaftete%20Teilchen%20wie%20Elektronen%20oder%20Protonen.%20Stelle%20mir%20zun%C3%A4chst%20nur%20diese%20Frage,%20gib%20mir%20noch%20keine%20Tipps%20oder%20hilfen.%20Hinweise:%20Wir%20betrachten%20ausschlie%C3%9Flich%20nichtrelativistische%20Teilchen.%20Bewerte%20sanft.)

---

7. Ermitteln Sie nun die de-Broglie Wellenlänge der schnellsten Elektronen, welche die Calcium-Kathode (Aufgabe 4) unter einer Betrahlung mit einer Wellenlänge von 350 nm verlassen.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda$, 1.494e-9 ,$\mathrm{m}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Die maximale Geschwindigkeit der Elektronen ergibt sich aus Aufgabe 4 zu $4,87\cdot10^{5}\mathrm{\frac{m}{s}}$. Ermitteln Sie nun mit Hilfe der de-Broglie Gleichung die Wellenlänge.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$$ \lambda = \frac{h}{m\cdot v} = 1,494 \cdot 10^{-9}\,\mathrm{m} $$

</details>

---

8. Die Elektronen aus Aufgabe 7 werden nun auf ein Gitter mit der Gitterkonstanten $b=5 \cdot 10^{-9}\,\mathrm{m}$ geleitet. Ermitteln Sie, unter welchem Ablenkwinkel ein Detektor das erste Maximum einfallender Elektronen bestimmen würde.

<p style='margin-left:10%'>

@rangeQuiz2($\alpha_1$,17.386,°)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Die Welleneigenschaft der Elektronen führt zu Beugung und Interferenz am Gitter. Nutzen Sie die Formeln für das Gitter, um den Ablenkwinkel des ersten Maximums zu ermitteln.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis 2 </summary>

Die Formel lautet $\sin\alpha_k=\frac{k \cdot \lambda}{b}$. Es gilt k=1.

</details>


### Aufgaben SchulLV Abitur 2021-2023

[AufgabenUndLösungen](https://diversewolken.ddns.net/nextcloud/index.php/s/NpYHBJLZrqPS42b)

### Materialgestützte Aufgabe (IQB)

[IQB-Aufgabe-Quantenobjekte](https://www.iqb.hu-berlin.de/media/exercise_files/Beispielaufgaben_-_Physik/TeilcheninterferenzgA_Aufgabe.pdf)


# LB 8 - Atomvorstellungen

![Atomvorstellungen](https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp)

## 8. 1. Die Geschichte der Atommodelle


{{0-1}}
************
| Atom-Modell | Beschreibungen |
| :---- | :---------- |
| Dalton'sches Atommodell |  |
| Thomson'sches Atommodell | |
| Rutherford'sches Atommodell |  |
| Bohr'sches Atommodell |  |
************

{{1-2}}
************
!?[EinfühungAtomvorstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/zXFSJYE9tddoNTf/download)
************

{{2}}
************
| Atom-Modell | Beschreibungen |
| :----------- | :---------- |
| Dalton'sches Atommodell | Atome sind unveränderbare Kugeln. Chemische Bindungen sind Neuanordnungen der Kugeln |
| Thomson'sches Atommodell <br> Rosinenmodell | Negativ geladene Elektronen sind von positiv geladener Materie umgeben |
| Rutherford'sches Atommodell | _Miniatur-Sonnensystem_ ; beinahe die gesamte Masse ist im Kern konzentriert <br> die Elektronen bewegen sich auf Kreisbahnen um den Kern |
| Bohr'sches Atommodell | fest gelegte Bahnen für die Elektronen (nur diese sind erlaubt) <br> jeder Bahn ist ein Energieniveau zugeordnet <br> bei Energiezufuhr kann ein Elektron auf einer weiter außen liegende Bahn springen <br> gibt das Elektron die Energie wieder ab, so wird diese als Strahlung emittiert <br> nur die äußeren Elektronen der nicht vollständig besetzten Bahnen tragen zur chemischen Bindung bei|
************

## 8. 2. Das Bohr'sche Atommodell

![TB_1](https://diversewolken.ddns.net/nextcloud/index.php/s/apsmjmxb3B2abe7/download)

---

![TB_2](https://diversewolken.ddns.net/nextcloud/index.php/s/apsmjmxb3B2abe7/download)

### Aufgaben zu den Atmomodellen (Multiple-Choice)

❓ Frage 1: Grundannahme des bohr’schen Atommodells

Welche zentrale Annahme macht das bohr’sche Atommodell über die Elektronenbewegung?

- [[ ]] Elektronen bewegen sich frei im Atomkern
- [[X]] Elektronen bewegen sich auf festen, quantisierten Kreisbahnen
- [[ ]] Elektronen verlieren kontinuierlich Energie beim Umlauf
- [[ ]] Elektronen befinden sich in einer Elektronenwolke ohne feste Bahnen
- [[ ]] Elektronen können jede beliebige Bahnenergie annehmen

---

❓ Frage 2: Energieniveaus im bohr’schen Atommodell

Warum geben Atome nach dem bohr’schen Modell nur bestimmte Spektrallinien ab?

- [[ ]] Weil Elektronen ihre Masse verändern
- [[ ]] Weil Protonen Energie abstrahlen
- [[X]] Weil Elektronen nur zwischen diskreten Energieniveaus wechseln können
- [[ ]] Weil die Umlaufgeschwindigkeit der Elektronen konstant ist
- [[ ]] Weil der Atomkern instabil ist

---

❓ Frage 3: Gültigkeitsbereich des bohr’schen Atommodells

Für welche Atome liefert das bohr’sche Atommodell gute Ergebnisse?

- [[X]] Für wasserstoffähnliche Atome mit nur einem Elektron
- [[ ]] Für alle Atome unabhängig von ihrer Größe
- [[ ]] Nur für schwere Atome wie Uran
- [[ ]] Ausschließlich für Moleküle
- [[ ]] Für Festkörper und Metalle

❓ Frage 4: Energieabgabe im bohr’schen Atommodell

Wann wird nach dem bohr’schen Atommodell Strahlung emittiert?

- [[ ]] Wenn sich ein Elektron auf einer stabilen Bahn bewegt
- [[ ]] Wenn ein Elektron den Atomkern berührt
- [[X]] Wenn ein Elektron von einem höheren auf ein niedrigeres Energieniveau wechselt
- [[ ]] Wenn ein Elektron seine Umlaufgeschwindigkeit erhöht
- [[ ]] Wenn sich zwei Elektronen abstoßen

❓ Frage 5: Kritik am bohr’schen Atommodell

Welche der folgenden Aussagen beschreibt eine bekannte Schwäche des bohr’schen Atommodells?

- [[ ]] Es erklärt das Wasserstoffspektrum korrekt
- [[ ]] Es führt quantisierte Energieniveaus ein
- [[X]] Es kann die Spektren von Mehrelektronenatomen nicht korrekt erklären
- [[ ]] Es berücksichtigt den Atomkern
- [[ ]] Es erklärt die Stabilität von Elektronenbahnen

### Aufgaben zum Wasserstoffatom (Berechnungen)

1. Zeichnen Sie ein Energieniveau-Schema des Wasserstoffatoms mit dem Grundzustand und den ersten 5 angeregten Zuständen. Notieren Sie an jedem Niveau die Bindungsenergie. Kennzeichnen Sie den Übergang n=3 -> n=2.

---

2. Die Emissionen, die im sichtbaren Bereich liegen sind beim Wasserstoff Übergänge auf die zweite Schale. Ermitteln Sie die Energie und die Wellenlänge der Übergänge von n=3 -> n=2. Notieren Sie die Farbe des emittierten Lichts.

<p style='margin-left:10%'>

@rangeQuiz2($E_{3->2}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{3->2}$,655e-9,$\mathrm{m}$)

<!-- data-solution-button="off" -->
[[ infrarot | rot | gelb | grün | blau | violett | ultraviolett ]]

</p>

---

3. Geben Sie für ein Wasserstoffatom die Ionisierungsenergie an. <br> _Hinweis: Die Ionisierungsenergie ist die Energie, die aufgewendet werden muss, damit das Elektron des Wasserstoffs nicht mehr gebunden ist._

<p style='margin-left:10%'>

@rangeQuiz2($E_{ion}$,13.6,$\mathrm{eV}$)

</p>


## 8. 3. Das Wasserstoffatom

![TB_1](https://diversewolken.ddns.net/nextcloud/index.php/s/7DwNPsGoEy62fNL/download)

{{1}}
************
__Zusammenfassung bis hierher:__
************

{{2}}
************
> - an einen Atomkern gebundene Elektronen können nur bestimmte (d.h. diskrete) Energieniveaus besetzen -> @color(Orbitale im quantenmechanischen Atommodell, red)
************

{{3}}
************
> - wechselt ein Elektron ein Energiniveau, so ist das mit einem __quantenhaften__ Energieaustausch mit der Umgebung verbunden -> @color(Emission und Absorption von Photonen, red)
************

## 8. 4. Orbitale des quantenmechanischen Atommodells

{{1}}
**********
__Aufenthaltswahrscheinlichkeit statt feste Kreisbahn:__

> Das quantenmechanische Atommodell beschreibt den Aufenthaltsort der Elektronen nicht als Kreisbahn (wie im bohrschen Atommodell), sondern als eine @color(Wahrscheinlichkeitsverteilung, red) im Raum um den Atomkern. -> [Video 1](https://youtu.be/behQ3O97DXw?t=446)
**********

{{2}}
**********
__Bemerkungen:__

- bei einer Messung ist der Ort des Elektrons __nicht vorhersagbar (nicht determiniert)__

- die Bohrsche Kreisbahn ist bei einem Wasserstoffatom der __wahrscheinlichste Abstand vom Kern__
**********


{{3}}
**********
> Die räumliche Wahrscheinlichkeitsverteilung nennt man @color(Orbital, red). Je nach Quantenzahl haben diese Orbitale unterschiedliche Formen. <br> [Simulation](https://www.leifiphysik.de/atomphysik/quantenmech-atommodell/versuche/wellenfunktionen-orbitale-des-wasserstoffatoms-simulation-von-paul-falstadt) & [Video 2](https://www.youtube.com/watch?v=2e31oqxlkJg)
**********

{{4}}
**********
__Bemerkungen:__

- das einfachste Orbital (K-Schale) ist kugelförmig

- je größer die Hauptquantenzahl n (K->L->M), desto weiter weg ist der wahrscheinlichste Aufenthaltsort des Elektrons

- [Orbitale](https://commons.wikimedia.org/wiki/Hydrogen_orbitals_3D_real) können z.B. kugelförmig, hantelförmig oder dounutförmig sein
**********

{{5}}
**********
<p style="margin-left:10%">
![Ausschnitt-Atomorbitale](https://diversewolken.ddns.net/nextcloud/s/2fDBpE4c7sQx6Et/download "n-Hauptquantenzahl, m-Nebenquantenzahl ")
</p>
**********


## 8. 5. Quantenhafte Absorption und Emission von Energie

> Wenn Elektronen das Energieniveau wechseln, kann Energie aufgenommen oder abgegeben werden.
>
> @color(__Der Energiebetrag entspricht dabei der Differenz der Energieniveaus.__, red)

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Absorption von Energie__

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Emission eines Photons__

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

---

Elektron wird auf eine höhere Bahn gehoben. Es muss Energie hinzugefügt werden.

---

![Absorption](https://diversewolken.ddns.net/nextcloud/s/BQ2Z5Apxa9TyqR4/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

---

Elektron springt auf eine niedrigere Bahn. Es wird Energie in Form eines Photons abgegen.

---

![Emission](https://diversewolken.ddns.net/nextcloud/s/wRYRWkGLbYcMqqA/download)

</div>

</section>

### Übungsaufgaben zu Orbitalen und Energieaustausch

<details>

<summary> 1. __Aussagen zu Atomorbitalen__ </summary>

1. 1. Welche Aussage beschreibt ein **Orbital** im quantenmechanischen Atommodell am besten?

<p style="margin-left:10%">

- [( )] Ein Orbital ist die feste Kreisbahn, auf der das Elektron um den Kern fliegt.
- [(X)] Ein Orbital ist ein Raumbereich, in dem sich ein Elektron mit hoher Wahrscheinlichkeit aufhält.
- [( )] Ein Orbital ist der Ort, an dem das Elektron immer exakt gefunden wird.
- [( )] Ein Orbital ist eine messbare Bahnkurve, die man mit einem Mikroskop sehen kann.
- [( )] Ein Orbital ist nur eine Zeichnung ohne physikalische Bedeutung.
- [( )] Ein Orbital ist identisch mit der Schale (z.B. „2. Schale“), mehr gibt es da nicht.

</p>

---

1. 2. Was bedeutet „Aufenthaltswahrscheinlichkeit“ bei Elektronen?

<p style="margin-left:10%">

- [( )] Sie sagt, wie schnell das Elektron unterwegs ist.
- [( )] Sie sagt, wie warm das Elektron ist.
- [(X)] Sie gibt an, wie wahrscheinlich es ist, ein Elektron in einem bestimmten Raumbereich zu finden.
- [( )] Sie gibt an, wie wahrscheinlich es ist, dass der Atomkern verschwindet.
- [( )] Sie ist die Wahrscheinlichkeit, dass das Elektron auf einer festen Bahn bleibt.
- [( )] Sie ist eine Zufallszahl ohne Bezug zu Messungen.

</p>

---

1. 3. Warum zeichnet man im quantenmechanischen Atommodell **keine festen Elektronenbahnen** wie im Bohr-Modell?

<p style="margin-left:10%">

- [( )] Weil Elektronen zu klein sind, um Bahnen zu haben.
- [(X)] Weil Ort und Impuls nicht gleichzeitig beliebig genau bestimmbar sind (Unschärferelation).
- [( )] Weil der Atomkern das Elektron „nicht reinlässt“.
- [( )] Weil Elektronen immer im Kreis fliegen.
- [( )] Weil die Elektronen ständig zwischen den Bahnen hin und her sprichen.

</p>

---

1. 4. Je größer die Hauptquantenzahl n, ..

<p style="margin-left:10%">

- [( )] desto geringer ist die Ausdehnung des Atomkerns.
- [( )] desto größer ist die Ausdehnung des Atomkerns.
- [( )] desto näher am Kern ist der wahrscheinlichste Fundort (bei einer Messung) des Elektrons.
- [(X)] desto weiter vom Kern entfernt ist der wahrscheinlichste Fundort (bei einer Messung) des Elektrons.

</p>

</details>


---

<details>

<summary> __2. Aussagen zu Absorption und Emission von Energie bei einem Atom__ </summary>

2. 1. Absorption: Wann passiert sie? <br> Wann wird bei einem Elektronenübergang **Energie absorbiert**?

<p style='margin-left:10%'>

- [( )] Wenn ein Elektron von einem höheren auf ein niedrigeres Energieniveau wechselt.
- [(X)] Wenn ein Elektron von einem niedrigeren auf ein höheres Energieniveau wechselt.
- [( )] Wenn ein Elektron im gleichen Energieniveau bleibt.
- [( )] Wenn ein Elektron den Atomkern berührt.
- [( )] Immer, egal in welche Richtung der Übergang geht.
- [( )] Nur wenn das Elektron vorher schon leuchtet.

</p>

---

2. 2. Emission: Was wird frei? Was passiert bei einem Übergang von einem **höheren** auf ein **niedrigeres** Energieniveau?


<p style='margin-left:10%'>

- [( )] Das Atom absorbiert ein Photon.
- [(X)] Das Atom emittiert Energie, oft als Photon (Licht).
- [( )] Das Elektron gewinnt Energie und springt nach außen.
- [( )] Es passiert nichts: Energieniveaus sind nur Theorie.
- [( )] Die Protonenzahl ändert sich.
- [( )] Das Elektron wird zu einem Proton (ist doch alles elektrisch).

</p>

---


2. 3. Zusammenhang Energie – Lichtfarbe <br> Welche Aussage ist richtig?



<p style='margin-left:10%'>

- [( )] Je größer die Energiedifferenz ΔE, desto kleiner die Photonenenergie.
- [( )] Die Farbe hängt nur von der Anzahl der Elektronen ab.
- [( )] Alle Übergänge haben die gleiche Photonenergie, so lange die Änderung der Quantenzahl gleich ist (z.B. $\Delta n=1$)
- [( )] Ein Photon kann nur bei Absorption entstehen, nicht bei Emission.
- [(X)] Je größer die Energiedifferenz ΔE, desto energiereicher (z.B. „blauer“) ist das emittierte/absorbierte Photon.
- [( )] Die Photonenenergie ist unabhängig vom Übergang.

</p>

</details>

---

<details>

<summary> __3. Berechnungen zur Emission und Absorption von Energie__ </summary>

3. 1. Die Emissionen, die beim Wasserstoffatom im sichtbaren Bereich liegen, sind Übergänge auf die zweite Schale. Ermitteln Sie die Energie und die Wellenlänge der Übergänge von n=3 -> n=2. Notieren Sie die Farbe des emittierten Lichts.

<p style='margin-left:10%'>

@rangeQuiz2($E_{3->2}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{3->2}$,655e-9,$\mathrm{m}$)

<!-- data-solution-button="off" -->
[[ infrarot | rot | gelb | grün | blau | violett | ultraviolett ]]

</p>

---

3. 2. Ein Photon der Wellenlänge 102,64 nm wird von einem Wasserstoffatom absorbiert. Ermitteln Sie, welche Bahnen des Wasserstoff-Atoms an diesem Übergang beteiligt sind.

<p style='margin-left:10%'>

von n= [[ 1 ]] auf n=[[ 3 ]]

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Ermitteln Sie die Photonenergie in der Einheit eV. Nutzen Sie die Formel für die Energieniveaus am Wasserstoffatom und überprüfen Sie, welchem Übergang die Photonenenergie entspricht.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Das Elektron springt auf die dritte Bahn.

</details>


</details>

---