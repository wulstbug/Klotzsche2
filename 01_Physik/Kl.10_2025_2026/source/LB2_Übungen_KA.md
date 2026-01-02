<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://snu.edu.in/site/assets/files/18322/nanotechnology-molecule-atom-model-image-mixed-media_2.1600x0.webp

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


# Übungen zur KA

# Grundlagen zu Schwingungen

1. Eine Feder wird von einer Kraft $F$ von $100\mathrm{N}$ um $5\mathrm{cm}$ zusammengedrückt. Ermitteln Sie die Federkonstante $D$.

<p style='margin-left:10%'>

@rangeQuiz2( $D$ , 2000, $\mathrm{\frac{N}{m}}$ )

</p>


<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Um die Federkonstante $D$ zu bestimmen, nutzt man das Hooke’sche Gesetz $F = D \cdot s$. Setzen Sie die Werte ein und stellen Sie nach $D$ um. Achten Sie darauf, die Auslenkung $s$ von Zentimetern in Meter umzurechnen ($10 \, \text{cm} = 0,1 \, \text{m}$). 

</details>


<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

__Gegeben:__ $F = 100 \, \text{N}$, $s = 0,05 \, \text{m}$

__Gesucht:__ $D$

__Lösung:__

$$D = \frac{F}{s}$$
$$D = \frac{100 \, \text{N}}{0,05 \, \text{m}} = \mathbf{2000 \, \frac{N}{m}}$$ 

</details>

---

2. An die Feder der vorherigen Aufgabe wird nun eine Masse von 10 kg angehängt. Ermitteln Sie die Frequenz der Schwingung.

<p style='margin-left:10%'>

@rangeQuiz2( $f$ , 2.25, $\mathrm{Hz}$ )

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Die Frequenz $f$ einer harmonischen Schwingung an einer Feder wird durch die Federkonstante $D$ und die schwingende Masse $m$ bestimmt. Die Grundlage bildet die Formel für die Eigenfrequenz eines Federpendels:

$f = \frac{1}{2\pi} \cdot \sqrt{\frac{D}{m}}$

Setzen Sie die gegebenen Werte ($D = 2000 \, \frac{\text{N}}{\text{m}}$ und $m = 10 \, \text{kg}$) in die Gleichung ein.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Gegeben: $D = 2000 \, \frac{\text{N}}{\text{m}}$, $m = 10 \, \text{kg}$

Die Berechnung erfolgt in folgenden Schritten:

1. Einsetzen der Werte:

$f = \frac{1}{2\pi} \cdot \sqrt{\frac{2000 \, \frac{\text{N}}{\text{m}}}{10 \, \text{kg}}}$

2. Berechnung

$f \approx \frac{14,142}{6,283} \, \text{Hz}$
$\mathbf{f \approx 2,25 \, Hz}$

Die Frequenz der Schwingung beträgt etwa **$2,25 \, \text{Hz}$**.

</details>

---

3. Die Feder soll nun von außen angeregt werden. Beschreiben Sie, unter welcher Bedingung sich eine sehr große Amplitude des angeregten Schwingers einstellt. Benennen Sie dieses Phänomen. Beschreiben Sie, wie man eine zu starke Auslenung des Schwingers vermeiden kann.

<p style='margin-left:10%'>

[[ Resonanz ]]

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Überprüfen Sie, unter welcher Bedingung das Phänomen der Resonanz auftritt.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Resonanz tritt auf, wenn äußere Anregungsfrequenz und Eigenfrequenz des Schwingers ungefähr übereinstimmen. Um die starke Überhöhung der Amplitude zu vermeiden, muss sich die Anregungsfrequenz stark von der Eigenfrequenz des Schwingers unterscheiden. Sie muss entweder deutlich größer oder deutlich kleiner sein.

</details>

# Grundlagenaufgaben zu mechanischen Wellen

__Mechanische Wellen an einem Seil:__ Eine Wellenmaschine erzeugt an einem sehr langen, gespannten Seil eine harmonische Querwelle. Die Welle breitet sich mit einer Ausbreitungsgeschwindigkeit von c=12,0m/s aus. Der Abstand zwischen zwei aufeinanderfolgenden Wellenbergen (die Wellenlänge) beträgt λ=3,0m.

a) Berechnen Sie die Frequenz f der Schwingung, mit der die Wellenmaschine das Seil anregt.

<p style='margin-left:10%'>

