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

@onload
window.LIA.settings.font_size = 2


const canvas = document.querySelector('.lia-canvas')
if (canvas) {
  canvas.classList.remove('lia-navigation--visible')
  canvas.classList.add('lia-navigation--hidden')
}

@end

mode: presentation


-->

## C: Grundlagenaufgaben zu mechanischen Wellen

1. __Erläuterung Wellenphänomene:__

     [Erläuterung Wellenphänomene - bitte anklicken](http://10.102.1.3:3001/?q=Stelle%20mir%20f%C3%BCnf%20Verst%C3%A4ndnisfragen%20zum%20Thema%20Eigenschaften%20Mechanischer%20Wellen%20,d.h.%20Beugung,%20Brechung,%20Reflexion%20und%20Interferenz.%20Mein%20Niveau%20ist%20Klasse%2010%20Gymnasium.%20Stelle%20mir%20die%20Fragen%20einzeln.%20Warte%20auf%20meine%20Antwort%20und%20bewerte%20meine%20Antwort%20auf%20einer%20Skala%20von%200-10.%20Gib%20mir%20anschlie%C3%9Fend%20eine%20Gesamteinsch%C3%A4tzung.%20Achte%20auf%20das%20Niveau%2010.%20Klasse.%20Die%20Begriffe%20Beugung,%20Interferenz%20und%20Brechung%20haben%20wir%20in%20der%20letzten%20Unterrichtseinheit%20zum%20ersten%20mal%20kennengelernt.)

2. __Mechanische Wellen an einem Seil:__ 

<p style="margin-left:10%">

![Seilwelle.gif](https://diversewolken.ddns.net/nextcloud/index.php/s/YeoFETY4PgBqTn8/download)Eine Wellenmaschine erzeugt an einem sehr langen, gespannten Seil eine harmonische Querwelle. Die Welle breitet sich mit einer Ausbreitungsgeschwindigkeit von v=12,0m/s aus. Der Abstand zwischen zwei aufeinanderfolgenden Wellenbergen (die Wellenlänge) beträgt λ=3,0m.

a) Berechnen Sie die Frequenz f der Schwingung, mit der die Wellenmaschine das Seil anregt.

<p style='margin-left:10%'>

@rangeQuiz2( f , 4.0, $\mathrm{Hz}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungweg </summary>

Zwischen der Ausbreitungsgeschwindigkeit v, der Wellenlänge λ und der Frequenz f besteht der grundlegende Zusammenhang der Wellenausbreitungsgleichung. Recherchiere diesen in deinem Hefter.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

_Hinweis: In dieser Lösung wird für die Geschwindigkeit der Welle der Buchstabe c, statt v verwendet._

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

</p>
