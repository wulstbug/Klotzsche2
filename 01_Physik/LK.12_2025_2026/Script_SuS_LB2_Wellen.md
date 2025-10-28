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

> Eine @color(mechanische Welle, orange) ist die Ausbreitung eines Schwingungszustands von einem Ort im Raum zu einem anderen. 
>
>> Sie ist eine zeitlich __und räumlich__ periodische Änderung physikalischer Größen
>
> - Vorraussetzung sind __gekoppelte Schwinger__
>
> - eine Welle transportiert __Energie aber keine Masse__
>
> - die einzelnen schwingenden Teilchen bewegen sich ausschließlich um ihre Gleichgewichtslage


## 10. 1. Arten mechanischer Wellen

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

## 10. 2. Eigenschaften mechanischer Wellen

@color(_Tipp: Nutze für diese Übersicht eine eigene Seite_, orange)

---

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

<p class="newspaper">

![y-x-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/gJp99q4HHbZ7z8e/download)

<p class="cb">

![y-t-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/wfReL2Xbc5iGoXs/download)

</p>

</p>

---


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

> __Wellenausbreitungsgleichung__ (Zusammenhang zwischen $\lambda$, $f$ und $v$:):
>
> $$ \boxed{v = \lambda \cdot f}$$

---

> __(*) Wellengleichung $y(x, t)$ einer harmonischen Welle:__
>
> Die Auslenkung $y$ der gesamten Welle lässt sich zu jedem Zeitpunkt $t$ und an jedem Ort $x$ mit der Wellengleichung angeben:
>
> $$ \boxed{y(x,t) = y_{max} \cdot \sin\Big( \frac{2\pi}{\lambda}\cdot x-\frac{2\pi}{T}\cdot t\Big)}$$



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

Zur Darstellung der Ausbreitung von Wellen nutzen man __Wellenfronten__ und @color(__Wellennormale__,red)

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

## 10. 4. Huygens'sche Prinzip

> Jeder Punkt einer Wellenfront ist seinerseits wieder Ausgangspunkt für @color(kreis- bzw. kugelförmige Elementarwellen, red)

