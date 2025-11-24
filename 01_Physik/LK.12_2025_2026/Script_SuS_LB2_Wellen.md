<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/WqqAQR3Xk4gkpNG/download

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

# LB 10 Mechanische und elektromagnetische Wellen


<iframe src="https://www.geogebra.org/classic/sn4xvwsj?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## 10. 1. Arten mechanischer Wellen

## 10. 2. Eigenschaften mechanischer Wellen

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

## 10. 4. Huygens'sche Prinzip

## 10. 5. Reflexion

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

## 10. 7. Beugung

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

### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)


## 10. 8. Interferenz

## 10. 9. Stehende Wellen

[StehendeWellen-Geogebra](https://www.geogebra.org/m/wcqzrbnh)

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


## 10. 12. Das Doppelspalt-Experiment

## 10. 13. Bestimmung der Wellenlänge des Lichts am Doppelspalt

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

## 10. 16. Intereferenz an dünnen Schichten

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
 
## 10. 18. Das Spektrum elektromagnetischer Wellen


<iframe src="https://learningapps.org/watch?v=pgqf50hd225" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

_Bitte anschließend stichpunktartig übernehmen_

## 10. 19. Interferometer


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
