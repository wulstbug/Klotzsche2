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

## E: Sachaufgabe zu mechanischen Wellen

__Aufgabe: Mechanische Wellen am Meer__

![Buhlen](https://www.ostfriesland-nordsee.com/wp-content/uploads/2025/02/Buhnen-Kuestenschutz-960x560.jpg) An einem Sommertag beobachtest du von einer Seebrücke aus die ankommenden Wasserwellen. Eine im Wasser stehender, am Boden fest verankerter Holzpfahl dient dir als Orientierungshilfe, um die Eigenschaften der Wellen zu bestimmen.

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

