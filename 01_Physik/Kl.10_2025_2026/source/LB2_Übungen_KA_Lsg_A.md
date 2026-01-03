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

## A: Grundlagen zum Feder-Schwinger

1. Eine Feder wird von einer Kraft $F$ von $100\mathrm{N}$ um $5\mathrm{cm}$ zusammengedrückt. Ermitteln Sie die Federkonstante $D$.

<p style='margin-left:10%'>

@rangeQuiz2( $D$ , 2000, $\mathrm{\frac{N}{m}}$)

</p>

<details style="margin-left:10%;color:blue">

<summary> Lösungsweg </summary>

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