@rangeQuiz2( f , 4.0, $\mathrm{Hz}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungweg </summary>

Zwischen der Ausbreitungsgeschwindigkeit c, der Wellenlänge λ und der Frequenz f besteht der grundlegende Zusammenhang der Wellenausbreitungsgleichung. Recherchiere diesen in deinem Hefter.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

![Uebung_Wellen_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/JH7YfGMxtE7dYP8/download)

</details>

---

b) Ermitteln Sie die Periodendauer T dieser mechanischen Welle.

<p style='margin-left:10%'>

@rangeQuiz2( T , 0.25, $\mathrm{s}$ )

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungweg </summary>

Die Periodendauer T gibt an, wie lange ein einzelner Oszillator für eine vollständige Schwingung benötigt. Sie ist der Kehrwert der Frequenz $f: T=\frac{1}{f}$
​
 
Verwenden Sie den in Teilaufgabe a) berechneten Wert für f.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

![Uebung_Wellen_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/mF29QznosbDKqrW/download)

</details>


# Sachaufgabe zu Schwingungen an einem PKW

![Fahrzeugfeder](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Double_wishbone_suspension.jpg/960px-Double_wishbone_suspension.jpg)<!-- style="max-width:200px"--> Eine Stahlfeder am Vorderrad eines PKWs wird durch eine Masse von $400 \, \text{kg}$ um $10 \, \text{cm}$ zusammengedrückt und dann losgelassen. Die Feder beginnt nach Anregung mit der Eigenfrequenz zu schwingen. 

---

a) Ermittle die Federkonstante dieser Stahlfeder. 

@rangeQuiz2( $D$ , 40000.0, $\mathrm{\frac{N}{m}}$ )

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Um die Federkonstante $D$ zu bestimmen, nutzt man das Hooke’sche Gesetz $F = D \cdot s$. Die wirkende Kraft $F$ ist hier die Gewichtskraft $F_G = m \cdot g$ der Masse, die die Feder zusammendrückt. Setzen Sie die Werte ein und stellen Sie nach $D$ um. Achten Sie darauf, die Auslenkung $s$ von Zentimetern in Meter umzurechnen ($10 \, \text{cm} = 0,1 \, \text{m}$). Für den Nachweis wird mit der Erdbeschleunigung $g \approx 10 \, \frac{\text{m}}{\text{s}^2}$ gerechnet. 

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Gegeben: $m = 400 \, \text{kg}$, $s = 0,1 \, \text{m}$, $g = 10 \, \frac{\text{m}}{\text{s}^2}$

$$F_G = F_F$$
$$m \cdot g = D \cdot s$$
$$D = \frac{m \cdot g}{s}$$
$$D = \frac{400 \, \text{kg} \cdot 10 \, \frac{\text{m}}{\text{s}^2}}{0,1 \, \text{m}} = \mathbf{40000 \, \frac{N}{m}}$$ 

</details>

---

b) Berechne die Frequenz, wenn sie mit den $400 \, \text{kg}$ schwingt. 

@rangeQuiz2( $f$ , 1.59, $\mathrm{Hz}$ )

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Die Eigenfrequenz $f$ eines Federpendels berechnet sich aus der Formel $f = \frac{1}{T}$. Da die Periodendauer $T = 2\pi \cdot \sqrt{\frac{m}{D}}$ ist, ergibt sich für die Frequenz:
$$f = \frac{1}{2\pi} \cdot \sqrt{\frac{D}{m}}$$
Setzen Sie die Masse $m = 400 \, \text{kg}$ und die Federkonstante $D = 40000 \, \frac{\text{N}}{\text{m}}$ ein. 

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

$$f = \frac{1}{2\pi} \cdot \sqrt{\frac{40000 \, \frac{\text{N}}{\text{m}}}{400 \, \text{kg}}}$$
$$f = \frac{1}{2\pi} \cdot \sqrt{100 \, \text{s}^{-2}}$$
$$f = \frac{10}{2\pi} \, \text{Hz} \approx \mathbf{1,59 \, Hz}$$ 

</details>

---

c) Zeichne für diese Schwingung das $y(t)$-Diagramm für die ersten zwei Perioden. 

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Ermitteln Sie zunächst die Periodendauer $T$ aus der Frequenz ($T = \frac{1}{f}$). Zeichnen Sie dann ein Koordinatensystem, bei dem die Zeit $t$ auf der x-Achse und die Auslenkung $y$ auf der y-Achse abgetragen wird. Da keine Dämpfung angegeben ist, zeichnen Sie eine harmonische Sinus- oder Kosinuskurve über den Zeitraum von $2 \cdot T$. 

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die Periodendauer beträgt $T = \frac{1}{1,59 \, \text{Hz}} \approx 0,63 \, \text{s}$.
Das Diagramm zeigt eine Sinuskurve mit:
- Einer Periodendauer von $0,63 \, \text{s}$.
- Einem Ende der Zeichnung nach zwei Perioden bei $t \approx 1,26 \, \text{s}$. 

