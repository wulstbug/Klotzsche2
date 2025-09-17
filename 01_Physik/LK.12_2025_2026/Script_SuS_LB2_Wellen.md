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

3. Wählen Sie die korrekte Wellengleichung $y(t)$ für den Ort $x=0\,\mathrm{m}$.

<p style="margin-left:10%">

[[ ( $y(t) = 1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ ) | $y(t) = 1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | $y(t) = -1,5\,\mathrm{m}\cdot\sin(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ | $y(t) = -1,5\,\mathrm{m}\cdot\cos(0,628\,\mathrm{\frac{1}{s}}\cdot t)$ ]]

</p>

4. Wählen Sie die korrekte Wellengleichung $y(x)$ für den Zeitpunkt $t=0\,\mathrm{s}$.

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