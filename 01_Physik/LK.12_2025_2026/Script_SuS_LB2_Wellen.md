<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/WqqAQR3Xk4gkpNG/download

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


### 10. 1. Arten mechanischer Wellen

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

### 10. 2. Eigenschaften mechanischer Wellen

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


### 10. 3. Darstellung der Wellenausbreitung mit Wellenfront und Wellennormale

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

### 10. 4. Huygens'sche Prinzip

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



### 10. 5. Reflexion

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


### 10. 6. Brechung


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

### 10. 7. Beugung

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


#### Übungsaufgaben zu Reflexion, Beugung, Brechung

__Quiz zur Licht-Brechung:__

- [Einfach](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-einfach)

- [Schwer](https://www.leifiphysik.de/optik/lichtbrechung/aufgabe/quiz-zur-lichtbrechung-schwer)

__Multiplayer-Quiz:__

- [Multiplayer-Learningapps](https://learningapps.org/604603)

__Zuordnung Wellenausbreitung:__

- [PaareZuordnen-Wellenausbreitung](https://learningapps.org/view4311115)


### 10. 8. Interferenz

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

### 10. 9. Stehende Wellen

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


### 10. 10. Begründung des Relfexionsgesetzes mit dem Huygens'schen Prinzip

![RG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/oNFR69QaAyscHcM/download)

![RG_TB2](https://diversewolken.ddns.net/nextcloud/index.php/s/nAGqm7nxZKQ3WRo/download)



#### Übungsaufgaben

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

### 10. 11. Begründung des Brechungsgesetzes mit dem Huygens'schen Prinzip

![BG_TB1](https://diversewolken.ddns.net/nextcloud/index.php/s/FitcjCLbt8ecfCW/download)



#### Aufgaben zu Wellen

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