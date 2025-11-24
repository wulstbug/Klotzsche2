<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://examio-mediafiles.s3.eu-west-1.amazonaws.com/schwingung-sinus-print.jpg

mode: presentation

import: https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/settings.md

@style
.lia-slide__footer {
      display: none !important;
}
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

-->


# LB VI - Schwingungen und Wellen
<!-- 
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg
-->

![WhyPhysics](https://cdn.sanity.io/images/i2z87pbo/production/986d42d83b06e224216a5129cdcfd179bf4ce59c-1440x1079.jpg)

@uhr


## (optional) Definition eines periodischen Vorgangs

!?[Motivationsvideo](https://diversewolken.ddns.net/nextcloud/index.php/f/719652/downlaod)

## 1. Beschreibung einer mechanischen Schwingung

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

## 2. Der Federschwinger

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


## 3. Definition mechanische Schwingung

### Experimentierauftrag zu Federschwingern

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

### Übung: Aussagen zum Federschwinger

@color(Entscheiden Sie für folgende Aussagen. Nutzen Sie im Zweifel die Simulation., blue)

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


## 5. Grundlagen Elektromagnetischer Schwingkreis

__Energiebetrachtung:__

> In einem idealen Schwingkreis schwingt die Energie zwischen dem [[ elektrischen ]] Feld des Kondensators ([[ elektrische ]] Energie) und dem magnetischen Feld der Spule ([[ magnetische ]] Energie) hin und her. Die Summe aus elektrischer und magnetischer Energie ist zu jedem Zeitpunkt [[ konstant ]].

<p style="color:blue">

Erstellen Sie mit Hilfe der Simulation einen Schwingkreis, den Sie eine Batterie aufladen können.

-> [PHeT-Simulation-AC-Circut](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac-virtual-lab/latest/circuit-construction-kit-ac-virtual-lab_all.html?locale=de)

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

### 5. 1. Eigenschaften idealer und realer Schwingkreise

-> [PHeT-Simulation-AC-Circut](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac-virtual-lab/latest/circuit-construction-kit-ac-virtual-lab_all.html?locale=de)

<p style="color:blue;margin-left:10%">

Nutzen Sie für die folgende Aufgabe die Simulation:

1. Erstellen Sie einen idealen Schwingkreis. Der Kondensator soll zunächst mit 10V aufgeladen werden. Ergänzen Sie dazu zwei Schalter und eine Batterie (anklicken -> $10V$).

---

2. Ändern Sie die Induktivität der Spule zu $2\,\mathrm{H}$ und die Kapazität des Kondensators zu $0,2\,\mathrm{F}$. Berechnen Sie die Frequenz der Schwingung.

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

2. 5. Ermitteln Sie die maximale Auslenkung des Systems. Nutzen Sie dazu die Zusammenhänge für $y_{max}$ aus $v_{max}$ aus _1. Beschreibung einer mechanischen Schwingung_.

<p style="margin-left:10%">

@rangeQuiz2($y_{max}$, 0.0095 ,$m$)

</p>

<details style="margin-left:10%">

<summary> Hinweise zur Lösung </summary>

In der Aufgabe aus _1. Beschreibung einer mechanischen Schwingung_
 wurde gezeigt, dass

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


## 6. (Teil I) Mechanische Wellen

### 6. 1. Arten mechanischer Wellen

<p style="color:blue">

__Beobachtung:__

1. Betrachten Sie die laufende Welle. Wechseln Sie zwischen Transversalwelle und Logitudinalwelle und beobachten Sie die Schwingung der Teilchen.

2. Ändern Sie die Amplitude und beobachten Sie die Welle. 

3. Verschieben Sie den Schieberegler ganz nach rechts und betrachten Sie die eingefrorene Welle.

<iframe src="https://www.geogebra.org/classic/cdyxv6pt?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

</p>

### 6. 2. Eigenschaften mechanischer Wellen

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


<p class="newspaper">


Kreisförmige Wellenfront (z.B. Steinwurf ins Wasser)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+4+668+0.00390625%0As+2+257+265+0+0.233333+0+10+100+1+0%0A)


<p class="cb">


Ebene Welle (z.B. Lichtausbreitung)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+0+569+0.048828125%0AS+2+0+1+511+1+0+0.466666+0+10+100+1+0%0A)

</p>

</p>

### 6. 4. Huygens'sche Prinzip

-> [Simulation-Ausbreitung-Kreiswelle-EbeneWelle](https://www.leifiphysik.de/mechanik/mechanische-wellen/ausblick/huygenssches-prinzip-zur-beschreibung-von-mechanischen-wellen)

### 6. 5. Reflexion

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



### 6. 6. Brechung


??[Fendt-Reflexion](https://www.walter-fendt.de/html5/phde/refractionhuygens_de.htm)

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


### 6. 7. Beugung

<p class="newspaper3">


![Welle-Beugung](https://diversewolken.ddns.net/nextcloud/index.php/s/M9eEFxFCjRATLt2/download)


<p class="cb">

__Kante:__

??[Simulation-Kante](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+489+1.5625e-8%0Aw+0+252+131+507+131%0AS+2+0+1+511+1+0+1.399998+0+10+100+1+0%0A)


<p class="cb">


__Spalt:__

??[Simulation-Spalt](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+578+1.5625e-8%0AS+2+0+1+511+1+0+2.2166635+0+10+100+1+0%0A203+0+-57+145+577+145+1+20+10%0A)


</p>

</p>

</p>

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




#### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)


### 6. 8. Interferenz


### 6. 9. Stehende Wellen

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

### 6. 11. Bestimmung der Wellenlänge des Lichts am Doppelspalt

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

![Gitter8](https://diversewolken.ddns.net/nextcloud/index.php/s/4igXLgZHtQ6nN6e/download)<!-- style="width:100%" -->

</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">



1. Es gelten die Formeln wie beim Doppelspalt

$$ \boxed{ \sin(\alpha) = \dfrac{\purple{k\cdot\lambda}}{\blue{b}}  } \hspace{.5cm} \boxed{\tan(\alpha) = \blue{\dfrac{a}{e}}}$$

2. Eigenschaften des Interferenzbildes am Gitter

<p style="margin-left:5%">

- Maxima sind schärfer abgegrenzt als beim Doppelspalt

- zwischen den Maxima ist die Lichtintensität sehr gering (Auslöschung)

</p>

3. __Kleinwinkelnäherung__ <br> <br> Wenn der Beobachtungswinkel $\alpha \leq 5^\circ$  beträgt, dann gilt in guter Näherung $$ sin(\alpha) = \tan(\alpha)$$ und die Formeln (1.) vereinfachen sich zu $$ \boxed{\dfrac{\purple{k\cdot\lambda}}{\blue{b}} = \blue{\dfrac{a}{e}}} $$ wobei das Maximum $\purple{k}$-ter Ordnung betrachtet wird.


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


1. 3. Berechnen Sie anschließend die Gitterkonstante und die Breite eines solchen Spektrums.

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