{{1}}
*************
![Huygernssches-Prinzip](https://diversewolken.ddns.net/nextcloud/index.php/s/zE2kb4mDwinM5M2/download)


-> [Simulation-Ausbreitung-Kreiswelle-EbeneWelle](https://www.leifiphysik.de/mechanik/mechanische-wellen/ausblick/huygenssches-prinzip-zur-beschreibung-von-mechanischen-wellen)
*************


### Aufgabenstellung zur Selbsständigen Präsentation

<p style="color:blue">

Aufgabe: 

1. Wählen Sie eines der folgenden Themen aus.

2. Erarbeiten Sie sich das Wellenphänomen.

3. Stellen Sie das Wellenphänomen dem Auditorium in einem kurzen Beitrag vor. Nutzen Sie die bereitgestellte Simulation um den Sachverhalt zu verdeutlichen.

4. Lösen Sie die Aufgabe allein oder gemeinsam mit dem Auditorium.


</p>

<p class="newspaper3">

__Reflexion:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/LK.12_2025_2026/Praesentationen_Wellen/Reflexion.md#1)

<p class="cb">

__Brechung:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/LK.12_2025_2026/Praesentationen_Wellen/Brechung.md#1)

<p class="cb">

__Beugung:__

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/01_Physik/LK.12_2025_2026/Praesentationen_Wellen/Beugung.md#1)

</p>

</p>

</p>



## 10. 5. Reflexion

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


## 10. 6. Brechung


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

## 10. 7. Beugung

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

??[Simulation-Kante](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+489+1.5625e-8%0Aw+0+255+132+514+132%0AS+2+0+1+511+1+0+1.399998+0+10+100+1+0%0Aw+0+511+-5+511+131%0A)
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


### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)


## 10. 8. Interferenz

{{0}}
***********
[LEIFI-Wellen](https://diversewolken.ddns.net/nextcloud/index.php/s/NeMj4nWBfqDXMWj/download)
***********

{{1}}
***********
> __Prinzip der ungestörten Überlagerung:__ Wellen durchdringen sich gegenseitig, ohne sich selbst oder einander zu verändern

> Die __Überlagerung__ oder __Superposition__ harmonischer Wellen wird als @color(Interferenz, red) bezeichnet. Diese hängt vom __Gangunterschied__ der inteferierenden Wellen ab.
>
> Umgangssprachlich: _"Interferenz ist die Addition der jeweiligen Auslenkungen"_

<p style="margin:5%;color:blue">

Wir untersuchen die Interferenz von Wellen grafisch als auch mathematisch.

[Geogebra-Interferenz-LK](https://www.geogebra.org/m/sd49erad)

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

---

***********

## 10. 9. Stehende Wellen

[StehendeWellen-Geogebra](https://www.geogebra.org/m/wcqzrbnh)

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

![RG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/oNFR69QaAyscHcM/download)

![RG_TB2](https://diversewolken.ddns.net/nextcloud/index.php/s/nAGqm7nxZKQ3WRo/download)



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

![BG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/FitcjCLbt8ecfCW/download)



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

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> __Beschreibung:__ Beim Doppelspaltexperiment schickt man @color(kohärentes, orange), einfarbiges Licht (z.B. Laserlicht) durch zwei nahe beieinander liegende Spalte, den sogenannten Doppelspalt. Das Licht fällt auf einen hinter dem Doppelspalt liegenden Schirm.
>
> __Beobachtung:__ Auf dem Schirm entsteht ein Muster aus vertikalen hellen und dunklen Streifen.
>
> __Erklärung:__ An den beiden Spalten entstehen laut dem huygen'schen Prinzip neue Elementarwellen. Diese Wellen überlagern (__interferieren__) sich und bilden beim Auftreffen auf einem Beobachtungsschirm ein Interferenzmuster aus hellen und dunklen Bereichen. ->[DoppelSpalt-Simulation](https://falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+578+1.5625e-8%0AS+2+0+1+511+1+0+1.633331+0+10+100+1+0%0A203+0+-60+54+574+54+2+6+15%0A)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Doppelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/PWMnf2JX4xiXamx/download "Prinzipskizze des Doppelspalt-Experiments")

</div>

</section>

---

> __Schlussfolgerung:__
>
> Das Muster auf dem Schirm ist nur durch Beugung und Interferenz, d.h. also durch Wellenerscheinungen, erklärbar: <br> => @color(Licht besitzt Welleneigenschaften, orange).

---

> __Eigenschaften von Lichtwellen:__

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

1. bei einer Lichtwelle schwingt das <span style="color:orange">***elektrische und das magnetische Feld.***</span>

2. eine Lichtwelle benötigt @color(***kein Medium***, orange) (anders als z.B. Schall[Luft], Wasserwellen[Wasser]) zur Ausbreitung. 

3. Licht ist eine @color(***Transversalwelle***, orange). 

4. Das elektromagnetische Feld @color(***transportiert Energie***, orange).

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

5. Die Ausbreitungsgeschwindigkeit (Lichtgeschwindigkeit) im Vakuum beträgt 

$$\boxed{c = 300.000 \dfrac{km}{s}}$$

6. Für die Lichtgeschwindigkeit in einem Medium gilt:

$$\boxed{c_{Medium} < 300.000 \dfrac{km}{s}}$$

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

6. Es gilt die Wellenausbreitungsgleichung: <br> $$ \boxed{c = \lambda \cdot f}$$ <br> Die Wellenlänge $\lambda$ der Lichtwelle bestimmt die <span style="color:orange">***Lichtfarbe***</span>.

</div>

</section>


## 10. 13. Bestimmung der Wellenlänge des Lichts am Doppelspalt

<section class="flex-container">

<div class="flex-child-3" style="min-width: 300px; margin-bottom: -10px">

![Doppelspalt5](https://diversewolken.ddns.net/nextcloud/index.php/s/rR93K2CqrPDwTDR/download)<!-- style="width:100%" -->

</div>

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

1. Die Spalte haben den Abstand $\blue{d}$, der Schirm hat vom Spalt den Abstand $\blue{e}.$

2. Im Punkt __A__ beobachten wir konstruktive Interferenz, wir nennen es @color(***Interferenz-Maximum***, orange). Dieses Maximum ergibt sich aus der Überlagerung der Elementarwellen aus den Spalten $s_1$ und $s_2$.

3. Für konstruktive Interferenz muss der Gangunterschied $\purple{\Delta s}$ einem Vielfachen der Wellenlänge entsprechen. <br> $$ \purple{\Delta s= k \cdot \lambda} \hspace{1cm}\mathrm{mit}\,\,k=1,\,2,..$$

4. Im rechtwinkligen Dreieck $\triangle S_1 S_2 P$ gilt:

$$ \dfrac{\purple{\Delta s}}{\blue{d}} = \boxed{\dfrac{\purple{k\cdot\lambda}}{\blue{d}} = \sin(\alpha) }$$

5. Im rechtwinkligen Dreieck $\triangle M O A$ gilt:

$$ \boxed{\tan(\alpha) = \blue{\dfrac{a}{e}}}$$

</div>

</section>

> Da wird die Größen $\blue{d,\,e}$ und $\blue{a}$ @color(__messen__, blue) können, lässt sich mit dem __Doppelspalt-Experiment__ die @color(Wellenlänge $\lambda$, purple) des Laserlichts bestimmen.

---

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
<p style="color:blue">

__Aufgabenstellung:__ 

- Erarbeiten Sie sich selbstständig die Grundlagen zum Thema: _Interferenz am Beugungsgitter_. 

- Nutzen Sie dafür (je nach Vorliebe) __Metzler__ S. 304-305 oder __Duden__ S. 413-414.

> Hinweis: Je nach Literaturquelle wird die Gitterkonstante mit dem Buchstaben $g$ oder $b$ angegeben.

- Achten Sie darauf, dass Sie die Beschreibung eines Beugungsgitters notiert haben, das Beugungsmuster verstanden haben und die zugehörigen Berechnungsformeln notiert haben.

- Bearbeiten Sie anschließend die experimentelle Aufgabe sowie die Abituraufgabe

</p>

### Experimentelle Aufgabe zum optischen Gitter

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

@rangeQuiz20($g$,12.5e-6,m)

</p>


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

<section class="flex-container">

<div class="flex-child-2" style="min-width: 200px; margin-bottom: -10px">

![Einzelspalt](https://diversewolken.ddns.net/nextcloud/index.php/s/obZ2NPnD2TyRds8/download)<!-- style="width:100%"-->

</div>

<div class="flex-child-1" style="min-width: 400px; margin-bottom: -10px">


__Beschreibung:__ Beträgt der Gangunterschied $\Delta s$ zwischen den beiden Randstrahlen gerade $\lambda$, dann kann man zu jedem Strahl aus dem Lichtbündundel der @color(__einen Hälfte__, green) einen Strahl aus dem Bündel der @color(__anderen Hälfte__, purple) finden, dessen Gangunterschied gerade $\frac{\lambda}{2}$ beträgt.Es kommt folglich zu einer Auslöschung aller Wellen.

> Für das **erste Minimum** gilt: $$ \boxed{\sin\alpha=\frac{\lambda}{d}}$$
>
> Für das **erste Maximum** gilt: $$ \boxed{\sin\alpha=\frac{(2k+1)\frac{\lambda}{2}}{d}}$$ <br> _Hinweis: Die Nebenmaxima (d.h. $k\neq0$) sind beim Einzelspalt von sehr geringer Intensität._

</div>

</section>

> -> [Simulation-LEIFI](https://www.leifiphysik.de/optik/beugung-und-interferenz/grundwissen/einzelspalt)