</details>

---

d) Die gesamte Masse des Fahrzeugs von $1,6 \, \text{t}$ wird auf vier Räder mit jeweils vier baugleichen Federn verteilt. Begründe die folgende Aussage: *Die Eigenfrequenz des gesamten Fahrzeugs entspricht der aus Aufgabe b).* 

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Untersuchen Sie, wie viel Masse auf eine einzelne Feder entfällt, wenn das Gesamtgewicht von $1,6 \, \text{t}$ gleichmäßig auf vier Räder verteilt wird. Vergleichen Sie diesen Wert mit der Masse aus Teilaufgabe b) und ziehen Sie einen Schluss bezüglich der Formel für die Eigenfrequenz. 

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die Gesamtmasse beträgt $M = 1600 \, \text{kg}$. Da diese auf 4 Räder verteilt wird, trägt jedes Rad (und damit jede Feder) eine Masse von $m_{Rad} = \frac{1600 \, \text{kg}}{4} = 400 \, \text{kg}$.
Da die Federkonstante $D$ pro Rad identisch bleibt und die zu tragende Masse pro Rad ebenfalls $400 \, \text{kg}$ beträgt (wie in Aufgabe b), bleibt das Verhältnis $\frac{D}{m}$ in der Frequenzformel gleich. Folglich ist auch die Eigenfrequenz identisch.

</details>

---

e) Auf einer schlechten Straße verlaufen viele Rillen im Asphalt (welche zueinander einen festen Abstand haben) quer zur Fahrtrichtung. Fährt das Auto über diese Rillen, wird es während der Fahrt angeregt. Beschreibe, worauf ein Fahrer bei der Wahl der Geschwindigkeit achten sollte, um nicht den Resonanzfall zu provozieren.

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Überprüfe die Bedingungen für welche Resonanz auftritt. Überlege, warum die Fahrt über die Rillen im Asphalt im Auto einen Resonanzfall erzeugen können. Überlege anschließend, wie die Geschwindigkeit mit der Anregung des Fahrzeugs zusammenhängt.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Durch die Fahrt über die Rillen, wird der Schwinger (Auto) von außen angeregt. Entspricht die Frequenz der äußeren Anregung ungefähr der Eigenfrequenz des Schwingers, dann kann es zur Resonanz kommen und das Auto _schaukelt sich auf_, dass heißt die Amplitude der Schwingung steigt.

Je nachdem wie schnell das Auto fährt, ändert sich auf die Anregungsfreuqenz von außen. Wenn das Auto schneller fährt, wird die Anregungsfrequenz größer. 

Der Fahrer sollte also eine Geschwindigkeit wählen, bei der die Anregungsfrequenz entweder deutlich unter oder deutlich über diesem der Eigenfrequenz (Resonanzfrequenz) des Schwingers liegt. Er sollte also entweder langsam fahren (wenige Stöße pro Minute) oder deutlich schneller fahren. 

</details>

# Sachaufgabe zu mechanischen Wellen

__Aufgabe: Mechanische Wellen am Meer__

An einem Sommertag beobachtest du von einer Seebrücke aus die ankommenden Wasserwellen. Eine im Wasser stehender, am Boden fest verankerter Holzpfahl dient dir als Orientierungshilfe, um die Eigenschaften der Wellen zu bestimmen.


---

__Teilaufgabe a) Bestimmung der Frequenz__

Du stoppst die Zeit und stellst fest, dass innerhalb von t=20s genau 5 Wellenberge den Pfosten passieren. Ermittle die Frequenz f der Wasserwellen.

<p style='margin-left:10%'>

@rangeQuiz2( f , 0.25 , \mathrm{Hz} )

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungsweg </summary>

Die Frequenz f gibt an, wie viele Wellenberge pro Sekunde einen festen Punkt passieren. Sie berechnet sich aus der Anzahl der Wellen n dividiert durch die gemessene Zeit t.​
 
</details>


<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

__Gegeben:__ n=5, t=20s

__Gesucht:__ f

__Lösung:__ $$f=\frac{20\,\mathrm{s}}{5}=0,25\,\mathrm{Hz}$$

Die Frequenz der Wasserwellen beträgt 0,25Hz.

