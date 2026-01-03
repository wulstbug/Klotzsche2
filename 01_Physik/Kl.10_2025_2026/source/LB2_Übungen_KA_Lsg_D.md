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

## D: Sachaufgabe zu Schwingungen an einem PKW

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