</details>

---

__Teilaufgabe b) Berechnung der Wellenlänge__

In Ausbreitungsrichtung der Wellen stehen mehrere Pfosten im Wasser. Diese Pfosten haben einen Abstand von 10 m. Du machst mit deinem Handy ein Foto zum richtigen Zeitpunkt und stellst fest, dass an jedem Pfosten ein Wellenberg ist. Zwischen den Pfosten befinden sich 7 weitere Wellenberge.

Skizziere eine seitliche Ansicht der Wellen und ergänze mindestens zwei Pfosten. Ermittle die Wellenlänge der Welle.

<p style='color:blue;margin-left:10%'>

@rangeQuiz2($\lambda$,0.8,$\mathrm{m}$)

</p>

---

__Teilaufgabe c) Berechnung der Ausbreitungsgeschwindigkeit__

Berechne die Ausbreitungsgeschwindigkeit v dieser Wasserwellen unter Verwendung der Frequenz aus Teilaufgabe a).

<p style='color:blue;margin-left:10%'>

@rangeQuiz2($v$,2.0,$\mathrm{\frac{m}{s}}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Zwischen der Ausbreitungsgeschwindigkeit c, der Wellenlänge λ und der Frequenz f besteht ein Zusammenhang. Er wird Wellenausbreitungsgleichung  genannt. Recherchiere die Wellenausbreitungsgleichung und nutze diese zur Berechnung der Wellengeschwindigkeit.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

__Gegeben:__ λ=8,0m, f=0,25Hz

__Gesucht:__ v

__Lösung:__ 

$$ v =λ \cdot f = 0,8\mathrm{m}\cdot2\,\mathrm{Hz} $$

Die Ausbreitungsgeschwindigkeit der Wellen beträgt 2,0 m/s.

</details>

---

__Teilaufgabe d) Veränderung der Wellenlänge__

Unter deinem Steg verändert sich die Tiefe des Wassers schlagartig und dadurch wird die Geschwindigkeit der Welle um 50% erhöht, während die Frequenz konstant bleibt. Ermittle die neue Wellenlänge $\lambda_{neu}$

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_{neu}$, 12.0 , $\mathrm{m}$ )

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungsweg </summary>

Ermittle erst die neue Wellengeschwindigkeit.

<p style='margin-left:10%'>

@rangeQuiz2($v_{neu}$,3.0, $\mathrm{\frac{m}{s}}$)

</p>

Nutze die Formel für die Wellenausbreitung um auf die neue Wellenlänge zu schließen.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

__Gegeben:__ $v_{neu} = 3.0 \,\mathrm{\frac{m}{s}}$, $f=0,25\,\mathrm{Hz}$

__Gesucht:__ $\lambda_{neu}$

__Lösung:__ $$ v_{neu} = \lambda_{neu} \cdot f  $$

$$ \lambda_{neu} = \frac{v_{neu}}{f} = 12 \,\mathrm{m}$$



</details>


---

e) Die Welle läuft mit einem Einfallswinkel von $\alpha=30^\circ$ auf die Kante mit der veränderten Wassertiefe zuläuft. Entscheide zunächst qualitativ ob und wenn ja, wie die Welle gebrochen wird. Ermittle anschließend den Brechungswinkel $\beta$.

<p style='margin-left:10%'>

[[ die Welle wird nicht gebrochen | die Welle wird zum Lot hin gebrochen | (die Welle wird vom Lot weg gebrochen) ]]

[[ $\alpha = \beta $ | $\alpha > \beta$ | ($\alpha < \beta $) ]]

</p>

<p style='margin-left:10%'>

@rangeQuiz2($\beta$, 48.59 , $^\circ$ )

</p>


<details style="color:blue;margin-left:10%">

<summary> Lösungsweg </summary>

Die Brechung von Wellen von einem Medium mit der Geschwindigkeit $v_1$ in ein Medium der Geschwindigkeit $v_2$ wird durch das Brechungsgesetz beschrieben. Recherchiere in deinen Unterlagen dieses Gesetz. Ermittle anschließend den Winkel $\beta$.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

Das Brechungsgesetz besagt:

$$ \dfrac{\sin\alpha}{\sin\beta} = \dfrac{v_1}{v_2} $$

Nach $\sin\beta$ umgestellt:

$$ {\sin\beta} = \sin\alpha\cdot\dfrac{v_2}{v_1} = 0,75 $$

Dann ergibt sich für $\beta$

$$ \beta = \sin^{-1}(\beta) \approx 48,59^\circ$$

</details>
