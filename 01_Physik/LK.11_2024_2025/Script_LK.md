<!--
author: Christian Golnik

language: de

@style
.lia-effect__circle {
    display: none !important;
}
.lia-slide__footer {
     display: none !important;
} 


@media (min-width: 600px) {
    .newspaper {
        column-count: 2;
        column-gap: 40px;
        column-rule: 1px solid lightblue;
    }
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
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
<div style="float:left">
@0$\ $=$\ $ 
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
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
<div style="float:left">
@2
</div>
</div>
@end

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0 = 
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
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
<div style="float:left">
@2
</div>
</div>
@end

@@@ ogy.de/11Ph2 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Physik LK 2024/2025

@uhr

# LB 1 - Erhaltungssätze und ihre Anwendungen

## 1.1 - Wiederholung Energieformen

__Energie__

{{1}}
*****************
> Defition: Energie beschreibt die Fähigkeit eines Körpers:
*****************
{{2}}
*****************
>- mechanische Arbeit zu verrichten (z.B. Beschleunigen, Verformen)
>- Licht auszusenden
>- Wärme abzugeben
*****************

{4}{__Energieformen__}

{{5}}
*****************
>__Mechanische Energieformen:__
>
>- __Kinetische Energie (Bewegungsenergie)__
>- __Potentielle Energie (Lageenergie)__
>- Rotationsenergie (Drehungen)
>- __Spannenergie (z.B. gespannte Feder)__

>- __Thermische Energie (Wärmeenergie)__
>- __Elektrische Energie__
>- Magnetische Energie
>- Strahlungsenergie (Lichtenergie)
>- Chemische Energie
>- Kernenergie (Atomenergie)
*****************

## Übung: Zuordnung Energieformen

Übungs 1: _Zuordnung Energieformen_

<iframe src="https://learningapps.org/watch?app=23986132" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

Übung 2: _Zuordnung Energieformen_

<iframe src="https://learningapps.org/watch?app=28854190" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

## 1.2 Erhaltungsgrößen

{{1}}
************
> Ist eine physikalische Größe eine __Erhaltungsgröße__, so {2}{ändert sich der Wert dieser physikalischen Größe nicht. <br> <br> In einem __abgeschlossenen System__ ändern sich Erhaltungsgrößen nicht.}

__Beispiele für Erhaltungsgrößen (in einem abgeschlossenen System):__
************

{{2}}
************
- __Gesamtenergie__
- __elektrische Ladung__
- __Impuls__ (bzw. Drehimpuls)
************


## 1.3 Energieerhaltungssatz

{{1}}
************
> In einem geschlossenen System ist __Gesamtenergie__ eine Erhaltungsgröße, d.h. die Summe aller Energien ist konstant.
************

{{2}}
************
> __Schlussfolgerung:__ Energie kann weder erzeugt noch vernichtet werden, sondern nur von einer Form in eine andere umgewandelt werden.
************

## 1.4 Beispiel - Schräger Wurf

Schräger Wurf einer Kugel, welche durch eine gespannte Feder beschleunigt wird.

{{1}}
*************
__Versuchsskizze:__

![Tafelbild_SchrägerWurf](https://diversewolken.ddns.net/nextcloud/index.php/s/jGeEEkxHXj9m8RC/download)
*************

{{2}}
*********************
__Energieumwandlungen:__

![Tafelbild_SchrägerWurf_Energie](https://diversewolken.ddns.net/nextcloud/index.php/s/EXzBa85WQYZQCeD/download)
*********************

## 1.5 Berechnung der kinetischen Energie

{{1}}
************
__Defintion:__ Kinetische Energie ist die in der Bewegung eines Körpers gespeicherte Energie. Sie hängt von der Geschwindigkeit $v$ des Körpers und seiner Masse $m$ ab.
************

{{2}}
***************
> __Formel:__ $$E_{kin} = \dfrac{1}{2} \cdot m \cdot v^2$$
>
>  v .. Geschwindigkeit in $\Big[ \dfrac{m}{s} \Big]$ 
>
>  m .. Masse in $\Big[ kg \Big]$

***************

{{3}}
***************
> __Einheit: 1 J [Joule]__
>
> _Hinweis: Rechne die Geschwindigkeit immer in **$\frac{m}{s}$** und die Masse immer in **kg** um, dann erhälst du als Ergebnis die Einheit Joule_
***************

{{4}}
***************
> __Beispielaufgabe:__
>
> Bestimme die kinetische Energie, die ein Auto (1,5 t) bei einer Geschwindigkeit von $ 100 \frac{km}{h}$  besitzt.
***************

{{5}}
***************
> __Berechnung:__
>
> geg.: 
>
> $\hspace{1cm}$ $v = 100 \frac{km}{h}$
>
> $\hspace{1cm}$ $m = 1,5 t$
>
> ges.: 
>
> $\hspace{1cm}$ $E_{kin}$
***************

{{6}}
***************
> Lsg.: 
>
> $\hspace{0.5cm}$ _1. Umrechnen der Einheiten_
>
> $\hspace{1cm}$  $v = 100 \frac{km}{h} = \frac{100}{3,6} \frac{m}{s} \approx 27,28 \frac{m}{s} $
>
> $\hspace{1cm}$ $m = 1,5 t = 1500 kg$
***************

{{7}}
***************
> $\hspace{0.5cm}$ _2. Berechnung_
>
> $\hspace{1cm}$  $E_{kin} = \dfrac{1}{2} \cdot m \cdot v^2 $
>
> $\hspace{1cm}$  $E_{kin} = \dfrac{1}{2} \cdot 1500 kg \cdot (27,78 \frac{m}{s})^2 $
***************

{{8}}
***************
> Ergebnis:
>
> $\hspace{1cm}$  $E_{kin} = 578796,3 J \approx 578,8 kJ $
***************

## 1.6 Berechnung der potentiellen Energie

{{1}}
************
__Defintion:__ Potentielle Energie eines Körpers ist die in seiner der Lage (d.h. Höhe) über einem Bezugspunkt (z.B. Erdboden) gespeicherte Energie. Sie hängt von der Höhe h und der Masse m des Körpers ab.
************

{{2}}
***************
> __Formel:__ $$E_{pot} = m \cdot g \cdot h. $$
>
>  $m$ .. Masse in $[kg]$
>
> $h$ .. Höhe in $[m]$
>
> $g$ .. Ortsfaktor: $g = 9,81 \frac{m}{s^2}$ (Konstante)

***************

{{3}}
***************
> __Einheit: 1 J [Joule]__
***************

{{4}}
***************
> __Beispielaufgabe:__
>
> Bestimme die potentielle Energie, die ein Auto (1,5 t) auf einem Berg mit der Höhe 50m besitzt.
***************

{{5}}
***************
> __Berechnung:__
>
> geg.: 
>
> $\hspace{1cm}$ $m = 1,5t = 1500 kg$
> 
> $\hspace{1cm}$ $h = 50 m$
>
> $\hspace{1cm}$ $g = 9,81 \frac{m}{s^2}$
>
> ges.: 
>
> $\hspace{1cm}$ $E_{pot}$
***************

{{6}}
***************
> Lsg.:
>
> $\hspace{1cm}$  $E_{pot} = m \cdot g \cdot h $
>
> $\hspace{1cm}$  $E_{pot} = 1500 kg \cdot 9,81\frac{m}{s^2} \cdot 50m $
***************

{{7}}
***************
> Ergebnis:
>
> $\hspace{1cm}$  $E_{pot} = 735750 J \approx 735,8 kJ $
***************

## 1.7 Berechnung der Spannenergie

{{1}}
************
__Defintion:__ Spannenergie ($E_{sp}$) ist die in einer gespannten mechanischen Feder gespeicherte Energie. Sie hängt von der Federkonstante $D$ der Feder und dem Spannweg $s$ ab.
************

{{2}}
***************
> __Formel:__ $$E_{sp} = \dfrac{1}{2} \cdot D \cdot s^2$$
>
>  D .. Federkonstante in $\Big[ \dfrac{N}{m} \Big]$ 
>
>  s .. Spannweg gegenüber Ruhelage in $\Big[ m \Big]$

***************

{{3}}
***************
> __Einheit: 1 J [Joule]__
***************

{{4}}
***************
> __Beispielaufgabe:__
>
> Bestimme die Spannenergie, welche eine Feder ($D=5\dfrac{N}{cm}$) besitzt, welche 3 cm gespannt wird.
***************

{{5}}
***************
> __Berechnung:__
>
> geg.: 
>
> $\hspace{1cm}$ $D = 5\dfrac{N}{cm}$
> 
> $\hspace{1cm}$ $s = 3 cm$
>
> ges.: 
>
> $\hspace{1cm}$ $E_{sp}$
***************

{{6}}
***************
> Lsg. 1: 
>
> $\hspace{0.5cm}$ _1. Umrechnen der Einheiten_
>
> $\hspace{1cm}$  $D = 5 \frac{N}{cm} = 5 \frac{100\cdot N}{100 \cdot cm} = 500 \frac{N}{m}$
>
> $\hspace{1cm}$ $s = 3\,cm = 0,03\,m$
***************

{{7}}
***************
> $\hspace{0.5cm}$ _2. Berechnung_
>
> $\hspace{1cm}$  $E_{sp} = \dfrac{1}{2} \cdot D \cdot s^2 $
>
> $\hspace{1cm}$  $E_{sp} = \dfrac{1}{2} \cdot 500 \frac{N}{m} \cdot (0,03\,m)^2 $
***************

{{8}}
***************
> Ergebnis:
>
> $\hspace{1cm}$  $E_{sp} = 0,225\,J \approx 225\,mJ $
***************

{{9}}
***************
> Lsg. 2: 
>
> $\hspace{0.5cm}$ _1. Berechnung_
>
> $\hspace{1cm}$  $E_{sp} = \dfrac{1}{2} \cdot D \cdot s^2 $
>
> $\hspace{1cm}$  $E_{sp} = \dfrac{1}{2} \cdot 5 \frac{N}{cm} \cdot (3\,cm)^2 $
>
> $\hspace{1cm}$  $E_{sp} = 22,5 \Big[ \frac{N}{cm} \cdot cm^2 = N\cdot cm \Big] $
>
***************

{{10}}
***************
> $\hspace{0.5cm}$ _2. Umrechnung_
>
> $\hspace{1cm}$ Achtung!! $1 J = 1 N \cdot m = 1 N \cdot 100 cm = 100 N \cdot cm$
>
> $\hspace{1cm}$ => $E_{sp} = 0,225 N\cdot m = 0,225 J$
***************

{{11}}
***************
> Ergebnis:
>
> $\hspace{1cm}$  $E_{sp} = 0,225\,J \approx 225\,mJ $
***************

## 1.8 Analyse des schrägen Wurfs (siehe 1.4)

__Energierelationen:__

![Tafelbild_SchrägerWurf_Energie](https://diversewolken.ddns.net/nextcloud/index.php/s/EXzBa85WQYZQCeD/download)

__Messwerte aus Experiment:__

![SchrägerWurf_Messwerte_1](https://diversewolken.ddns.net/nextcloud/index.php/s/pkj48Zo77dGA36G/download)

__Berechnungen aus Messwerten:__

Die Spannenergie $E_{sp1}$ entspricht der potentiellen Energie $E_{pot}$ beim senkrechten Schuss und maximaler Höhe $h_{max}$.

$$E_{sp1} = E_{pot} = m \cdot g \cdot h = 0,017kg \cdot 9,81\frac{N}{kg} \cdot 0,41m \approx 0,068 J $$

Die Federkonstante $D$ erhält man durch umstellen der Gleichung für $E_{sp1}=\frac{1}{2}\cdot D \cdot s^2$ als

$$ D = \dfrac{2\cdot E_{sp1}}{s^2} = \dfrac{2\cdot 0,068 J}{0,04^2 m^2} = 85 \frac{N}{m}$$

Setzt man Energieerhaltung voraus und vernachlässigt Energieverluste durch Reibung so entspricht die kinetische Energie im Punkt 4 genau $E_{sp1}$

$$ E_{kin4} = E_{sp1} = 0,068 J.$$

Die Geschwindigkeit der Kugel im Punkt 4 erhält man durch umstellen der Gleichung für $E_{kin4} = \frac{1}{2} \cdot m \cdot v^2$.

$$ v_4 = \sqrt{\dfrac{2\cdot E_{kin4}}{m}} = \sqrt{\dfrac{2\cdot 0,068 J}{0,017 kg}} \approx 2,84 \frac{m}{s}$$


## Aufgabe Bungeespringerin

| | |
| ![Bungee_Mtz67_Bsp2](https://diversewolken.ddns.net/nextcloud/index.php/s/XbQpeLEaPG88bZk/download) | Eine Bungeespringerin (60 kg) beabsichtigt, von einer Brücke herabzuspringen. Das Bungeeseil hat im ungedehnten Zustand eine Länge von $l=25m$ und der Abstand des Sprungpunktes zur Wasseroberfläche beträgt 45m. <br> Nimm an, dass für die Seildehnung das Hook'sche Gesetz gilt und die Federkonstante $D = 160 \frac{N}{m}$ beträgt. <br> <br> Ermittle den tiefsten Punkt des an den Füßen befestigten Seils (über der Wasseroberfläche). <details>

  <summary>Hinweise zur Lösung</summary>

<p>
Hat die Springerin den tiefsten Punkt erreicht, so hat sich die potentielle Energie, komplett in Spannenergie des Seils umgewandelt.
<br>
Die potentielle Energie am Ort (l+s) unterhalb des Absprungs berechnet sich mit

$$ E_{pot} = m \cdot g \cdot (l+s). $$

Hier ist l die Länge des Seils und s die zusätzliche Dehnung des Seils über die Ruhelage hinaus. Die Spannenergie die Seils berechnet sich mit

$$ E_{sp} = \frac{1}{2} \cdot D \cdot s^2.$$

Wie oben beschrieben setzen wir nun für den untersten Punkt $E_{pot} = E_{sp}$, d.h.

$$m \cdot g \cdot (l+s) = \frac{1}{2} \cdot D \cdot s^2 $$

<iframe scrolling="no" title="Loesung_Bungee_Fehlerrechnung" src="https://www.geogebra.org/material/iframe/id/rjvn7mcv/width/800/height/200/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/true/ctl/false" width="100%" height="200px" style="border:0px;"> </iframe>

Diese Gleichung enthält als Unbekannt nur s. Mit Hilfe des Taschenrechners erhält man die Lösungsmenge $$\mathbb{L} = \{-10,37 ; 17,73\}.$$

Die negative Lösung ist unphysikalisch, somit bleibt für $s = 17,73 m$ übrig. Die gesuchte Höhe über der Wasseroberfläche ergibt

$$ 45 - (l + s) = 45 - (25+17,73) = 2,27 m$$
</p>

</details> |

__Weitere Aufgaben:__ Metzler LB S. 67 Aufgabe 2, 3, 11*

<details>

  <summary>Lösungen 2</summary>

    $\hspace{1cm}$ 2a) $E_{kin} \approx 111`111 J $  
    $\hspace{1cm}$ 2b) $h \approx 14,16 m$

</details>

<details>

<summary>Lösung 3</summary>

![Lsg_Metz67_3](https://diversewolken.ddns.net/nextcloud/index.php/s/AawA8akxi3W9TDR/download)

</details>


<details>

<summary>Lösung 11*</summary>

![Lsg_Metz67_11](https://diversewolken.ddns.net/nextcloud/index.php/s/EH9Q3z2DkEEJ7tP/download)

</details>

## 1.9 Fehlerrechnung zur Aufgabe: Bungeespringerin

> __Annahme zur Fehlerrechnung:__ Für die Federkonstante des Seils wird vom Hersteller eine Tolleranz (d.h. Ungenauigkeit oder Messfehler) von 5% angegeben. Die Masse eines Menschen ist ebenfalls natürlichen Schwankungen unterworfen. Nimm hier eine Toleranz von $\pm\,1\,kg$ an.

> __Aufgabenstellung:__ Überprüfe, ob der Spung für die Bungeespringerin sicher ist.

{{1}}
***************
> __Analyse:__
>
> geg.: 
>
> $\hspace{1cm}$ $D = 160\frac{N}{m}$ "$\pm5\%$" = $160 \frac{N}{m} \pm 8 \frac{N}{m}$
> 
> $\hspace{1cm}$ $m = 60 kg \pm 1 kg$
>
> $\hspace{1cm}$ $l = 25 m$
>
> $\hspace{1cm}$ $h_{max} = 45\,m$
>
> ges.: 
>
> $\hspace{1cm}$ $s$...maximale Seildehnung im __ungünstigsten Fall__
***************

{{2}}
***************
> Lsg.:
>
> $\hspace{1cm}$  Die maximale Seildehnung $s$ wird größer, wenn 
***************

{{3}}
***************
> $\hspace{1cm}$  die Masse steigt und die Federkonstante des Seils kleiner wird.
***************

{{4}}
***************
> $\hspace{1cm}$ d.h. um die maximal mögliche Seildehnung zu ermitteln, setzen wir in unseren Lösungsansatz: 
>
> $\hspace{1cm}$ 1. die maximale Masse ($m=60+1kg=61kg$) und 
>
> $\hspace{1cm}$ 2. die minimale Federkonstante ($160-8\frac{N}{m}= 152\frac{N}{m}$) ein.
***************

{{5}}
***************
> $\hspace{1cm}$ Löse die Gleichung: 
>
> $$m \cdot g \cdot (l+s) = \frac{1}{2} \cdot D \cdot s^2 $$
>
> $$61\,kg \cdot 9,81 \frac{m}{s^2} \cdot (25 m+s) = \frac{1}{2} \cdot 152\frac{N}{m} \cdot s^2 $$
***************

{{6}}
***************
<iframe scrolling="no" title="Loesung_Bungee_Fehlerrechnung" src="https://www.geogebra.org/material/iframe/id/sfkffrzq/width/800/height/200/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/true/ctl/false" width="100%" height="200px" style="border:0px;"> </iframe>
***************



{{7}}
***************
> $$\mathbb{L} = \{-10,64 ; 18,51\}$$
> 
> Maximal Höhe über dem Boden beträgt $45m-(25m+18,51m)=1,49m$
***************

## 1.10 Mechanische Arbeit

{{1}}
*******
> __Definition:__ Mechanische Arbeit wird verrichtet, wenn ein Körper durch eine Kraft bewegt oder verformt wird.<br>
>
> _Anders ausgedrückt: Arbeit ist die mit Kraft über eine Systemgrenze übertragene Energie_
*******

<p class="newspaper">
{{2}}
*******
> Formelzeichen: $W$
>
> Formeln:
>
> $\hspace{1cm}$ $ W = \Delta E $ (_Arbeit ist Energieänderung_)
>
> $\hspace{1cm}$ $ W = F \cdot s \cdot \cos\alpha$
>
> $F$ .. wirkende Kraft in $[N]$
>
> $s$ .. zurückgelegter Weg in $[m]$
>
> $\alpha$ .. Winkel zwischen Kraft $F$ und Weg $s$
*******

<p class="cb">

{{2}}
*******
![Arbeit_Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/K9JzW2EaRmayMQN/download)
*******
</p>

</p>

{{3}}
*******
>_Hinweis 1: Im Gegensatz zur Energie (Zustandsgröße) ist die Arbeit eine Prozessgröße._
>
> _Hinweis 2: Wenn die Kraft parallel zum zurückgelegten Weg wirkt, gilt_
>
> $\hspace{1cm}$ $ W = F \cdot s$
>
> _denn für  $\alpha=0$ ist $\cos\alpha=1$_
*******

{{4}}
*******
__Spezielle mechanische Arbeiten:__

$\hspace{1cm}$ __Hubarbeit $W_H$:__ Ein Kran hebt einen Körper nach oben. 
$$ W_H = \Delta E_{pot}$$
*******

{{5}}
*******
$\hspace{1cm}$ __Beschleunigungsarbeit $W_B$:__ Ein Auto wird vom Motor auf gerader Strecke beschleunigt 
$$W_B = \Delta E_{kin}$$
*******

## 1.11 Hubarbeit $W_H$ und potentielle Energie $E_{pot}$

<p class="newspaper">

{0-1}{![HubArbeit_Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/f7KCX6MpoLz4P5w/download)}

{1}{![HubArbeit_Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/PXmtZ73HgaM2PQx/download)}

<p class="cb">

Ein Körper der Masse $m$ wird die Höhe $h$ senkrecht nach oben angehoben. 
<br>
Berechne die Hubarbeit <br>
$ W_H = \Delta E_{pot} $
<br>
<br>
{1}{Die aufzuwindende Kraft $F$ ist die Gewichtskraft}
{1}{$ F_g = m \cdot g. $} 
{1}{Diese Kraft wirkt parallel zur Höhe $h$.}
<br>
<br>
{2}{Die Hubarbeit $W_H$ und somit der Zugewinn an potentieller Energie lässt sich berechnen mit}
<br>
{2}{$W_H = F_g \cdot h$}
<br>
{2}{$W_H = m \cdot g \cdot h = \Delta E_{pot}$}
<br>
<br>
{3}{Anders ausgedrückt: Am Körper wird die Hubarbeit $W_H$ verrichtet und er gewinnt die potentielle Energie $m \cdot g \cdot h$ dazu.}

</p>

</p>

## 1.12 Beschleunigungsarbeit $W_B$ und kinetische Energie $E_{kin}$

Es gilt:

> $$ W_B = \Delta E_{kin} $$

_Untersuche für die gleichmäßige Beschleunigung eines Körpers der Masse $m$ entlang der Wegstrecke $s$ mit der beschleuinigenden Kraft $F$ den durch Beschleunigungsarbeit $W_B$ verrichteten Zugewinn an kinetischer Energie $\Delta E_{kin}$._

![BeschlArbeit_Skizze](https://diversewolken.ddns.net/nextcloud/index.php/s/TESsTwEAHB9xHew/download)

{{1}}
*********
_Nutze dafür:_

> 2. Newton'sche Axiom
>
> $$ F = m \cdot a $$

_sowie die Gleichungen für die gleichmäßig beschleunigte Bewegung_

> $$s = \frac{1}{2} \cdot a \cdot t^2$$
> 
> $$v = a \cdot t $$
*********

{{2}}
****************
__Lösung:__

Beschleunigungsarbeit $W_B$ ist definiert als

$$ W_H = F \cdot s $$

Wir nutzen für die Beschreibung der Kraft F das zweite Newton'sche Axiom

$$ F = m \cdot a $$

und setzen bei $W_B$ ein

$$  W_B = F \cdot s = m \cdot a \cdot s$$.

Mit der Formel für die gleichmäßig beschleunigte Bewegung für den zurückgelegten Weg s gilt

$$s = \frac{1}{2} \cdot a \cdot t^2$$

kann man für $W_B$ notieren

$$W_B = m \cdot a \cdot s =  m \cdot a \cdot \frac{1}{2} \cdot a \cdot t^2 $$

und zusammengefasst

$$ W_B = \frac{1}{2} \cdot m \cdot a^2 \cdot t^2. $$

Nutzt man nun noch $ a = \frac{v}{t}$ so ergibt sich

$$ W_B = \frac{1}{2} \cdot m \cdot a^2 \cdot t^2 = \frac{1}{2} \cdot m \cdot \frac{v^2}{t^2} \cdot t^2 $$

und es bleibt

$$ W_B = \frac{1}{2} \cdot m \cdot v^2 $$

Die mechanische Beschleunigungsarbeit und somit auch die Änderung der kinetischen Energie lässt sich ausdrücken mittels

$$ W_B = \Delta E_{kin} = \frac{1}{2} \cdot m \cdot v^2 $$
****************

## 1.13 Grafische Interpretitation der mechanischen Arbeit

> In einem Kraft-Weg-Diagram ($F-s-Diagramm$) entspricht die mechanische Arbeit der Fläche unter dem $F-s-Graphen$.

__Beispiele:__

| 1 | 2 | 3 | 4 |
| ![Konstante-Kraft](https://www.leifiphysik.de/sites/default/files/2019/10/image/Arbeit_einfach_0.svg) | {1}{![ZUsammengesetzte-Kräfte](https://www.leifiphysik.de/sites/default/files/2019/10/image/Arbeit_doppelt_0.svg)} | {2}{![LinearerKraftanstieg-Kräfte](https://www.leifiphysik.de/sites/default/files/2019/10/image/Arbeit_doppelt_0.svg)} | {3}{![Nicht_Konstante-Kraft2](https://diversewolken.ddns.net/nextcloud/index.php/s/PW5ZfpqBGGFcWJx/download)} |

{{4}}
**************
_Hinweis 1: Lässt sich die Fläche unter dem Graphen geometrisch bestimmen (z.B. Dreieck), so kann die mechanische Arbeit darüber berechnet werden._

_Hinweis 2: In allgemeinen Fällen (siehe Beispiel 5) kann die Fläche in kleine Abschnitte ("Streifen") unterteilt werden, deren Fläche dann addiert wird._

**************

## Beispiel: Bogenschießen

_Arbeitsauftrag: Bearbeite die Aufgabe a) zum Bogenspannen bei Leifi-Physik. Die Lösungen sind ebenfalls gegeben._

??[Leifi-Bogenschießen](https://www.leifiphysik.de/mechanik/energieerhaltung-und-umwandlung/aufgabe/spannarbeit-beim-bogenschiessen)

## 1.14 Herleitung Federspannarbeit -> Spannenergie

> $$ W_{sp} = \Delta E_{sp} $$

| Kraft $F$ | $F-s-Diagramm$ |
| {1}{![FederSpannarbeit](https://diversewolken.ddns.net/nextcloud/index.php/s/Q5nf7D3WYQCxNSW/download)} | {2}{![F-s-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/ijzAksKEza8XDKP/download)} |
| {1}{Annahme: Hook'sche Gesetz <br> => Kraft ~ Dehnung}| {3}{$W_{sp} = \frac{1}{2} \cdot F_{E} \cdot s $} <br> <br> {4}{$W_{sp} = \frac{1}{2} \cdot D \cdot s \cdot s $} <br> <br> {5}{$W_{sp} = \frac{1}{2} \cdot D \cdot s^2 = \Delta E_{sp} $}|

## Übungsaufgaben - Energieerhaltung LB

Duden S. 169: Aufgaben 58, 60, 62 (a,b, c*)

<details>

<summary>Lösung 58</summary>

![Lsg_Duden168_58](https://diversewolken.ddns.net/nextcloud/index.php/s/Wp7CnW3wB6kL7kp/download)

</details>


<details>

<summary>Lösung 60a</summary>

![Lsg_Duden168_60a](https://diversewolken.ddns.net/nextcloud/index.php/s/qMH7fNBPnS9wPKa/download)

</details>

<details>

<summary>Lösung 60b</summary>

![Lsg_Duden168_60b](https://diversewolken.ddns.net/nextcloud/index.php/s/jXGnXQTinNxB8Y2/download)

</details>

<details>

<summary>Lösung 62ab</summary>

![Lsg_Duden168_60ab](https://diversewolken.ddns.net/nextcloud/index.php/s/NNzfYC5dcqc8joz/download)

</details>

<details>

<summary>Lösung 62c*</summary>

![Lsg_Duden168_60c](https://diversewolken.ddns.net/nextcloud/index.php/s/6r2B7rMkmeLWfYj/download)

</details>

Metzler S. 67, 8

<details>

<summary>Lösung 8</summary>

![Lsg_Metzler_67_8](https://diversewolken.ddns.net/nextcloud/index.php/s/yXL4GaHJjpi9HCw/download)

</details>

Kommentar: CG

@@@ ## Aufgaben Pitty-Physik

@@@ Reibung:

@@@ 739, 1335

## Aufgaben - Mechanische Energien und Reibung

??[Aufgaben Mechanische Energien und Reibung](https://diversewolken.ddns.net/nextcloud/index.php/s/i5KTPn8kwebfkxX/preview)

[Aufgaben Mechanische Energien und Reibung](https://diversewolken.ddns.net/nextcloud/index.php/s/i5KTPn8kwebfkxX)

[Lösung MechEnergie Und Reibung](https://diversewolken.ddns.net/nextcloud/index.php/s/EoxcWHzsLKd9AEy)

## Eine neue Erhaltungsgröße

!?[ThreeBallDrop](https://www.youtube.com/watch?v=2UHS883_P60)

## Zwei-Körper-Stoß

??[ImpulsPHET](https://phet.colorado.edu/sims/html/collision-lab/latest/collision-lab_all.html?locale=de)


{{1}}
************
__Problem:__ Energieerhaltung

![Impuls_Problem_Energieerhaltung](https://diversewolken.ddns.net/nextcloud/index.php/s/nRgSSi4AeppbBob/download)

************


## 1.15 Erhaltungsgröße Impuls

> Der __Impuls__ $p$ eines Körpers beschreibt umgangssprachlich dessen _Wucht_ oder auch den _Schwung_. 
>
> Der Impuls ist __definiert__ als das Produkt aus Masse und Geschwindigkeit.

{{1}}
**********
> Formel:
>
> $$ \boxed{p = m \cdot v}$$
>
> Einheit:
>
> $$ \Big[\dfrac{kg \cdot m}{s} \Big] $$
>
> $\hspace{1cm} m$ .. Masse des Körpers in [$kg$]
>
> $\hspace{1cm} v$ .. Geschwindigkeit des Körpers in [$\frac{m}{s}$]
**********

{{2}}
**********
__Impulserhaltung:__

> In einem abgeschlossenen System ist der Impuls eine Erhaltungsgröße. <br> D.h. die Summe aller Einzelimpulse ist zu allen Zeiten konstant.
>
> $$ p_1 + p_2 + .. + p_N = \text{const}$$
**********

## Beispielaufgabe

Ein Körper (1) der Masse $m_1=1\,kg$ bewegt sich mit einer 
Geschwindigkeit von $v_1=1\,\frac{m}{s}$ und stößt elastisch und zentral gegen einen Körper (2) mit einer Masse $m_2=2\,kg$. <br> Bestimme die Geschwindigkeiten beider Körper nach dem Stoß.

{{1}}
***************
geg.: 

$\hspace{1cm}$ $m_1=1\,kg$

$\hspace{1cm}$ $m_2=2\,kg$

$\hspace{1cm}$ $v_1=1\,\frac{m}{s}$

$\hspace{1cm}$ $v_2=0\,\frac{m}{s}$

ges.: 

{2}{$\hspace{1cm}$ $v_1'$, $v_2'$ <br> $\hspace{1cm}$_Hinweis: alle Größen nach dem Stoß werden mit einem ' gekennzeichnet_)}

***************

{{3}}
***************
Lsg.: 

$\hspace{0.5cm}$ _1. Energieerhaltung_

$\hspace{1cm}$ $E_{kin1} + E_{kin2} = E'_{kin1} + E'_{kin2} $
***************

{{4}}
***************
$\hspace{1cm}$ $E_{kin1} + 0 = E'_{kin1} + E'_{kin2} $
**************

{{5}}
***************
$\hspace{1cm}$ $\dfrac{1}{2} \cdot m_1 \cdot v_1^2 = \dfrac{1}{2} \cdot m_1 \cdot v_1'^2 + \dfrac{1}{2} \cdot m_2 \cdot v_2'^2 $

$\hspace{0.5cm}$ _Problem:_ {6}{ _1 Gleichung, zwei unbekannte Größen_ }
**************

{{6}}
***************
$\hspace{0.5cm}$ _Idee: Impulserhaltung_

$\hspace{1cm}$ $p_{1} + p_{2} = p'_{1} + p'_{2} $
***************

{{7}}
***************
$\hspace{1cm}$ $m_1 \cdot v_1 + m_2 \cdot v_2 = m_1 \cdot v'_1 + m_2 \cdot v'_2 $
***************

{{8}}
***************
$\hspace{1cm}$ $m_1 \cdot v_1 + 0 = m_1 \cdot v'_1 + m_2 \cdot v'_2 $
***************

{{9}}
***************
$\hspace{0.5cm}$ _Gleichungssystem: 2 Gleichungen, zwei Unbekannte $\checkmark$_
***************

{{10}}
***************
$\hspace{1cm}$ (I)$\hspace{0.5cm}$ $m_1 \cdot v_1^2 =  m_1 \cdot v_1'^2 + m_2 \cdot v_2'^2 $

$\hspace{1cm}$ (II)$\hspace{0.5cm}$ $m_1 \cdot v_1 = m_1 \cdot v'_1 + m_2 \cdot v'_2 $
***************

{{11}}
***************
$\hspace{0.5cm}$ _Lösen mit CAS oder Umstellen_
***************

{{12}}
***************
$\hspace{0.5cm}$ _Lösungen:_

<iframe scrolling="no" title="Loesung_Bungee_Fehlerrechnung" src="https://www.geogebra.org/material/iframe/id/q9zzyrf2/width/800/height/400/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/true/ctl/false" width="100%" height="400px" style="border:0px;"> </iframe>
***************

{{13}}
***************
$\hspace{0.5cm}$ _Interpretation der Lösung:_


$\hspace{1cm}$ 1. Lösung: $v'_1= 1\frac{m}{s}$ und $v'_2= 0\frac{m}{s}$

$\hspace{1cm}$ => {14}{Körper 1 verfehlt Körper 2 und fliegt vorbei (Triviallösung)}
***************

{{15}}
***************
$\hspace{1cm}$ 2. Lösung: $v'_1= - \frac{1}{3}\frac{m}{s}$ und $v'_2= \frac{2}{3}\frac{m}{s}$
***************

{{15}}
***************
$\hspace{0.5cm}$ Probe: Energie

$\hspace{1cm}$ (I) $\hspace{0.5cm}$ $1\,kg \cdot (1\frac{m}{s})^2 = 1\,kg \cdot (-\frac{1}{3}\frac{m}{s})^2 + 2\,kg \cdot (\frac{2}{3}\frac{m}{s})^2$

$\hspace{1cm}$ (I) $\hspace{0.5cm}$ $1\,J = \frac{1}{9}\,J + \frac{8}{9}\,J$

$\hspace{1cm}$ (I) $\hspace{0.5cm}$ $\checkmark$
***************

{{16}}
***************
$\hspace{0.5cm}$ Probe: Impuls

$\hspace{1cm}$ (II) $\hspace{0.5cm}$ $1\,kg \cdot 1\frac{m}{s} = 1\,kg \cdot (-\frac{1}{3}\frac{m}{s}) + 2\,kg \cdot \frac{2}{3}\frac{m}{s}$

$\hspace{1cm}$ (II) $\hspace{0.5cm}$ $1\,\frac{kg\cdot m}{s} = -\frac{1}{3}\,\frac{kg\cdot m}{s} + \frac{4}{3}\,\frac{kg\cdot m}{s}$

$\hspace{1cm}$ (II) $\hspace{0.5cm}$ $\checkmark$
***************

## Gleichungssystem lösen mit dem ClassPad fx-CP400

!?[GleichungssystemLösenMitClassPad](https://www.youtube.com/watch?v=HkCrY7X-g6Q)

## Beispielaufgabe 2

Ein Körper (1) der Masse $m_1=1\,kg$ bewegt sich mit einer 
Geschwindigkeit von $v_1=2\,\frac{m}{s}$ und stößt elastisch und zentral gegen einen Körper (2) mit einer Masse $m_2=3\,kg$. <br> Bestimme die Geschwindigkeiten beider Körper nach dem Stoß mit Hilfe des CAS.

{{1}}
************
_Lösungen:_

<iframe scrolling="no" title="Loesung_Bungee_Fehlerrechnung" src="https://www.geogebra.org/material/iframe/id/ypvnghec/width/800/height/400/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/true/ctl/false" width="100%" height="400px" style="border:0px;"> </iframe>
***************

## Aufgaben - Impuls

Metzler S. 41, 1,3, 6

<details>

<summary>Lösung 1</summary>

![Lsg_Metzler41_1](https://diversewolken.ddns.net/nextcloud/index.php/s/fb7GokCF2CMept6/download)

</details>

<details>

<summary>Lösung 3</summary>

![Lsg_Metzler41_3](https://diversewolken.ddns.net/nextcloud/index.php/s/6WBJFiy9gL3N7Pz/download)

</details>

<details>

<summary>Lösung 6</summary>

![Lsg_Metzler41_6](https://diversewolken.ddns.net/nextcloud/index.php/s/PHPbTztDsFqLCFA/download)

</details>

## 1.16 Arten von Stößen

![Tafelbild_StossArten](https://diversewolken.ddns.net/nextcloud/index.php/s/GRmxkRPnqMe2qya/download)

## 1.17 Kraftstoß und Impulsänderung

Um den Impuls eines Körpers zu ändern, gibt es verschiedene Möglichkeiten:

{{1}}
**************
| | | |
| Änderung der Masse des Körpers | Änderung des Betrags der Geschwindigkeit | Änderung der Richtung der Geschwindigkeit |
**************

{{2}}
**************
> Der Kraftstoß kennzeichnet die Wirkung einer Kraft über eine bestimmte Zeit auf einen Körper. 
> Dies resultiert in einer Änderung des Impulses:
>
> $$ \boxed{\Delta p = F \cdot \Delta t}$$
>
> mit:
>
> $\hspace{1cm}$ $\Delta p$ ... Impulsänderung
>
> $\hspace{1cm}$ $F$ ... wirkende Kraft
>
> $\hspace{1cm}$ $\Delta t$ ... Zeitdauer der Wirkung (Zeitspanne)
>
> Einheit: $[ N \cdot s ]$
**************


{{3}}
************
_Hinweis: Der griechische Buchstabe Delta $\Delta$ kennzeichnet in der Physik die ***Änderung*** einer physikalischen Größe._

_Hier ist $\Delta p$ die Impulsänderung während der Zeitspanne $\Delta t$._
************

## Beispiel Impulsänderung - LEIFI Physik

siehe [Kraftstoß bei LEIF-Physik](https://www.leifiphysik.de/mechanik/impulserhaltung-und-stoesse/grundwissen/kraftstoss)

## Übungsaufgaben - Impuls und Impulserhaltung

Duden S. 170, Aufgaben 74, 77, 79

<details>

<summary>Lösung 74</summary>

![Lsg_Duden170_74](https://diversewolken.ddns.net/nextcloud/index.php/s/YY6XkGAzmqXkNKP/download)

</details>

<details>

<summary>Lösung 77</summary>

![Lsg_Duden170_77](https://diversewolken.ddns.net/nextcloud/index.php/s/so8Ya4d9aKkk7Lj/download)


![Lsg_Duden170_77c](https://diversewolken.ddns.net/nextcloud/index.php/s/AZ4zndkY2Y3a6yL/download)

</details>

<details>

<summary>Lösung 79</summary>

![Lsg_Duden170_79](https://diversewolken.ddns.net/nextcloud/index.php/s/tWfBagZiqY3rn7Y/download)

</details>

# LB2

<p class="newspaper">

![KräfteDreieck](https://diversewolken.ddns.net/nextcloud/index.php/s/B9e6ZLDf9EGF3Nc/download)

<p class="cb">

![Brückenarten](https://diversewolken.ddns.net/nextcloud/index.php/s/E8XLkanmHRE2c6Y/download)

Quelle: [Mitterhofer](https://andreasmitterhofer.de/2018/12/01/brueckenarten/)

</p>

</p>

{{1}}
*******************
![SkizzeKraefteMoti](https://diversewolken.ddns.net/nextcloud/index.php/s/8sE3RZpxws3YBo4/download)
*******************

## 2.1 Beschreibung Kraft

Kräfte erkennt man an ihrer Wirkung. Die Wirkung von Kräften kann sein:

{{1}}
**************************
1. Ein Körper ändert seine Bewegungsform (d.h. Geschwindigkeit oder Bewegungsrichtung).

2. Ein Körper verformt sich.

3. Beides gleichzeitig.
**************************

{{2}}
**************************

<p class="newspaper">



__Darstellung:__

Kräfte werden grafisch als Pfeile dargestellt. Dabei beschreibt 

1. die __Länge__ des Pfeils den Wert (Betrag, z.B. 3N)

2. der __Ansatzpunkt__ des Pfeils den Wirkort (_meist Schwerpunkt des Körpers_)

3. die __Richtung__ des Pfeils die Wirkrichtung

der Kraft

<p class="cb">

__Beispiel:__

![HorizontaleEbene](https://diversewolken.ddns.net/nextcloud/index.php/s/gtxDSYYLcJPSFQW/download)

</p>

</p>

**************************

{{3}}
**************************
> __Formelzeichen:__ $\vec{F}$ $\hspace{1cm}$ __Einheit:__ 1N (Newton)
>
> *Hinweis: __Vektorgrößen__, wie die Kraft, werden in Zukunft mit einem Pfeil darüber gekennzeichnet, wenn die Wirkrichtung entscheident ist.*
**************************

## 2.2 Superposition von Kräften

> Unter der Superposition von Kräften versteht man das gleichzeitige Wirken mehrerer Kräfte. Durch Addition der Kraftpfeile kann die resultierende __Gesamtkraft $F_{ges}$__ ermittelt werden.

{{1}}
**********
__Beispiel 1:__  Ruhender Körper auf horizontaler Ebene(siehe 1.9.3)

![GewichtskraftGegenkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/WDBCJmyZ7Q4jkrK/download)
_Gewichtskraft $F_g$ und Gegenkraft $F_U$ haben den gleichen Wert wirken aber in entgegen gesetzte Richtung und heben sich gegenseitig auf._ 

__=> Resultierende Kraft $F_{ges}$ ist Null, der Körper ruht__
**********

<br>
<br>

{{2}}
***********
__Beispiel 2:__ Flugzeug mit Seitenwind

{2-3}{![Kräfte_Senkrecht1](https://diversewolken.ddns.net/nextcloud/index.php/s/snYyLGyD4wKW7rF/download)} {3}{![Kräfte_Senkrecht2](https://diversewolken.ddns.net/nextcloud/index.php/s/6smmTrbPsk834Js/download)} Schubkraft $F_S$ und Windkraft $F_W$ wirken senkrecht zueinander.

__=> Gesamtkraft $F_{ges}$ kann geometrisch emittelt werden durch Addition der Pfeile.__

***********

{{4}}
**********
__Beispiel 3:__ Kräfteaddition allgemein

{4-5}{![Kräfte_Allg_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9f2c7SWt66wH2R7/download)}{5}{![Kräfte_Allg_2](https://diversewolken.ddns.net/nextcloud/index.php/s/ZwdPTzyYjoj2jaL/download)} _Wirken zwei Kräfte in beliebigen Richtungen auf denselben Körper, so addiere die Kraftpfeile durch $\textbf{Parallelverschieben}$ des Ursprungs eines Pfeils in die Spitze des anderen Pfeils. Die Gesamtkraft entsprich der Diagonale des entstandenen Parallelogramms._

__=> Gesamtkraft $F_{ges}$ kann mit Richtung und Wert geometrisch bestimmt werden.__
**********

### 2.2.1 Aufgaben zum Thema Kräfte

![Aufgabe1](https://diversewolken.ddns.net/nextcloud/index.php/s/eEqaeWXtm6GDc9i/download)

<details>

<summary>Lösung 1 _(Hinweise für 1b findest du in 2.3)_ </summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/WBPp9mREz4zzdqS/download)

</details>



## 2.3 Kraftzerlegung (_am Beispiel der schiefen Ebene_)

> __Hinweis Kräfte-Zerlegung__: Eine Gesamtkraft kann man gedanklich in Teilkräfte zerlegen, deren Addition wieder die Gesamtkraft ergibt. <br> Im Beispiel der schiefen Ebene zerlegt man die Gewichtskraft ($F_g$) in eine Teilkraft senkrecht zur Ebene ($F_N$) und eine Teilkraft parallel zur Ebene ($F_H$)

<br>

![Aufgabe_Schiefe_Ebene](https://diversewolken.ddns.net/nextcloud/index.php/s/fSJdL6YnB7RMQ4s/download) An einer schiefen Ebene mit dem Neigungswinkel $\alpha$ lässt sich die Gewichtskraft $F_g$ in eine Normalkraft $F_N$ (senkrecht zur Ebene) und eine Hangabtriebskraft $F_H$ (parallel zur Ebene) zerlegen.

_Aufgabe 2.3: Zeichne diese Kraftzerlegung in deinen Hefter. Konstruiere anschließend folgendes Beispiel: Auf einer schiefen Ebene (30°) ruht ein Körper mit der Gewichtkraft 3000 N._ 

1. _Ermittle grafisch oder durch Berechnung die Normalkraft $F_N$_ und die Hangabtriebskraft $F_H$.


<details>

<summary>Lösung 1</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/wtm7y9772WdKNaS/download)

</details>

<br>

$ \hspace{0.5cm} $__LB Metzker S. 49/3__

<details>

<summary>Lösung Metzler 47/3</summary>

Gewichtskraft $F_g = m \cdot g = 589 N$

Hangabtriebskraft $F_H = m \cdot g \cdot \sin\alpha = 294 N$

Normalkraft $F_N = m \cdot g \cdot \cos\alpha = 510 N$ 

Der Normalkraft hält eine Gegenkraft der Unterlage $F_U = F_N$ entgegen. Der Hangabtriebskraft $F_H$ wirkt die in der Aufgabe genannte Haltekraft $F' = F_H$ entgegen.

</details>

<br>

2. Konstruiere das Beispiel der Metzler-Aufgabe (47/3) mit dem Unterschied, dass die haltende Kraft $F'$ horizontal wirkt. Ermittle den Wert dieser haltenden Kraft $F'$ so, dass der Körper ruht.

<details>

<summary>Lösung 2</summary>

![Lsg_2.3.2](https://diversewolken.ddns.net/nextcloud/index.php/s/R35smRB9m8FdADi/download)

Berechnung: $F' = F_g \cdot \tan\alpha = 340 N$

</details>


## 2.4 Newtonsche Gesetze

{{1}}
**************
1. _Trägheitsgesetz:_ Ein kräftefreier Körper bleibt in Ruhe oder bewegt sich geradlinig mit konstanter Geschwindigkeit. <br> 
$\hspace{1cm}$ __Beispiel:__ {2}{![VoyagerSone](https://heise.cloudimg.io/width/1220/q70.png-lossy-70.webp-lossy-70.foil1/_www-heise-de_/imgs/18/3/5/4/6/9/3/7/Voyager-illustration-with-stars-16.jpg-e02f3b734d477d20.jpeg) Sonde ohne Antrieb im Weltall}
**************

<br>
<br>

{{3}}
**************************
2. _Grundgesetz der Mechanik_: Kraft gleich Masse mal Beschleunigung

>    $$ F = m \cdot a $$
**************************

{{4}}
********
$\hspace{1cm}$ __Beispiel:__ [Freier Fall](https://youtu.be/-Fhc51_JbcQ) 
 eines Körpers auf der Erde: $$\boxed{F_g = m \cdot g} $$ <br> 
$\hspace{1cm}$mit Gewichtskraft $F_g$ und Erdbeschleunigung/Ortsfakor $g=9,81\frac{m}{s^2}$.
********



{{5}}
**************************
3. Wechselwirkungsgesetz: Kraft gleich Gegenkraft

> Eine Kraft von Körper A auf Körper B geht immer mit einer gleich großen, aber entgegen gerichteten Kraft von Körper B auf Körper A einher
**************************
{{6}}
********
$\hspace{1cm}$ __Beispiel:__ ![Gegenkraft](https://av.ph.nat.tum.de/Experiment/1000/Grafik/b1105.gif) 

********


## 2.5 Einführung in das Thema Reibung

### 2.5.1 Definition Reibung

Reibung ist eine Kraft, die der Bewegung zweier Oberflächen entgegenwirkt, die miteinander in Kontakt stehen. Sie tritt auf, wenn zwei Oberflächen aneinander __haften, gleiten oder rollen__.

Reibung kann im Alltag nützlich oder hinderlich sein.

{{1}}
*****
__Es gibt drei Hauptarten der Reibung (von zwei Körpern):__

1. **Haftreibung** ($F_{Haft}$)
2. **Gleitreibung** ($F_{Gleit}$)
3. **Rollreibung** ($F_{Roll}$)

<br>

4. [ **Luftreibung** ($F_{Luft}$) ]
*****

{{2}}
*****
| | | | |
| ![Reibung1](https://diversewolken.ddns.net/nextcloud/index.php/s/Mck6oNwSa46L2Qx/download) | ![Reibung2](https://diversewolken.ddns.net/nextcloud/index.php/s/asZf57L4XxwawnT/download) | ![Reibung3](https://diversewolken.ddns.net/nextcloud/index.php/s/SG9GxsxxpbT6m8Z/download) | ![Reibung4](https://diversewolken.ddns.net/nextcloud/index.php/s/5kJ3R7npPtCGb5p/download) |
| {3}{$F_{Gleit}$} | {4}{$F_{Roll}$} | {5}{$F_{Gleit}$} | {6}{$F_{Haft}$} |

{6}{_Aufgabe: Zuordnung von Reibungsarten_}
*****

{{7}}
*********
---

__Haftreibung__

Haftreibung tritt auf, wenn zwei Oberflächen aufeinander haften, ohne sich zu bewegen. Diese Art der Reibung muss überwunden werden, um ein Objekt in Bewegung zu setzen.

- **Beispiel**: Ein Buch liegt auf einem Tisch. Es bleibt in Ruhe, bis eine ausreichend große Kraft aufgebracht wird, um es in Bewegung zu versetzen.
*********


{{8}}
*******
---


__Gleitreibung__

Gleitreibung tritt auf, wenn zwei Oberflächen aneinander entlang gleiten. Diese Art der Reibung wirkt der Bewegung entgegen und ist in der Regel geringer als die Haftreibung.

- **Beispiel**: Ein Schlitten gleitet über Schnee. Die Reibungskraft, die der Bewegung entgegenwirkt, ist die Gleitreibung.

*******



{{9}}
********
---

__Rollreibung__

Rollreibung tritt auf, wenn ein Objekt über eine Oberfläche rollt. Sie ist in der Regel geringer als die Gleitreibung, da der Kontaktpunkt sich ständig ändert.

- **Beispiel**: Ein Rad rollt über eine Straße. Die Reibungskraft, die der Rollbewegung entgegenwirkt, ist die Rollreibung.

********



### Übung: Zuordnung von Reibungsarten

__Erwünschte und unerwünschte Reibung:__
<iframe src="https://learningapps.org/watch?app=21913985" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

__Erkenne Reibungsarten:__
<iframe src="https://learningapps.org/watch?app=374843" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>


### Video: Reibung

??[MussteWissenReibung](https://www.zdf.de/funk/musstewissen-1066/funk-reibung---physik-musstewissen-100.html)

Quelle: ZDF.de

### 2.5.2 Die Reibungszahl $\mu$ - Berechnung der Reibungskraft

Die Reibungszahl, auch Reibungskoeffizient genannt, ist eine dimensionslose Größe, die angibt, wie stark die Reibung zwischen zwei Oberflächen ist. Sie hängt von den Materialien der Oberflächen und ihrer Beschaffenheit ab.

{{1}}
********

Auf einer horizontalen Unterlage (waagerecht), gilt für die Berechnung der Reibung:

<p class="newspaper">

$$
\boxed{F_R = \mu \cdot F_g}
$$

<p class="cb">

![Horizontal](https://physikunterricht-online.de/wp-content/uploads/2022/03/Reibung.png)

</p>

</p>

----

********

{{2}}
********
Auf einer schiefen Ebene (Neigungswinkel $\alpha$) gilt für die Reibung:

<p class="newspaper">

$$
\boxed{F_R = \mu \cdot F_N = \mu \cdot F_g \cdot cos\alpha}
$$

<p class="cb">

![HSchiefeEbene](https://technikermathe.de/wp-content/uploads/2020/03/tk-statik-schiefe-ebene-2-768x432.jpg)

</p>

</p>

---

********


{{3}}
********
Dabei ist:

- $F_R$ die Reibungskraft,
- $F_g$ Gewichtskraft (_Hinweis: $\boxed{F_g = m \cdot g}$_ )
- $F_N$ die Normalkraft, Kraft die senkrecht auf die Kontaktfläche wirkt 
********

{{4}}
********
- $\mu$ der Reibungskoeffizient (Haft-, Gleit- oder Rollreibung)

  - **Haftreibungskoeffizient** ($\mu_{Haft}$)

  - **Gleitreibungskoeffizient** ($\mu_{Gleit}$)

  - **Rollreibungskoeffizient** ($\mu_{Roll}$)

********

---

{{4}}
********
>> __Merke:__ Bei identischen Oberflächen ist der Rollreibungskoeffizient  ($\mu_{Roll}$) deutlich am kleinsten. 
>>
>> Haftreibungskoeffizient($\mu_{Haft}$) ist immer größer, als Gleitreibungskoeffizient ($\mu_{Gleit}$)
>>
>> $$\mu_{Roll} \ll \mu_{Gleit} < \mu_{Haft}$$
>>
>> _Hinweis: $\ll$ bedeutet "sehr viel kleiner als"_

_Aufgabe: siehe 2.3.4_

********

### 2.5.3 Zusammenfassung

Reibung ist eine fundamentale Kraft in der Physik, die der Bewegung zwischen zwei Oberflächen entgegenwirkt. Sie kann in Haft-, Gleit- und Rollreibung unterteilt werden. Die Berechnung der Reibungskraft erfolgt durch die Multiplikation des Reibungskoeffizienten mit der Normalkraft.

### 2.5.4 Qualitative Übung zur Reibung (ohne Berechnungen)

Diskutiere mit einem Partner. Stellt euch Wechselseitig die Fragen und überprüft die Antworten.

__Empfehlung: Aufgaben 113-117__

??[PittysPhysik](https://physikaufgaben.de/aufgaben_zeige_an.php?thid=1&tab=6&auswahl_t1=13&auswahl_n1=4)

### 2.5.5 Quantitative Übung zur Reibung (mit Berechnungen)

_Quantitative Aufgaben zur Reibung auf horizontalen Ebene. Bitte anklicken und allein oder in Gruppenarbeit berechnen und Lösung vergleichen._

[Leifi-Physik-Aufgabe-Reibung-1](https://www.leifiphysik.de/mechanik/reibung-und-fortbewegung/aufgabe/wohnanhaenger)

[Leifi-Physik-Aufgabe-Reibung-2](https://www.leifiphysik.de/mechanik/reibung-und-fortbewegung/aufgabe/die-verrueckte-kiste)

### Fortsetzung Aufgabe 2.3 (_jetzt mit Reibung_)

![Aufgabe_Schiefe_Ebene](https://diversewolken.ddns.net/nextcloud/index.php/s/fSJdL6YnB7RMQ4s/download) An einer schiefen Ebene mit dem Neigungswinkel $\alpha$ lässt sich die Gewichtskraft $F_g$ in eine Normalkraft $F_N$ (senkrecht zur Ebene) und eine Hangabtriebskraft $F_H$ (parallel zur Ebene) zerlegen.


3. _Die Unterlage und Körper haben eine Haftreibungszahl $\mu_{Haft} = 0,4$ (s. 2.3.2). Ermittle die Haftreibungskraft auf der Unterlage._

4. _Ist die Hangabtriebskraft größer als die Reibungskraft, so beginnt der Körper zu rutschen. Überprüfe, ob sich der Körper bewegt._

5. _Der Neigungswinkel $\alpha$ wird nun so verändert, sodass der Körper gerade noch ruht. Bestimme diesen Grenzwinkel $\alpha_G$, bei welchem der Körper gerade noch nicht zu rutschen beginnt._


<details>

<summary>Lösung 3</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/AD8EM2imFcfbFtS/download)

</details>

<details>

<summary>Lösung 4</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/SaJ5yqyRBqLDToJ/download)

</details>

<details>

<summary>Lösung 5</summary>

Für den Grenzwinkel $\alpha_G$ gilt ( Haftreibungskraft gleich Hangabtriebskraft):
$$ F_{Haft} = F_H $$ 

Für die Haftreibungskraft gilt die Formel:
$$ F_{Haft} = F_G \cdot \cos(\alpha_G) \cdot \mu_{Haft} $$

Für die Hangabtriebskraft gilt die Formel:
$$ F_H = F_G \cdot \sin(\alpha_G)$$

Setzt man $F_{Haft} = F_H $, so ergibt sich:
$$ F_G \cdot \cos(\alpha_G) \cdot \mu_{Haft} = F_G \cdot \sin(\alpha_G) $$

also

$$ \mu_{Haft} = \dfrac{\sin(\alpha_G)}{\cos(\alpha_G)} $$

Mit der Trigonometrie $\tan(\alpha_G) = \frac{\sin(\alpha_G)}{\cos(\alpha_G)}$ ergibt sich:

$$ \alpha_G = tan^{-1}(\mu_{Haft}) $$
$$ \underline{\alpha_G = 21,8^\circ}$$ 

Bei einem Winkel größer als 21.8° beginnt der Körper zu rutschen.

</details>

### 2.5.6 Bestimmung des Haftreibungskoeffizienten

__Aufgabe:__ Bestimmen Sie die Haftreibungszahl $\mu_{Haft}$ zwischen einem Holzklotz und einer Plastikschiene mit zwei Messmethoden. Fertigen Sie ein Kurzprotokoll an.

1. Teilen Sie dazu das Blatt in zwei Teile.

2. Notieren Sie jeweils die Versuchsmethode und zeichnen Sie eine Skizze. 

3. Notieren Sie Ihre Messwerte. Geben Sie zu beiden Methoden ein Ergebnis der Haftreibungszahl $\mu_{Haft}$ an.

4. Vergleichen Sie beide Ergebnisse. Nehmen Sie Bezug auf die Ungenauigkeit der jeweiligen Messung (Fehlerbetrachtung).

<p class="newspaper">

__Versuch 1__

_Messmethode 1:_ Nutzen Sie einen Federkraftmesser und bestimmen Sie für 3 zugeladene Massestücke die Gewichtskraft (50g, 100g, 150g), sowie die Haftreibungskraft des Holzklotzes mit der Plastikschiene. Ermitteln Sie daraus den Haftreibungskoeffizienten $\mu_{Haft}$.

<p class ="cb">

__Versuch 2__

_Messmethode 2:_ Nutzen Sie eine schiefe Ebene  und bestimmen Sie die Haftreibungszahl mit Hilfe des Grenzwinkels $\alpha_G$ (siehe Fortsetzung Aufgabe 2.3/5). Nutzen Sie dieselben zugeladenen Massestücke, wie in Versuch 1.

</p>

</p>

__Ergebnisse:__

??[mu-haft](https://diversewolken.ddns.net:8080/survey/results/yo9q45a9)


### 2.5.7 Übungsaufgaben

Metzler S. 81/12



## 2.6 Einheitenbetrachtungen

Bisher haben wir in Formeln folgendes Vorgehen genutzt:

- rechne alle Größen in Standard-Einheiten um, dann ergibt die Formel jeweils auch die Standard-Einheit

__Jetzt: Einheitenbetrachtungen__

Allgemein: Einheiten können innerhalb einer Formel oder auch dahinter in eckigen Klammern analysiert/diskutiert werden.

Grundlagen:

> $\hspace{1cm}$ Kraft: $\Big[ N = \dfrac{kg \cdot m}{s^2} \Big]$
>
> $\hspace{1cm}$ Energie: $\Big[ J = N\cdot m = \dfrac{kg \cdot m}{s^2}\cdot m = \dfrac{kg \cdot m^2}{s^2} \Big]$
__Beispiel:__

> geg.: 
>
> $\hspace{1cm}$ $v = 100 \frac{km}{h}$
>
> $\hspace{1cm}$ $m = 1,5 t = 1500 kg$
>
> ges.: 
>
> $\hspace{1cm}$ $E_{kin}$

> Lsg.: 
>
> $\hspace{1cm}$  $E_{kin} = \dfrac{1}{2} \cdot m \cdot v^2 $
>
> $\hspace{1cm}$  $E_{kin} = \dfrac{1}{2} \cdot 1500 \cdot (27,78 )^2 $ $ \Big[ \dfrac{kg \cdot m^2 }{s^2} \Big] $
>
> $\hspace{1cm}$  $E_{kin} \approx 578.796 \Big[ \dfrac{kg \cdot m }{s^2} \cdot m = Nm = J \Big] $

### 2.6.1 Übungen Einheitenbetrachtung

Zeige für folgende Formeln, dass sich die geforderte Standard-Einheit ergibt.

|#  | Formel | Standard-Einheit |
| -- | ---------------- | --------------- |
| 1 | $v = \sqrt{\dfrac{2\cdot E_{kin}}{m}}$ | $\Big[\dfrac{m}{s}\Big]$ |
| 2 | $h = \dfrac{E_{pot}}{g \cdot h}$ | $\Big[m\Big]$ |
| 3 | $\Delta p = F \cdot \Delta t $ | $\Big[\dfrac{kg \cdot m}{s}\Big]$ |
| 4 | $W_{sp} = \frac{1}{2} \cdot D \cdot s^2 $ | $\Big[J\Big]$ |
| 5 | $g = \dfrac{F_g}{m}$ | $\Big[ \dfrac{m}{s^2} \Big]$ |
| 6 | $v = \dfrac{m_1 + m_2}{m_2}\sqrt{2\cdot g\cdot h}$ | $\Big[\dfrac{m}{s}\Big]$ | 


## 2.7 Luftwiderstandskraft

> Die Luftwiderstandskraft hängt von der Querschnittsfläche des Körpers, der Dichte der Luft, dem Quadrat der Geschwindigkeit und dem $c_w$-Wert des Körpers ab: 
>
> $$F_{Luft} = \frac{1}{2} \cdot c_w \cdot A \cdot \rho_{Luft} \cdot v^2$$
>
> mit:
>
> $\hspace{1cm}$ $F_{Luft}$ ... Luftwiderstandskraft $\Big[ N \Big]$
>
> $\hspace{1cm}$ $c_w$ ... Luftwiderstandswert [einheitenlos]
>
> $\hspace{1cm}$ $A$ ... (projezierte) Querschnittsfläche $\Big[ m^2 \Big]$ 
>
> $\hspace{1cm}$ $\rho_{Luft}$ ... Dichte der Luft $\Big[ \dfrac{kg}{m^3} \Big]$
>
> $\hspace{1cm}$ $v$ ... Bewegungsgeschwindigkeit $\Big[ \dfrac{m}{s} \Big]$


{{1}}
***********

__Einheitenbetrachtung__:

{{2}}
***********
![Tb_Einheiten_cw](https://diversewolken.ddns.net/nextcloud/index.php/s/x8HZPgoPBq9G4cG/download)
***********


__Schülerexperiment $c_w$-Bestimmung Papierkegel:__

{{3}}
***********

<p class="newspaper">

Bestimme den $c_w$_Wert eines Papierkegels.

Bestimme dazu <br>

- die (projezierte) Fläche $A$ des Kegels

<details>

<summary>Hinweis $A$</summary>

> _Bestimme den Radius oder Durchmesser des Außenkegels und ermittle den Flächeninhalt A des Kreises (in m²)_

</details>

- die Luftwiderstandskraft $F_{Luft}$ bei gleichförmiger Bewegung im freien Fall

<details>

<summary>Hinweis $F_{Luft}$</summary>

> _Bei gleichförmiger Bewegung im freien Fall ist die Summe aller wirkenden Kräfte gleich Null (1. Newton'sches Axiom). Da außer der Luftwiderstandskraft nur die Gewichtskraft wirkt, müssen diese beiden gleich groß sein. Ermittle für die Bestimmung von $F_{Luft}$ die Gewichtskraft und nutze $F_{Luft}=F_g$_

</details>

- die Bewegungsgeschwindigkeit $v$ im freien Fall

<details>

<summary>Hinweis $v$</summary>

> _Bei gleichförmiger Bewegung im freien Fall kann die Bewegungsgeschwindigkeit über die Gleichung $v=\frac{s}{t}$ ermittelt werden. Achte bei der Wahl der Strecke darauf, dass die gemessene Zeit so groß ist, dass die Reaktionsgeschwindigkeit (ca. 0.3s) nicht mehr als 10% beträgt._

</details>

- die Dichte der Luft $\rho_{Luft}$

<details>

<summary>Hinweis $\rho_{Luft}$ </summary>

> _Die aktuelle Luftdichte ist ein täglich wechselnder Wert und kann online ermittelt werden. Achte bei der Einheit auf die Standardeinheit $[\frac{kg}{m^3}]$_. Z.B. [hier](https://wind-data.ch/tools/luftdichte.php)

</details>

<p class="cb">

![PapierKegel](https://diversewolken.ddns.net/nextcloud/index.php/s/7Gi2pbyzdAyjD5J/download)

</p>

</p>
***********

***********

## Berechnung $c_w$-Wert Papierkegel

<p class="newspaper">

__Messwerte:__

> $\hspace{0.5cm}$ geg.:
>
> $\hspace{1cm}$ $\rho_{Luft}=$ <input type="number" default="0" min="0" max="10" size="5" id="rho"> $\dfrac{kg}{m^3}$ $\hspace{0.2cm}$[>LD<](https://wind-data.ch/tools/luftdichte.php)
>
> $\hspace{1cm}$ $d=$ <input type="number" default="0" id="d" min="0" max="10" size="5"> $m$
>
>$\hspace{1cm}$ $m = $ <input type="number" default="0" id="m" min="0" max="10" size="5"> $kg$
>
>$\hspace{1cm}$ $s=$ <input type="number" default="0" id="s" min="0" max="10" size="5"> $m$
>
>$\hspace{1cm}$ $t=$ <input type="number" default="1" id="t" min="0" max="10" size="5"> $s$
>
>$\hspace{0.5cm}$ ges.:
>
>$\hspace{1cm}$ $c_W$ 

<p class="cb">

__Papierkegel:__

![PapierKegel](https://diversewolken.ddns.net/nextcloud/index.php/s/7Gi2pbyzdAyjD5J/download)

</p>

</p>

{{1}}
*************
__Lösung:__

> $\hspace{0.5cm}$
>
>$\hspace{1cm}$ $A=\frac{\pi}{4}{d^2}$= <script input="button">
    let d = document.getElementById("d").value;
    let A = d*d/4*3.1415
    if ((isNaN(A))||(A==0)) "..."
    else A.toPrecision(3)
 </script> $m^2$
>
>$\hspace{1cm}$ $v=\dfrac{s}{t}=$ <script input="button">
    let t = document.getElementById("t").value;
    let s = document.getElementById("s").value;
    let v = s/t
    if (isNaN(v)) "..."
    else v.toPrecision(3)
 </script> $\dfrac{m}{s}$
>
>$\hspace{1cm}$ $F_g=F_{Luft}=m \cdot g=$ <script input="button">
    let g = 9.81;
    let m = document.getElementById("m").value;
    let F = m*g
    if (isNaN(F)||(F==0)) "..."
    else F.toPrecision(3)
 </script> $N$
>
>$\hspace{1cm}$ $c_w=\dfrac{2\cdot F_{Luft}}{A \cdot \rho_{Luft} \cdot v^2}$ = <script input="button">
    let d = document.getElementById("d").value;
    let g = 9.81
    let m = document.getElementById("m").value;
    let t = document.getElementById("t").value;
    let s = document.getElementById("s").value;
    let rho = document.getElementById("rho").value;
    let v = s/t;
    let A = 3.1415/4*d*d
    let result = 2*m*g/(A*rho*v*v)
    if (isNaN(result)) "..."
    else result.toPrecision(3)
 </script>
*************

{{2}}
*************
![cwWert](https://diversewolken.ddns.net/nextcloud/index.php/s/3B7ngZsZjz7fmJe/download "Auszug-Wikipedia")

- [Wikipedia cw-Wert](https://de.wikipedia.org/wiki/Str%C3%B6mungswiderstandskoeffizient)
*************

### 2.7.1 Übung zum $c_w$-Wert

> Der $c_w$ spielt bei Fahrzeugen eine entscheidene Rolle, denn er beschreibt die Luftwiderstandskraft, welche bei Fahrten aufgewendet werden muss und sagt somit etwas über den Benzin/Energieverbrauch des Fahrzeugs aus. 
>
> In Deutschland wird immer wieder über ein Tempolimit von $130\,\frac{km}{h}$ diskutiert. Untersuche für zwei Fahrzeuge (1. [VW T5 (Multivan)](https://de.wikipedia.org/wiki/VW_T5%2FT6) | 2. Selbst gewähltes Fahrzeug) die Luftwiederstandskraft bei einer gleichförmigen Fahrtgeschwindigkeit von $100\,\frac{km}{h}$, $130\,\frac{km}{h}$ und $180,\frac{km}{h}$. Fertige dazu eine Tabelle an.
>
> $c_w$_Werte und Querschnittsflächen gängiger Fahrzeugtypen können [hier](https://automobil-guru.de/cw-werte-tabelle-stirnflaeche/) ermittelt werden.
>
> Nutze für die Dichte der Luft eine mittleren Wert von $1,12\frac{kg}{m^3}$

| | || 
| | VW-T5 | 2. Fahrzeug |
| | $F_{Luft}$ in N | $F_{Luft}$ in N |
| $100\,\frac{km}{h}$ | 492 | |
| $130\,\frac{km}{h}$ | 831 | |
| $180\,\frac{km}{h}$ | 1593 | |

<details>

<summary>Beispiel T5 </summary>

> ![LsgLWT5](https://diversewolken.ddns.net/nextcloud/index.php/s/iirTC4DjQSrkb28/download)

</details>

## 2.8 Reibungsarbeit

> $W_R = F_R \cdot s$


> mit:
>
> $\hspace{0.5cm}$ $W_R$ .. Reibungsarbeit in $[J]$
>
> $\hspace{0.5cm}$ $F_R$ .. Reibungskraft in $[N]$
>
> $\hspace{0.5cm}$ $s$ .. zurückgelegter Weg in $[m]$

{{1}}
*************
>> Die durch Reibungsarbeit umgwandelte Energie wird in vielen Fällen in Innere Energie umgewandelt (z.B. Wärme).Man sagt sie wird dadurch _entwertet_ (d.h. schlecht nutzbar).
*************

### 2.8.1 Übung zum Verbauch von Kraftfahrzeugen

Für den Volkswagen Mulitvan T5 gibt der Hersteller bei konstanter Fahrt (90 km/h) einen Benzinverbrauch von 8,2 Liter je 100 km an. Die Fahrzeugmasse beträgt mit Zuladung 2,5 t. Der Rollreibungskoeffizient von Kraftfahrzeugreifen kann mit 0,02 angenommen werden.. 

#### Aufgabe 1

> __Aufgabe 1:__ Vergleichen Sie die im angegebenen Benzinvolumen enthaltene chemische Energie (Brennwert) mit der verrichteten Reibungsarbeit. Berücksichtigen Sie hierzu den Luftwiderstand und die Rollreibung. Diskutieren Sie mögliche Unterschiede und deren Ursache.

<details>

<summary> Hilfe 1: Reibungsarbeit </summary>

Die betrachteten Reibungskräfte sind Rollreibung und Luftreibung. Berechnen Sie die beiden Kräfte (Rollreibung siehe 2.5.2,Luftreibung siehe 2.7.1).

Vergleichswerte:

 - $F_{roll}= 490,5\,N$ 
  
 - $F_{Luft}= 444,3\,N$

</details>

<details>

<summary> Hilfe 2: Reibungsarbeit </summary>

Ermitteln Sie die verrichtete Arbeit auf der Strecke s = 100 km mit der Formel W = F * s.

</details>

<details>

<summary> Hilfe 3: Chemische Energie </summary>

Recherchieren Sie den Brennwert von einem Liter Benzin. Ermitteln Sie den gesamten Brennwert von 8,2 Litern.

</details>

<details>

<summary> Hilfe 4: Vergleich </summary>

Die enthaltene chemische Energie (ca. 260 MJ) ist deutlich höher als die verrichtete Reibungsarbeit (ca. 90 MJ). Überlegen Sie, ob die zugeführte chemische Energie vollständig in die Bewegung des Fahrzeugs umgewandelt wird.

</details>

#### Aufgabe 2

> __Aufgabe 2:__ Ermitteln Sie die Geschwindigkeit, bei welcher Rollreibungskraft und Luftreibungskraft den gleichen Wert haben.


<details>

<summary> Hilfe 1: Ansatz </summary>

Um die Geschwindigkeit zu berechnen, bei welcher Luftreibung und Rollreibung identisch sind, setzt man $F_{roll} = F_{Luft}$ und ermittelt als einzige unbekannte die Geschwindigkeit.

<div style="text-indent:5%">

<details>

<summary> Berechnung </summary>

> $\hspace{1cm}$ $F_{roll} = F_{Luft}$
>
> $\hspace{1cm}$ $m \cdot g \cdot \mu_{roll} = \frac{1}{2} \cdot c_w \cdot A \cdot \rho_{Luft} \cdot v^2$
>
> $\hspace{1cm}$ $v = \sqrt{\dfrac{2 \cdot m \cdot g}{c_w \cdot A \cdot \rho_{Luft}}} $
>
> $\hspace{1cm}$ $v = 26,27 \frac{m}{s}$

</details>

</div>

#### Aufgabe 3

> __Aufgabe 3:__ Das Tesla Modell 3 hat einen cw-Wert von 0,23 und eine projezierte Stirnfläche von 2,22 m². Die maximale, in der Batterie speicherbare Energie wird vom Hersteller mit 75 kWh angegeben. Die Masse des Fahrzeugs beträgt inlusive der Ladung/Personen 2 t. Die Rollreibungszahl zwischen Reifen und Fahrbahn beträgt 0,02. 
>
> Für den zu untersuchenden Fall soll das Fahrzeug einen Hang hinauf fahren. Die Steigung beträgt 12%. Der Tempomat wird dabei auf 90 km/h eingestellt, sodass sich Fahrzeug mit konstanter Geschwindigkeit bewegt. Die Länge des Hangs beträgt 12 km. Die Dichte der Luft kann mit 1,12 kg/m³ angenommen werden.
>
> 3. 1. Untersuchen sie die bei dieser Fahrt die zu verrichtende Arbeit. Vergleichen Sie dazu unterschiedliche Anteile der Arbeit miteinander.
>
> 3. 2. Ermitteln Sie, um wieviel Prozent die Batteriekapazität sinkt, wenn  diese Fahrt durchgeführt wird

<details>

<summary> Hilfe 1: Arten verrichteter Arbeit </summary>

Überlegen Sie, welche Arten von Arbeit hier verrichtet werden.

<div style="text-indent:5%">

<details>

<summary> Antwort </summary>

Hier wird Hubarbeit $W_H$, Rollreibungsarbeit $W_{Roll}$ und Luftreibungsarbeit $W_{Luft}$ verrichtet

</details>

</div>

</details>


<details>

<summary> Hilfe 2: Berechnung der verrichteten Arbeit </summary>

- Hubarbeit $W_H$ entspricht der potentiellen Energie, welche dem Körper am Ende der Fahrt zugeführt worden ist.

<div style="text-indent:5%">

<details>

<summary> Berechnung Rollreibungsarbeit $W_{roll}$ </summary>

> geg.: 
>
> $\hspace{1cm}$ $m = 2000 kg$
>
> $\hspace{1cm}$ $s = 12.000 m$
>
> $\hspace{1cm}$ Steigung 12%
>
> $\hspace{1cm}$ $\mu_{roll} = 0,02$
>
> ges.: 
>
> $\hspace{1cm}$ $W_{roll}$
>
> Lsg.:
>
> $\hspace{1cm}$ Winkel der Steigung wird berechnet mit $\alpha=\tan^{-1}(0,12)=6,8^\circ$
>
> $\hspace{1cm}$ $ W_{roll} = F_{roll} \cdot s = F_N \cdot \mu_{roll} \cdot s = m \cdot g \cdot \cos\alpha \cdot \mu_{roll} \cdot s$
>
> $\hspace{1cm}$ Die Rollreibung $F_{roll}$ muss mit der Normalkraft (s. 2.5.2) und dem Rollreibungskoeffizienten berechnet werden. 
>
> $\hspace{1cm}$ $W_{roll} = 467568 J \approx 4,68 MJ$

</details>

</div>

<div style="text-indent:5%">

<details>

<summary> Berechnung Hubarbeit $W_H$ </summary>

> geg.: 
>
> $\hspace{1cm}$ $m = 2000 kg$
>
> $\hspace{1cm}$ $s = 12.000 m$
>
> $\hspace{1cm}$ Steigung 12 %
>
> ges.: 
>
> $\hspace{1cm}$ $W_H = E_{pot}$
>
> Lsg.:
>
> $\hspace{1cm}$ $ W_H = E_{pot} = m \cdot g \cdot h$
>
> $\hspace{1cm}$ Die zu erreichende Höhe kann mit der Steigung ermittelt werden.
>
> $\hspace{1cm}$ $h = s \cdot 0,12 = 1440 m$
>
> $\hspace{1cm}$ => $ W_H = E_{pot} = 28.252.800 \approx 28,25 MJ$

</details>

</div>

<div style="text-indent:5%">

<details>

<summary> Berechnung Luftreibungsarbeit $W_{Luft}$ </summary>

> geg.: 
>
> $\hspace{1cm}$ $m = 2000 kg$
>
> $\hspace{1cm}$ $A = 2,22 m^2$
>
> $\hspace{1cm}$ $c_w = 0,23$
>
> $\hspace{1cm}$ $\rho_{Luft} = 1,12 \frac{kg}{m^3}$
>
> $\hspace{1cm}$ $v=25 \frac{m}{s} $
>
> ges.: 
>
> $\hspace{1cm}$ $W_{Luft}$
>
> Lsg.:
>
> $\hspace{1cm}$ $ W_{Luft} = F_{Luft} \cdot s = \frac{1}{2} \cdot c_w \cdot A \cdot \rho_{Luft} \cdot v^2 \cdot s$
>
> $\hspace{1cm}$ Da die Geschwindigkeit konstant ist, ist die Luftreibung den gesamten Weg über konstant.
>
> $\hspace{1cm}$ $W_{Luft} = 2144520 J \approx 2,14 MJ$

</details>

</div>

</details>

<details>

<summary> Hilfe 3: Vergleich </summary>

Die Hubarbeit macht hier den größten Teil ($28,25 MJ$) aus, gefolgt von der Rollreibungsarbeit ($4,68$) der Luftreibungsarbeit ($2,14 MJ$). Die insgesamt verrichtete Arbeit beträgt demnach ca. 35,07 MJ.

<div style="text-indent:5%">

<details>

<summary> Batterie-Kapazität </summary>

Die Batteriekapazität von 75 kWH entspricht entspricht $75kW \cdot 3600s = 270.000 kWs = 270 MJ$ (da eine Stunde 3600s entspricht). Es gilt: $ 1Ws = 1 J$. Somit enthält die Batterie 270 MJ. Die verrichtete Arbeit entspricht demnach $\frac{35,1 MJ}{270 MJ} \approx 13 \% $.

</details>

</div>

</details>

#### Aufgabe 4 (aus Abitur 2018)

1. Der Übungshang einer Skischule für Kinder hat die Neigung 9,5°. Ein Förderband bringt die Kinder bis zur Bergstation.

<!-- style="display: block; width:60%; margin:auto; display" -->
![Bild_Aufgabe_4](https://diversewolken.ddns.net/nextcloud/index.php/s/wbqrqwGx4KppPTw/download)

> 1. 1. Ein Kind (Gesamtmasse mit Ausrüstung 35 kg ) wird vom Förderband bergauf bewegt, dabei legt es den Weg 30 m zurück. Berechnen Sie die vom Förderband an dem Kind verrichtete Hubarbeit.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.1 </summary>

Nutzen Sie an der geneigten Ebene den Zusammenhang von mechanischer Arbeit (allgemein) und Hubarbeit.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.1 </summary>

![Aufgabe_4_L1.1](https://diversewolken.ddns.net/nextcloud/index.php/s/kQTopwPxoaQ3tW2/download)

</details>

</div>

> 1. 2. Das Kind steht am oberen Ende des Hanges. Der Skilehrer schiebt das Kind an. Dieses hat dadurch die Anfangsgeschwindigkeit 1,0 m/s und gleitet gleichmäßig beschleunigt den 30 m langen Hang geradlinig hinab. Nachdem das Kind das untere Ende des Hangs erreicht hat, gleitet es horizontal weiter. Die Reibungszahl ist konstant und beträgt 0,10.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.2 </summary>

![Aufgabe_4_L1.2](https://diversewolken.ddns.net/nextcloud/index.php/s/DNx4BR5zC656Lfa/download)

</details>

</div>

> 1. 2. 1. Weisen Sie nach, dass die maximale Geschwindigkeit des Kindes $v = 6,33 \frac{m}{s}$ beträgt.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.2.1 </summary>

Erstellen Sie eine Energiebilanz. Berücksichtigen Sie Anfangsgeschwindigkeit und Reibungsarbeit. Zeigen Sie, dass die Energiebilanz eine wahre Aussage ist.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.2.1 </summary>

![Aufgabe_4_L1.2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/gWD7HaLHNjmqy8C/download)

</details>

</div>

> 1. 2. 2. Eine Skilehrerin (Gesamtmasse mit Ausrüstung 65 kg ) steht auf dem horizontalen Auslauf und fängt das ankommende Kind auf. Beide gleiten gemeinsam 1,9 m weit und bleiben dann stehen. Die Reibungszahl ist konstant und beträgt für beide 0,10. <br> Ermitteln Sie die Länge des horizontalen Gleitweges, den das Kind zurückgelegt hat, bevor es von der Skilehrerin aufgefangen wird.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.2.2 </summary>

Gliedern Sie die Bewegungen in verschiedene Abschnitte.
Überlegen Sie, welche Vorgänge vor dem Stoß, beim Stoß und nach dem Stoß stattfinden. Nutzen Sie für die Bewegungen jeweils eine Energiebilanz, für den Stoßvorgang den
zutreffenden Impulserhaltungssatz.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.2.2 </summary>

![Aufgabe_4_L1.2](https://diversewolken.ddns.net/nextcloud/index.php/s/DNx4BR5zC656Lfa/download)

![Aufgabe_4_L1.2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/qAeB5NDJHek5gng/download)

</details>

</div>

## 2.9 Gleichförmige Kreisbewegung

<p class="newspaper">

![Kreisbewegung1.png](https://diversewolken.ddns.net/nextcloud/index.php/s/KwTabXpYXzfopyB/download) <!-- style="width:100%" -->

<p class="cb">

Ein Körper befindet sich in einer gleichförmigen Kreisbewegung, wenn er sich auf einer Kreisbahn mit konstantem Radius und auf seiner Bahn in gleich langen Zeitspannen gleich lange Strecken s zurücklegt. 

Hierbei sind:

> $\hspace{0.5cm}$ $r$ .. Radius der Kreisbahn
>
> $\hspace{0.5cm}$ $\vec{v}$ .. Bewegungsgeschwindigkeit
>
> $\hspace{0.5cm}$ $s$ .. Strecke auf der Kreisbahn
>
> $\hspace{0.5cm}$ $\varphi$ .. Drehwinkel
>
> $\hspace{0.5cm}$ $m$ .. Masse des Körpers
>
> $\hspace{0.5cm}$ $F_r$ .. Radialkraft

</p>

</p>
>> <div style="color:red">Zentripedalkraft / Radialkraft $F_r$</div>
>> 
>> Eine gleichförmige Kreisbewegung benötigt immer eine zum Mittelpunkt gerichtete Kraft. Diese Kraft heißt Radialkraft (Synonym: Zentripetalkraft). Sie wirkt senkrecht zur Bahngeschwindigkeit zum Mittelpunkt hin.
>>
>> Formel: $$ \boxed{F_r = \dfrac{m \cdot v^2}{r}} $$

> __Deutung:__ Die Zentripedalkraft $F_r$ ist notwendig, damit sich ein Körper der Masse $m$ auf einer Kreisbahn mit dem Radius $r$ und der Geschwindigkeit $v$ bewegt. Sie wirkt immer senkrecht zur Bewegungsrichtung.

### Aufgaben zur Kreisbewegung

Im Folgenden sind Aufgaben zur Kreisbewegung gestellt. Die Aufgaben sind mit "Aufwändigkeits-Marken" versehen.

- (+) geringer Aufwand
- (++) mittlerer Aufwand
- (+++) erhöhter Aufwand

<p style="color:red">
>> __Löse insgesamt 7 Aufgaben. Davon sollen mindestens zwei Aufgaben (++) und eine Aufgabe (+++) enthalten sein.__
</p>

#### 1. Kugel am Faden (++)

Eine Kugel (m = 2,5 kg) wird gleichförmig an einem Faden der Länge 40 cm mit einer Bahngeschwindigkeit von 36 km/h auf einer Kreisbahn bewegt.​

---

1. 1. Benenne die Kraft, welche auf die Kugel wirkt und als Zentripedalkraft fungiert.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.1 </summary>

Der Faden hält die Kugel auf der Kreisbahn. Demzufolge fungiert die Fadenkraft hier als Zentripedalkraft.

</details>

</div>

---


1. 2. Berechne die Kraft, welche auf die Kugel wirkt und als Zentripedalkraft fungiert.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.2 </summary>

Rechne sämtliche gegebenen Größen in die Standardeinheiten um und setze diese in die Formel für die Zentripedalkraft (2.9.) ein.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.2 </summary>

$$F_r = \dfrac{m \cdot v^2}{r} = \dfrac{2,5\,kg \cdot (10\frac{m}{s})^2}{0,4\,m} = 625\,N$$

</details>

</div>

---

1. 2. Berechne die Zeit, die nötig ist, damit die Kugel zwei Umdrehungen schafft.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.3 </summary>

Berechne aus den gegebenen Werten den Umfang $u$ des Kreises. Die Kugel legt in gleichförmiger Bewegung die Strecke $2u$ zurück. Mit der gegebenen Geschwindigkeit lässt sich die Zeit ermitteln.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.3 </summary>

Der Umfang $u$ eines Kreises wird berechnet mit $u = 2\pi\cdot r$. Die Zeit, welche die Kugel bei gleichförmiger Bewegung für 2 Umläufe braucht ist daher $$t=\frac{2\cdot u}{v}\approx0,503\,s$$.

</details>

</div>

#### 2. Fahrradtachometer (++)

Ein Fahrradtachometer bestehend aus einem Sensor und einem Magneten (mittig montiert auf der Speiche zwischen Lauffläche und Nabe). Das Rad hat einen Durchmesser von 635 mm. Er misst alle 0,25s eine Umdrehung.

---

2. 1. Fertige eine Skizze zur Aufgabe an. Trage die gegebenen Größen ein.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.1 </summary>

![KB_Lsg_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/PEYT5WH9o8x4GGH/download)

</details>

</div>

---

2. 2. Berechne die Bahngeschwindigkeiten des Magneten und der Lauffläche.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.2 </summary>

![KB_Lsg_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/6GEe3gTeiG7pMyS/download)

</details>

</div>

---

2. 3. Berechne die Kraft, die nötig ist, damit der Magnet ($m=10g$) an der Speiche bleibt.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.3 </summary>

![KB_Lsg_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/P3W7LZBZ3LaHCnB/download)

</details>

</div>

#### 3. Satellitenbahn (+++)

3. 1. Erläutere die Bewegung eines Satelliten um die Erde. Erkläre warum der Satellit nicht auf die Erde stürzt. 

<div style="text-indent:10%">

<details>

<summary> Lösung 3.1 </summary>

![KB_Lsg_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/kYBZsG4kTxDngXf/download)

</details>

</div>

---

3. 2. Zeige, dass der Radius des geostationären Orbits für Erdsatteliten etwa 42000 km beträgt. <br> _Hinweis: Bei einem geostationären Orbit bleibt der Satellit immer über dem gleichen Punkt auf der Erdoberfläche._

<div style="text-indent:10%">

<details>

<summary> Hinweis 3.2. A</summary>

Recherchiere, wie sich die Gravitationskraft in größerer Entfernung von der Erde berechnen lässt (hier gilt nicht $F_g=m\cdot g$).

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Hinweis 3.2. B </summary>

$$ F_g = G\cdot\frac{m\cdot M}{r^2} $$ 

($M$..Erdmasse, $G$..Graviationskonstante)

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 3.2 A </summary>

![KB_Lsg_3.2A](https://diversewolken.ddns.net/nextcloud/index.php/s/9Tbn8xWaW97xXCL/download)

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 3.2 B </summary>

![KB_Lsg_3.2B](https://diversewolken.ddns.net/nextcloud/index.php/s/RiTem8mfeWk2ZZt/download)

</details>

</div>

#### 4. Kurvenfahrt (+++)

Bei Kurvenfahrten mit konstanter Geschwindigkeit treten an einem Fahrzeug zwischen Reifen und Fahrbahn zwei Arten von Reibungskräften auf. Die Rollreibung wirkt parallel zur Bewegungsrichtung, Haftreibung wirkt senkrecht zur Bewegungsrichtung. 
Ein Fahrzeug (1,5 t) bewegt sich auf einer kreisförmigen Kurve (Radius 50 m) mit einer konstanten Geschwindigkeit von 72 km/h. Die Haftreibungszahl µHaft zwischen Reifen und Fahrbahn beträgt 0,85. Die Rollreibungszahl µRoll beträgt 0,025.

---

4. 1. Entscheiden Sie, ob die Haftreibung in diesem Fall eine erwünschte oder eine unerwünschte Reibungskraft ist. Begründen Sie Ihre Entscheidung. Ermitteln Sie den Wert der Haftreibungskraft.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.1</summary>

Für eine Kreisbewegung muss eine Kraft als Zentripedalkraft zum Mittelpunkt der Kreis/Kurvenbahn zeigen. Überlegen Sie welche der beschriebenen Kräfte, das sein könnte und entscheiden Sie dann, ob diese Kraft erwünscht ist.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.1 A</summary>

Da die Zentripedalkraft immer senkrecht zur Bewegungsrichtung wirkt, kommt hier nur die Haftreibungskraft als Zentripedalkraft in Frage. Diese wäre dann eine erwünschte Reibungskraft, weil sonst die Kurvenfahrt nicht durchgeführt werden könnte.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.1 B</summary>

$F_{haft} = F_g \cdot \mu_{haft} = m \cdot g \cdot \mu_{haft} = 1500\,kg\cdot9,81\,\frac{N}{kg}\cdot0,85$

$\underline{F_{haft} = 12508 N}$


</details>

</div>

---

4. 2. Begründen Sie, warum das Fahrzeug nicht mit beliebig hoher Geschwindigkeit durch die Kurve fahren kann. Diskutieren Sie dazu die für die Kreisbewegung relevanten Kräfte.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.2 </summary>

Die Haftreibungskraft wirkt als Zentripedalkraft. Überprüfen Sie anhand der Formel den Zusammenhang von Zentripedalkraft und Geschwindigkeit. Schätzen Sie ein, ob sich die Haftreibungskraft mit zunehmender Geschwindigkeit ändert?

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.2</summary>

Die Haftreibungskraft ist nicht von der Geschwindigkeit abhängig. Bei wachsender Geschwindigkeit aber festem Kurvenradius muss die Zentripedalkraft wachsen, damit die Kreisbewegung stattfinden kann. Überschreitet die geforderte Zentripedalkraft die Haftreibungskraft, so rutscht das Fahrzeug aus der Kurve.

</details>

</div>

---

4. 3. Ermitteln Sie die Höchstgeschwindigkeit für die beschriebene Kurvenfahrt.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.3 </summary>

Setzen Sie für den Grenzfall Haftreibungskraft und Zentripedalkraft gleich.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.3 </summary>

![KB_Lsg_4.3](https://diversewolken.ddns.net/nextcloud/index.php/s/9Zjg4azKE4CmNAA/download)

</details>

</div>

#### 5. Erdrotation (+)

5. Der Erdradius beträgt etwa 6370 km. Ermitteln Sie die Geschwindigkeit, mit der sich ein Punkt auf der Erdoberfläche des Äquators bei der Erddrehung bewegt? Beachten Sie: Die Erde dreht sich in einem Tag einmal um sich selbst.

<div style="text-indent:10%">

<details>

<summary> Lösung 5. </summary>

>![Lsg_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/JDkA7GJwBgw8Led/download)

</details>

</div>

#### 6. Turmuhr (++)

6.1  Die Spitze des Minutenzeigers einer Turmuhr hat die Geschwindigkeit $1,5 \frac{mm}{s}$. Ermitteln Sie die Zeigerlänge?

<div style="text-indent:10%">

<details>

<summary> Lösung 6.1 </summary>

>![Lsg_3.2](https://diversewolken.ddns.net/nextcloud/index.php/s/LQAmgYazNjHo3rD/download)

</details>

</div>

---

6.2  Bestimmen Sie unter Berücksichtigung physikalisch möglicher Geschwindigkeiten die maximale (hypotetische) Größe einer Uhr, d.h. ihrer Zeigerlänge (Minutenzeiger). Setzen Sie Ihr Ergebnis mit einer typischen astronomischen Entfernung sinnvoll ins Verhältnis.

<div style="text-indent:10%">

<details>

<summary> Hinweis 6.2 </summary>

Ermitteln Sie die größte überhaupt mögliche Geschwindigkeit. Überlegen Sie, welcher Teil der Uhr sich mit der größten Geschwindigkeit bewegt. Setzen Sie die Maximalgeschwindigkeit für diesen Teil an.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 6.2 A</summary>

Die maximal mögliche Geschwindigkeit ist die Lichtgeschwindigkeit $c=300.000\,\frac{km}{s}$. Der schnellste Teil einer Uhr ist die Zeigerspitze des Minutenzeigers. Dieser kann sich nach physikalischen Prinzipien nicht schneller als mit Lichtgeschwindigkeit bewegen. Setzt man Lichtgeschwindigkeit für die Zeigerspitze an, ergibt sich die größtmögliche Uhr. Setzen Sie dieses Ergebnis mit einer astronomischen Entfernung sinnvoll ins Verhältnis.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 6.2 A</summary>

$ c = \dfrac{2\pi\cdot r}{T}$ mit $T=60\cdot60\,s$ und $c=300.000.000\,\frac{m}{s}$

$ r = \dfrac{T\cdot c}{2\pi} = \dfrac{3600\,s\cdot 300.000.000 \frac{m}{s}}{2\pi}$

$ \underline{r \approx 1,72 \cdot 10^{11}m}$

Der Abstand Erde Sonne (auch eine astronomische Einheit genannt) beträgt etwa $1,5\cdot 10^{11}m$. Der Minutenzeiger einer Uhr und deren Zeiger sich um das Zentrum der Sonne drehen würden, deren Länge etwas weiter als bis zur Erde reichen würde, hätten an der Spitze ungefähr Lichtgeschwindigkeit.

Alternativ: Das Verhältnis der hypothetischen Zeigerlänge zum Abstand Erde-Sonne beträgt etwa 1,15.

</details>

</div>

#### 7. Dynamo (+)

7. Fahrradfahren/Dynamo

![A3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/Xz8KES8f8kHPE3G/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 7. </summary>

> ![Lsg_3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/XsJtHCgnrrBqPb5/download)

</details>

</div>

#### 8. Flugzeugturbinen (+)

8. Turbinen und Drehgeschwindigkeit

![A3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/A4yG37d3eHf6ZTL/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 8. </summary>

> ![Lsg_3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/qTEzgnK4ZZcGcxB/download)

</details>

</div>

#### 9. Winkelschleifer (+)

![A3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/5xsPM2oXRNsEmzZ/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 9. </summary>

> ![Lsg_3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/dEGwgjJLZ5Lx9YY/download)

</details>

</div>

## Rückgabe Klausur

__Verteilung__

![Verteilung_Kl1](https://diversewolken.ddns.net/nextcloud/index.php/s/oNjdMyiSNnSPTbR/download)

- Nächste LK: @color(vor Weihnachten, red)

- Nächste Klausur: @color(15.01.,red)

## 2.10 Kurvenfahrt mit Fahrbahnüberhöhung


{{1}}
*********

![TB_KraefteBeiKurvenfahrten](https://diversewolken.ddns.net/nextcloud/index.php/s/cfAWrYFHTDGYdgw/download)

*********

<details>

<summary> Ablauf der Stunde </summary>

1. [LEIFI-Physik Aufgabe zur Bobfahrt](https://www.leifiphysik.de/mechanik/kreisbewegung/aufgabe/bobfahrer-der-kurve)

2. [LEIFI-Physik Aufgabe zur Kugel in Rinne](https://www.leifiphysik.de/mechanik/kreisbewegung/versuche/kugel-rotierender-rinne)

2. Aufgabe zur @color(__gegenseitigen Beurteilung__, orange)

    - 20 min Aufgabe bearbeiten (danach Tausch mit Partner)

    - 20 min Muster-Lösung mit Punkten gemeinsam besprechen

    - 15 min Lösung des Partners korrigieren

</details>

## 2.11 Abiturähnliche Aufgabe zur Rodelbahn

> Im sächsischen Altenberg befindet sich eine Bobbahn. Beim Einerbob erteilt der Pilot dem Bob eine Anfangsgeschwindigkeit. Er steuert den Bob durch kleine auf die Kufen übertragene Lenkbewegungen durch den Eiskanal.
>
> Verschiedene grundlegende physikalische Prinzipien werden untersucht, die Vorgänge werden modellhaft vereinfacht. Die folgenden Teilaufgaben sind unabhängig voneinander.

1. Eine Person der Masse $70\,kg$ springt mit der Geschwindigkeit $7,0\,\frac{m}{s}$ auf einen ruhenden, gleitfähigen Körper der Masse $200\,kg$ und bewegt sich gemeinsam mit diesem weiter. Berechnen Sie die infolge der Wechselwirkung maximal mögliche Geschwindigkeit. <br> $$\mathrm{2\,BE}$$

{1}{![Lsg_1](https://diversewolken.ddns.net/nextcloud/index.php/s/yFxa7rzqyNRBMzM/download)}

2. Ein Körper der Masse $270\,kg$ gleitet aus der Ruhe heraus eine Ebene geradlinig herab. Der Neigungswinkel beträgt $10,0^\circ$, die Gleitreibungszahl ist konstant $0,015$. Der Luftwiderstand wird vernachlässigt. <br> Weisen Sie nach, dass der Körper mit  $a \approx 1,6 \frac{m}{s^2}$ beschleunigt wird. <br> $$\mathrm{3\,BE}$$

{2}{![Lsg_2](https://diversewolken.ddns.net/nextcloud/index.php/s/PNzNai7TWYERCDX/download)}

3. Der Körper gleitet nun geradlinig eine geneigte Ebene hinab, Gleitreibungszahl und Luftwiderstand werden nicht vernachlässigt. Zeigen Sie, dass sich bei einer Verdopplung der Geschwindigkeit die Luftreibungskraft vervierfacht. Begründen Sie, dass die Bewegung des Körpers im weiteren Verlauf gleichförmig werden kann. <br> $$\mathrm{2\,BE}$$

{3}{![Lsg_3](https://diversewolken.ddns.net/nextcloud/index.php/s/3ZdzjLqGXrkSx4j/download)}

4. Ein Körper gleitet gleichförmig durch eine überhöhte Kurve. Körper und Bahn wechselwirken so, dass die Wirkungslinie der zugehörigen Kraft (siehe Abbildung) genau senkrecht zur Bahn gerichtet ist, der Körper gleitet somit in konstanter Bahnhöhe h durch die Kurve. 

    ![BobBahn](https://diversewolken.ddns.net/nextcloud/index.php/s/s2JE9kJ7pZWjyZs/download "Foto und Querschnitt der Bobbahn.")

    Zeichnen Sie diese Abbildung in Ihre Aufzeichnungen. Ergänzen Sie ein maßstabsgetreues Kräfteparallelogramm und benennen Sie die Kraftpfeile.<br> $$\mathrm{3\,BE}$$

    {4}{![Lsg_4](https://diversewolken.ddns.net/nextcloud/index.php/s/xKe3fkrXdWsjAZE/download)}

    
## Simulation zum Looping

Aufgabe: Untersuche die Bewegung des Körpers an einem Looping. Welche Geschwindigkeit muss der Körper bei der Einfahrt in den Looping haben, damit er nicht "rausfliegt"?

Empirische Beobachtung:

1. Stelle die Anfangshöhe zunächst auf die gleiche Höhe (1m), wie den höchste Punkt des Loopings und beobachte die Bewegung.

2. Überprüfe, ob die Masse des Körpers einen Einfluss auf den Bewegungsablauf hat.

3. Stelle eine Vermutung auf, warum der Körper den Looping nicht schafft. Beobachte dazu den höchsten Punkt, den der Körper erreicht und überprüfe in diesem Punkt seine Energiebilanz.

4. Untersuche empirisch, ab welcher Anfangshöhe der Körper den Looping schafft.

??[Looping](https://www.walter-fendt.de/html5/phde/looping_de.htm)

Theoretische Untersuchung:

1. Wenn der Körper den obersten Punkt erreicht hat, wirkt auf den Körper neben der Zwangskraft durch die Loopingbahn eine weitere Kraft. Welche ist das. Notiere eine Berechnungsformel. Notiere auch die potentielle Energie, die der Körper in diesem Punkt hat. Beziehe dich auf den Radius des Kreises.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

     Gewichtskraft: $F_g = m \cdot g$

     potentielle Energie: $E_{pot} = m \cdot g \cdot (2r)

</details>

</div>

2. Im Grenzfall ist diese Kraft gleich der Zentripetalkraft, welche zur erzwungenen Kreisbahn passt. Notiere eine Formel für die Zentripetalkraft und setze diese gleich der wirkenden Kraft (aus 1.).

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

    $$ F_{ZP} = \dfrac{m \cdot v^2}{r} $$

    $$ \boxed{F_{ZP} = F_g} $$

    $$ \dfrac{m \cdot v^2}{r} = m \cdot g $$

</details>

</div>

3.  Stelle die Gleichung (aus 2.) nach der Geschwindigkeit um. Notiere auch die zugehörige kinetische Energie

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

    $$ v = \sqrt{g\cdot r} $$

    $$ E_{kin} = \frac{1}{2} \cdot m \cdot v^2 $$

    $$ E_{kin} = \frac{1}{2} \cdot m \cdot g \cdot r $$

</details>

</div>

4. Diese Geschwindigkeit (bzw. kin. Energie) muss dem Körper im obersten Punkt mindestens verbleiben, damit er im Looping verbleibt. Notiere die Gesamtenergie, die der Körper im obersten Punkt mindestens haben muss.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

    $$ E_{ges} = E_{pot} + E_{kin} $$
    
    $$ E_{ges} = m \cdot g \cdot (2r) + \frac{1}{2} \cdot m \cdot g \cdot r $$

    $$ E_{ges} = m \cdot g \cdot (2r + \frac{1}{2} r) $$

    Ergebnis: Die Gesamtenergie des Körpers muss zu jedem Zeitpunkt, __@color(also auch zu Beginn der Bewegung, orange)__ mindestens der potentiellen Energie des 2,5 fachen Radius entsprechen.

</details>

</div>

## 2.12 Kräftegleichgewicht an einer Looping-Bahn

Wir betrachten einen Körper, der auf einer festen Schiene gleitet, welche einen Looping enthält. Zur Vereinfachung werden Reibungseffekte vernachlässig. 

> __Bedingung:__ Der Körper kann den Looping erfolgreich durchfahren, wenn die radiale Komponte, der auf den Körper wirkenden Kraft in jedem Punkt kleiner ist, als die zur momentanen Geschwindigkeit gehörende @color(Zentripetalkraft $F_{ZP}$,red).

> __Analyse:__ Auf den Körper wirkt während der gesamten Fahrt lediglich die Gewichtskraft $F_g$. Im obersten Punkt des Loopings zeigt $\vec{F_g}$ zum Mittelpunkt des Looping-Radius. Somit ist der radiale Anteil von $F_g$ hier am größten. In diesem Punkt darf $F_g$ nur maximal der Zentripetalkraft bezogen auf Radius $r$ und Geschwindigkeit $v$ sein.

> __Berechnung der minimalen Geschwindigkeit $v_{min}$ im obersten Punkt für den Grenzfall $F_{ZP}=F_g$:__
>
> $$ F_{ZP} = F_g$$
>
> $$ \dfrac{m\cdot v_{min}^2}{r} = m \cdot g$$
>
> $$ \dfrac{m\cdot v_{min}^2}{r} = m \cdot g$$
>
> $$ v_{min}^2 = r \cdot g$$
>
> __Die @color(minimale mechanische Gesamtenergie $E_{ges}=E_{pot}+E_{kin}$,red) des Körpers beträgt daher:__
>
> $$ E_{ges} = m \cdot g \cdot (2r) + \frac{1}{2} \cdot m \cdot g \cdot r $$
>
> $$ E_{ges} = m \cdot g \cdot (2r + \frac{1}{2} r) $$

> __Ergebnis__: Die Gesamtenergie des Körpers muss zu jedem Zeitpunkt, __@color(also auch zu Beginn der Bewegung, orange)__ mindestens der potentiellen Energie des 2,5 fachen Radius entsprechen.

### Übungsaufgaben zum Looping

<bdi style="color:red"> Die überprüfbaren Lösungen werden mit drei signifikanten Stellen überprüft. D.h. wenn das Ergebnis 16,786 m ist, muss 16,8 m gerundet werden. Bei 0,086434 s, sollte 0,0864 s überprüft werden. <br> __Signifikante Stellen__ sind diejenigen Ziffern, die nach den führenden Nullen folgen.
</bdi>

1. Eine Achterbahn soll eine Loopingkurve durchfahren. Sie durchfährt den höchsten Punkt des Kreises mit der Geschwindigkeit 50 km/h. Wie groß darf der Radius der Kreisbahn höchstens sein? 

@rangeQuiz2($\hspace{1cm}$ r,19.7,m)

<p class="newspaper">

2. Im Punkt B steht ein Wagen K mit einer Masse von 20,0 g direkt vor einer entspannten Feder. Die Feder hat eine Federkonstante von $112,5 \frac{N}{m}$. Der Körper wird bis zum Punkt A geschoben, wodurch die Feder um 10 cm zusammengedrückt wird. <br> In A wird der Körper dann aus der Ruhe heraus losgelassen. <br> Er bewegt sich mit einer vernachlässigbaren Reibung über B, C, D, E nach C. Auf dem weiteren Weg zwischen C und F tritt Reibung auf.

<p class="cb">

__Skizze:__

![Aufgabe_Looping](https://diversewolken.ddns.net/nextcloud/index.php/s/bpNoweSbDj7t8a4/download)

</p>

</p>

<bdi style="color:orange">_Hinweise: <br> -> Die Marker (+) oder (++) weisen auf den Rechenaufwand hin._<br> -> _Sämtliche überprüfbaren Lösungen sind auf drei signifikante Stellen in der gegebenen Einheit gerundet._</bdi>

2. a) (+) Zeigen Sie, dass der Körper den Punkt C mit $7,5 \frac{m}{s}$ durchfährt.

<div style="text-indent:10%">

<details>

<summary> Lösung a) </summary>

![Looping_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/s3LDidLkHEbLYew/download)<!-- style="width:80%"-->

</details>

</div>

2. b) (+) Der Looping hat einen Radius von 1,00 m. Ermitteln Sie den Wert der Radialkraft im Punkt D (welche durch die Bahn als Zwangskraft ausgeübt wird).

@rangeQuiz2($\hspace{1cm}$ $F_R$, 0.733, N)

<div style="text-indent:10%">

<details>

<summary> Lösung b) </summary>

![Looping_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/8ssegiDmPA6tcMq/download)<!-- style="width:80%"-->

</details>

</div>

2. c) (++) Der Körper soll die Loopingbahn vollständig durchlaufen. Wird zuvor die Feder nicht ausreichend zusammengedrückt, reicht die Geschwindigkeit im Punkt C nicht aus, um komplett durch den Kreis zu kommen. <br> Ermitteln Sie die Strecke s, welche die Feder mindestens zusammengedrückt werden muss, damit der Körper den Looging durchlaufen kann.

@rangeQuiz2($\hspace{1cm}$ s, 9.34, cm)

<div style="text-indent:10%">

<details>

<summary> Lösung c) </summary>

Damit der Wagen den Looping durchfahren kann, braucht er im oberen Punkt eine bestimmte Mindestgeschwindigkeit $v_{min}$.

Bei $v_{min}$ entspricht die Gewichtskraft $F_g$ exakt der zum Radius passenden Radialkraft $F_R$. Setzt man diese gleich, so erhält man einen Ausdruck für die Mindestgeschwindigkeit im Punkt E.

$$F_{ZP}=F_g$$

$$ v_{min} = \sqrt{g \cdot r} $$

Zur Probe: $$ v_{min} \approx 3,13 {m}{s} $$

Diese Geschwindigkeit entspricht der kinetischen Energie:

$$ E_{kin} = \frac{1}{2} \cdot m \cdot v^2 $$

Zur Probe: $$ E_{kin} = 0,0981 J $$

Zusätzlich benötigt der Körper in diesem Punkt die potentielle Energie $E_{pot}$:

$$ E_{pot} = m \cdot g \cdot (2r) $$

Zur Probe: $$ E_{pot} = 0,3924 J $$

Die Gesamtenergie des Körper, zu Anfang als Spannenergie $E_{sp}$ im Punkt A wird also im Punkt E in $ E_{kin}+E_{pot} $ umgewandelt. Energieerhaltung:

$$ E_{sp} = E_{kin}+E_{pot} $$ 

Eingesetzt (mit Formelzeichen)

$$ \frac{1}{2}\cdot D \cdot s^2 = \frac{1}{2} \cdot m \cdot v_{min}^2
 + m \cdot g \cdot (2r) $$ 

Bzw. wie schon die Untersuchung zum Looping ergab:

$$ \frac{1}{2}\cdot D \cdot s^2 = m \cdot g \cdot 2,5r $$

Die Strecke s ergibt sich also zu:
$$ s = \sqrt{\dfrac{5 \cdot m \cdot g}{D}} $$

Bzw. als Ergebnis

$$ s \approx 0,0934 m = 9,34 cm $$

</details>

</div>

2. d) (++) Nach dem Durchlaufen der Looping-Bahn bewegt sich der Wagen von C nach F fort. Auf dieser Streckt beträgt die Reibungszahl 0,5. Der Körper hat im Punkt F eine Geschwindigkeit von $5 \frac{m}{s}$. Ermittlen Sie die Länge der Strecke $l = \overline{CF}$.

@rangeQuiz2($\hspace{1cm}$ l, 3.19, m)

<div style="text-indent:10%">

<details>

<summary> Lösung d) </summary>

Wie in Aufgabe a) gezeigt beträgt die Geschwindigkeit in Punkt C $7,5 \frac{m}{s}$. Die Reibungsarbeit $W_R = F_R \cdot l$ ergibt sich aus der Differenz der kinetischen Energien in Punkt C und F.

$$ W_R = E_{kin, C} - E_{kin, F} $$

und eingesetzt:

$$ F_R \cdot l = \frac{1}{2} \cdot m \cdot v_{C}^2 - \frac{1}{2} \cdot m \cdot v_{F}^2 $$

Da die Reibungskraft $F_R = F_g \cdot \mu = m \cdot g \cdot \mu$ berechnet werden kann, findet man:

$$ m \cdot g \cdot \mu \cdot l = \frac{1}{2} \cdot m \cdot v_{C}^2 - \frac{1}{2} \cdot m \cdot v_{F}^2 $$

und für $l$ schließlich

$$ l = \dfrac{v_C^2 -v_F^2}{2\cdot g \cdot \mu} $$

$$ l \approx 3,19 m $$ 

</details>

</div>

2. e) (+++) Vom Punkt F aus geht es reibungsfrei weiter. Der nach unten gehende Bogen hat einen Radius $r_2$ von 3,00 m. Im Punkt G löst sich der Wagen von der Bahn und hebt ab. Ermitteln Sie den Winkel Alpha?

@rangeQuiz2($\hspace{1cm}$ $\alpha$, 18.2, °)

<div style="text-indent:10%">

<details>

<summary> Lösung e) </summary>

![Looping_Lsg_e](https://diversewolken.ddns.net/nextcloud/index.php/s/rLKSp9JRz3D6eGB/download)

</details>

</div>

# LB 3 Kinematik und Dynamik - Praktikum

@uhr

![KinematikUndDynamik](https://www.online-wissensdatenbank.de/wp-content/uploads/2023/12/kinematik-grundlagen-der-bewegungslehre.jpg "Bild-Quelle: https://www.online-wissensdatenbank.de")

## 3.1. Einführung in die Analyse von Bewegungen

Die __Kinematik__ (altgriechisch κίνημα kinema, deutsch ‚Bewegung‘) ist das Gebiet der Mechanik, in dem die Bewegung von Körpern rein geometrisch mit den Größen <bdi style="color:red">Ort, Zeit, Geschwindigkeit und Beschleunigung</bdi> beschrieben wird.

{{1}}
*******
__Formelzeichen:__

<div style="text-indent:10%">

> $t$ .. Zeit $\Big[ s \Big]$
>
> $x,y,z$ .. Ort/Position/Koordinate des Körpers $\Big[ m \Big]$
>
> $v$ .. Geschwindigkeit des Körpers $\Big[ \dfrac{m}{s} \Big]$
>
> $v_x$, $v_y$, $v_z$ .. Geschwindigkeits-Komponenten in x- y- bzw. z-Richtung
> 
> $a$ ..Beschleunigung $\Big[ \dfrac{m}{s^2} \Big]$
>
> $a_x$, $a_y$, $a_z$ .. Beschleunigungs-Komponenten in x- y- bzw. z-Richtung

</div>
*******

{{2}}
*******
__Abhängigkeiten:__ Um zu beschreiben, zu welcher Zeit sich ein Körper an welchem Ort aufhält, notiert man die Beziehung verschiedener kinematischer Größen folgender Art

_Beispiele:_

<div style="text-indent:10%">

> $x(t)$ ..  @color(_Gesprochen: x von t_,blue) bedeutet: Der Körper befindet sich zum Zeitpunkt $t$ am Ort $x$
>
> $v_x(t)$ .. Der Körper besitzt zum Zeitpunkt $t$ die x-Geschwindigkeit $v_x$ (oder Geschwindigkeit in x-Richtung)  

</div>
*******

{{3}}
*******
<bdi style="color:blue">
_Hinweis:_ Werden eindimensionale Probleme behandelt wird gelegentlich auf die Angabe der Koordinaten verzichtet. Dann kann für $x$ auch die Strecke $s$ und für die Geschwindigkeit lediglich $v$ genutzt werden.
</bdi>
******

## 3. 2. Kinematische Darstellung in Diagrammen

Häufig ist es __anschaulich__ die Bewegung eines Körpers in @color(Diagrammform, red) darzustellen.

<bdi style="color:red">
Vereinbahrung: In der Kinematik wird die Zeit __immer__ auf der x-Achse dargestellt.
</bdi>

Beispiel: x(t) Diagramm

![BeispielDiagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/EsD2fMgGed8tjRC/download)

__Aufgabe:__ Ergänze die Bewegungsarten

- P0 -> P1 

    <!-- data-solution-button="off" -->
    [(X)] Stillstand
    [( )] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung

- P1 -> P2

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [( )] gleichförmige Bewegung
    [(X)] gleichmäßig beschleunigte Bewegung

- P2 -> P3

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [(X)] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung


## 3. 3. Einführung Bewegungsanalyse

__Möglichkeiten zur zeitlichen Analyse von Bewegungen gibt es viele:__

- Stoppuhr und Maßband

- Maßband und Lichtschranke

- Videoanalyse 

- Ultraschallsensoren

- ...

{{1}}
**********
__Heute:__ Videoanalyse-Tool VIANA 2

@color(_Hinweise zur Handhabung:_,blue)

1. Positioniere die Kamera so, dass sie sich nicht bewegt.

2. Achte auf einen guten Kontrast zwischen bewegtem Objekt und Hintergrund während der gesamten Bewegung.

3. Führe vor der Aufnahme ein paar Beispielabläufe durch.

4. Markiere die vorab einen möglichst großen Streckenabschnitt im Bewegungsraum.

5. Bei eindimensionalen Bewegungen sollte das Koordinatensystem so ausgerichtet werden, dass sich das Objekt entlang der x-Achse bewegt.
*********

{{2}}
*********
__Aufgaben:__

1. Mache dich mit der Videoanalyse in VIANA 2 vertraut

2. Nimme eine gleichmäßg beschleunigte Bewegung anhand der Erklärung im Unterricht auf. 

3. Stelle das x(t) und v(t) Diagramm in der App __Numbers__ auf dem IPad dar. 

4. Ermittle die Beschleunigung aus den Messwerten der Kugel.

@rangeQuiz20($\hspace{1cm}$ $a$, 0.11, $\frac{m}{s^2}$)

_Hinweis: Bei dieser Überprüfung wird eine Ungenauigkeit von 20% gegenüber der Vergleichsmessung der Lehrkraft akzeptiert._

**********

## 3. 4. Bewegungsgleichungen für gleichförmige und gleichmäßig beschleunigte Bewegung

@color(Fertige eine Übersicht mit den Bewegungsgleichungen zur gleichförmigen und gleichmäßig beschleunigten Bewegung an. Ergänze die fehlenden Punkte., blue)

{{0-1}}
*****************

@timer(10,00)

| | Gleichförmige Bewegung | Gleichmäßig beschleunigte Bewegung |
| --- | --- | --- |
| Bedingungen für Gültigkeit | .. | .. |
| Bewegungsgleichungen | .. | .. |
| phys. Größen | .. | .. |
*****************

{{1-2}}
*****************
| | Gleichförmige Bewegung | Gleichmäßig beschleunigte Bewegung |
| --- | --- | --- |
| Bedingungen für Gültigkeit | $v(t) = konst. = v$ | |
| Bewegungsgleichungen | $s(t) = v \cdot t + s_0$ <br> $a(t) = 0$ | |
| phys. Größen | $v$ .. Geschwindigkeit <br> $s_0$ .. Anfangsweg |  |
****************

{{2}}
*****************
| | Gleichförmige Bewegung | Gleichmäßig beschleunigte Bewegung |
| --- | --- | --- |
| Bedingungen für Gültigkeit | $v(t) = konst. = v$ | $a(t) = const. = a$ |
| Bewegungsgleichungen | $s(t) = v \cdot t + s_0$ <br> $a(t) = 0$ | $s(t) = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t + s_0$ <br> $v(t) = a \cdot t +v_0$ |
| phys. Größen | $v$ .. Geschwindigkeit <br> $s_0$ .. Anfangsweg | $a .. $ Beschleunigung <br> $v_0$ .. Anfangsgeschwindigkeit <br> $s_0$ .. Anfangsweg |
****************



{{3}}
****************

__Graphen zu den Bewegungsgleichungen:__

![TB_Bewegungsgraphen](https://diversewolken.ddns.net/nextcloud/index.php/s/ALC7i99HXpRtPwT/download)

*****************

## 3. 5. Analyse einer gleichmäßig beschleunigten Bewegung

<p style="color:blue">

Analysiere die gleichmäßig beschleunigte Bewegung einer Kugel auf einer schiefen Ebene auf einer Strecke von s = 1m.

1. Nutze Metzler LB S18/19. Lies den Abschnitt 1.1.4. 

2. Zeichne eine Skizze und notiere alle geometrisch notwendigen Größen. Ermittle den Neigungswinkel der Ebene.

3. Erstelle mit Hilfe der Videoanalyse-Software ein s(t) und ein zugehöriges v(t)-Diagramm. 

4. Ermittle mit Hilfe der Bewegungsgleichung und eines Messwertes die Beschleunigung.

5. Erzeuge mit Hilfe deiner berechneten Beschleunigung einen theoretische s(t) und v(t) Graph und stelle diese mit den jeweiligen Messwerten gemeinsam dar.

6. Erzeuge aus den Diagrammen ein pdf und lade es [hier hoch](https://diversewolken.ddns.net/nextcloud/index.php/s/g5fRq7MWqJWJ8Sa), du erhältst einen Ausdruck.

7. Analysiere die auf die Kugel wirkenden Kräfte. Ermittle die wirkende Rollreibungskraft $F_R$ und den Rollreibungskoeffizienten $\mu_{roll}$.

</p>

__Lösungen:__

_Messwerte:_

- Länge des Tischs ca. 1,94 m

- Höhe des Blocks 0,03 m

- Masse der Kugel $m_K = 0,017 kg$

- Ermittelte Beschleunigung: $a_{exp} = 0,11 \frac{m}{s^2}$

_Berechungen:_

- Neigungswinkel $\alpha = \arctan{\frac{0,03}{1,94}} = 0,89^\circ$

- Beschleunigung ohne Reibung $a = g \cdot \alpha = 0,15 \frac{m}{s^2}$

### Aufgabe: Berechnungen an zusammengesetzten Bewegungen

__Erläuterung:__ Das folgende Diagramm wurde mit Hilfe der App Phyfox auf einer Autofahrt zwischen der _Tannenstraße (Dresden Neustadt)_ und der Haltstelle _Industriegebiet Süd_ aufgezeichnet. An Punkten, wo sich die Art der Bewegung ändert sind Markierungen auf dem Diagramm hinterlegt.

Die farbig gekennzeichneten Bereiche können als gleichmäßig beschleunigte Bewegungen betrachtet werden.

![Diagramm_PraktischeFahrt](https://diversewolken.ddns.net/nextcloud/index.php/s/K9XZ7yMM9n9AtLT/download)

> __Vorbetrachtung:__ Für die Bestimmung der Beschleunigung $a$ bei einer gleichmäßig beschleunigten Bewegung lässt sich auch die Formel
>
> $$ a = \frac{\Delta v}{\Delta t} $$
>
> verwenden. Hier bei ist $\Delta v$ die Geschwindkeitsänderung während des Zeitintervals $\Delta t$.
>
> Dabei ist $\Delta v$ definiert als 
>
> $$ \Delta v = v_{2} - v_{1}, $$
>
> also die Differenz der Geschwindigkeiten am Ende des Zeitintervals ($v_2$) und der Geschwindigkeit am Anfang des Zeitintervals ($v_1$).

__Löse folgende Aufgaben. Zur Selbstüberprüfung gibt es die Kontrollkästchen. Bei fehlerhaften Lösungen bitte per E-Mail rückmelden.__

1. Bestimme die gesamte Fahrtzeit (d.h. die gesamte Messzeit).

@rangeQuiz2($\hspace{1cm}$ t, 370, s)

---

2. Bestimme den gesamten Fahrtweg (d.h. die gesamte Messstrecke). 

@rangeQuiz2($\hspace{1cm}$ s, 3060, m)

---

3. Berechne die Geschwindigkeit  $v_2$, d.h. die Geschwindigkeit zwischen den Punkten 6 und 7 in der Einheit m/s.

@rangeQuiz2($\hspace{1cm}$ $v_2$, 12.56 , $\frac{m}{s}$)

---

4. Berechne die Geschwindigkeit  $v_3$, d.h. die Geschwindigkeit zwischen den Punkten 8 und 9 in der Einheit km/h.

@rangeQuiz2($\hspace{1cm}$ $v_3$, 63.16 , $\frac{m}{s}$)

---

5. Berechne die Durchschnittsgeschwindigkeit für die gesamte Messung/Fahrt (d..h von 0->11).

@rangeQuiz2($\hspace{1cm}$ $\overline{v_{ges}}$, 8.27 , $\frac{m}{s}$)

---

6. Berechne die Durchschnittsgeschwindigkeit für die gesamte Messung/Fahrt ohne Wartephase an den Ampeln, d.h. berechne die Durchschnittsgeschwindigkeit für die reine Bewegungszeit.

@rangeQuiz2($\hspace{1cm}$ $\overline{v'_{ges}}$, 11.91 , $\frac{m}{s}$)

<div style="text-indent:10%">

<details>

<summary> Lösung 6. </summary>

$ v_D = \frac{3060\,m}{370\,s-20\,s-73\,s-20s}= \frac{3060\,m}{257\,s} = 11,91 \frac{m}{s} = 15,15 \cdot 3,6 \frac{km}{h}  = 50 \frac{km}{h}$

</details>

</div>

---

7. Bestimme die Beschleunigungszeit zwischen den Punkten 5 und 6.

@rangeQuiz2($\hspace{1cm}$ $\overline{t_{5->6}}$, 25 , s)

---

8. Ermittle die Gschwindigkeitsänderung $\Delta v_{7->8}$ zwischen den Punkten 7 und 8.

@rangeQuiz2($\hspace{1cm}$ $\Delta v_{7->8}$, 4.985 , $\frac{m}{s}$)

<div style="text-indent:10%">

<details>

<summary> Lösung 8. </summary>

Die Geschwindigkeit $v_3$ beträgt $17,54 \frac{m}{s}$. Die Geschwindigkeit $v_2$ beträgt $12,56 \frac{m}{s}$. Die Änderung der Geschwindigkeit ist dann die Differenz $4,99 \frac{m}{s}$.

</details>

</div>

---

9. Ermittle die Beschleunigungen der farbig markiert Intervalle: $a_{1->2}$, $a_{3->4}$, $a_{5->6}$, $a_{7->8}$ und $a_{9->10}$.

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{1->2}$, 1.72 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Hinweis $a_{1->2}$  </summary>

Die Beschleunigung kann ermittelt werden aus der Änderungen der Geschwindigkeit $\Delta v$ geteilt durch die dafür benötigte Zeit $\Delta t$.

</details>

<details>

<summary> Lösung $a_{1->2}$  </summary>

Die Geschwindigkeit im Abschnit 0->1 ist $0 \frac{m}{s}$. Die Geschwindigkeit im Abschnitt 2->3 ist 

$$v_{2->3} = \frac{275m-60m}{50s-25s} = 8,6 \frac{m}{s}$$ 

Damit ist die Geschwindigkeitsänderung $\Delta v_{1->2} = 8,6 -0 \frac{m}{s} = 8,6 \frac{m}{s}$.

Die benötigte Zeit $\Delta t_{1->2} = 25s-20s = 5s$. Somit ist die Beschleunigung

$$ a_{1->2} = \frac{\Delta v_{1->2}}{\Delta t_{1->2}} = \frac{8,6 \frac{m}{s}}{5s} = 1,72 \frac{m}{s^2}$$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{3->4}$, -0.319 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Hinweis $a_{3->4}$  </summary>

Eine _gleichmäßg gebremste Bewegung_ ist eine gleichmäßig beschleunigte Bewegung mit @color(negativer, red) Beschleunigung. Da hier die Geschwindigkeit von $8,6 \frac{m}{s}$ auf $0 \frac{m}{s}$ sinkt, ist die Geschwindigkeitsänderung negativ. D.h. $\Delta v_{3->4} = -8,6 \frac{m}{s}$.

</details>

<details>

<summary> Lösung $a_{3->4}$  </summary>

$$ a_{3->4} = \frac{\Delta v_{3->4}}{\Delta t_{3->4}} = \frac{-8,6 \frac{m}{s}}{27s} = -0,319 \frac{m}{s^2}$$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{5->6}$, 0.502 , $\frac{m}{s^2}$)

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{7->8}$, 0.199 , $\frac{m}{s^2}$)

<div style="text-indent:10%">

<details>

<summary> Lösung $a_{7->8}$  </summary>

$$ a_{7->8} = \frac{\Delta v_{7->8}}{\Delta t_{7->8}} = \frac{v_{8->9} - v_{6->7}}{\Delta t_{7->8}} = \frac{17,54\frac{m}{s} - 12,56\frac{m}{s}}{25s}  = 0,199 \frac{m}{s^2} $$

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $\Delta a_{9->10}$, -0.877 , $\frac{m}{s^2}$)


## Bewegungsanalyse eines schrägen Wurfes

{{1}}
************
__$y(x)$-Diagramm__:

![Diagram-x-y](https://diversewolken.ddns.net/nextcloud/index.php/s/EpjbjtLSPyRePeZ/download)
************

<p class="newspaper">

{{2}}
************
__$x(t)$__

![Diagram-t-x](https://diversewolken.ddns.net/nextcloud/index.php/s/jN69KQoCJZdy8Xf/download)
************

{{3}}
************
__$v_x(t)$__

![Diagram-t-y](https://diversewolken.ddns.net/nextcloud/index.php/s/mGjYeN46XzHgsaE/download)
************

<p class="cb">

{{2}}
************
__$y(t)$__

![Diagram-t-vx](https://diversewolken.ddns.net/nextcloud/index.php/s/Ey7B9XgB7795GA6/download)
************

{{3}}
************
__$v_y(t)$__

![Diagram-t-vy](https://diversewolken.ddns.net/nextcloud/index.php/s/XBoLRYiosKtKCsx/download)
************

</p>

</p>

## 3.6 Kinematik des schrägen Wurfs

> __Beschreibung:__ Bei einem schrägen Wurf wird ein Körper unter einem Winkel $\alpha$ mit einer Anfangsgeschwindigkeit $\vec{v_0}$ abgeschossen (geworfen). Reibungseffekte werden zunächst vernachlässigt.

> __Zerlegung der Bewegung in x- und y-Richtung:__ 
{{1}}
*******
1. die Flugbahn $y(x)$ entspricht einer Parabel.
![Parabel](https://diversewolken.ddns.net/nextcloud/index.php/s/EpjbjtLSPyRePeZ/download)<!-- style="width:40%"-->
*******
{{2}}
*******
2. die horizontale Bewegung $x(t)$ ist eine __gleichförmige Bewegung__

$$ \boxed{x(t) = v_{0x} \cdot t} \mathrm{\ \ \ und\ \ \ } \boxed{v_x(t) = v_{0x}}$$

$\hspace{1cm}$ $v_{0x}$ .. Anfangsgeschwindigkeit in x-Richtung
*******
{{3}}
*******
3. die vertikale Bewegung $y(t)$ ist eine __gleichmäßig beschleunigte Bewegung__ mit dem Ortsfaktor $g=9,81\frac{m}{s^2}$ als Beschleunigung.

$$ \boxed{y(t) = \frac{1}{2}\cdot g \cdot t^2 + v_{0y} \cdot t} \mathrm{\ \ \ und\ \ \ } \boxed{v_y(t) = g \cdot t + v_{0y}}$$

$\hspace{1cm}$ $v_{0y}$ .. Anfangsgeschwindigkeit in y-Richtung

$\hspace{1cm}$ @color(Achtung:,red) Wenn die y-Achse nicht zur Erde hin zeigt, ist @color(g=-9.81$\frac{m}{s^2}$,red).
*******
{{4}}
*******
4. Die Anfangsgeschwindigkeit $\vec{v_0}$ ist eine vektorielle Größe und lässt sich in ihre x-Kompente ($v_{0x}$) und y-Komponente ($v_{0y}$) zerlegen. <br>
![Geschwindigkeit](https://diversewolken.ddns.net/nextcloud/index.php/s/qdAbC6XTmRXztaa/download)$$ \boxed{v_{0x} = v_0 \cdot \cos\alpha} \mathrm{\ \ \ und\ \ \ } \boxed{v_{0y} = v_0 \cdot sin\alpha} $$
*******
{{5}}
*******
5. die gesamte Bewegung ist eine @color(Superposition, red) (d.h. Überlagerung) der Bewegungen in x- und y-Richtung
*******

### 3.6.1 Berechnungen am Demonstrationsexperiment: Schräger Wurf

@timer(45,00)

Für das Demonstrationsexperiment beträgt der Abwurfwinkel $\alpha=59^\circ$. Die Anfangsgeschwindigkeit $v_0$ wird mit $3,21 \frac{m}{s}$ angegeben.

__Aufgaben__:

1. Ermittle die Anfangsgeschwindigkeiten $v_{0x}$ und $v_{0y}$.

@rangeQuiz2($\hspace{1cm}$$v_{0x}$, 1.65, $\frac{m}{s}$)

@rangeQuiz2($\hspace{1cm}$$v_{0y}$, 2.75, $\frac{m}{s}$)

---

2. Notiere die Bewegungsgleichungen x(t) und y(t). Schreibe alle Zahlenwerte aus.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

$$ x(t) = 1,65 \frac{m}{s} \cdot t $$

$$ y(t) = - \frac{1}{2} \cdot 9,81 \frac{m}{s^2}\cdot t^2 + 2,75 \frac{m}{s} \cdot t $$

</details>

</div>

---

3. Notiere die Bewegungsgleichungen $v_x(t)$ und $v_y(t)$.

<div style="text-indent:10%">

<details>

<summary> Lösung </summary>

$$ v_x(t) = 1,65 \frac{m}{s} $$

$$ v_y(t) = - 9,81 \frac{m}{s^2}\cdot t + 2,75 \frac{m}{s}$$

</details>

</div>

---

4. Ermittle für den höchsten Punkt: $t_{max}$, $x(t_{max})$, $y(t_{max})$. Vergleiche deine Berechung mit dem experimentellen Diagramm (aus 3.6). Hier ist $t_{max}$ der Zeitpunkt, an welchem der Körper die höchste Stelle erreicht.

@rangeQuiz2($\hspace{1cm}$ $t_{max}$, 0.28, $s$)

@rangeQuiz2($\hspace{1cm}$ $x_{max}$, 0.4625, $m$)

@rangeQuiz2($\hspace{1cm}$ $y_{max}$, 0.385, $m$)



<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Im Maximum ist $v_y(t)=0$.

</details>

</div>

5. Ermittle aus den Messdaten die Wurfweite $x_{Wurf}$, d.h die Entfernung, wo die Kugel wieder die Ausgangshöhe (0) zurückkehrt.

@rangeQuiz2($\hspace{1cm}$ $x_{wurf}$, 0.925 , $m$)

<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Für den Zeitpunkt der Wurfweite gilt:  $y(t_{wurf}) = 0$.

</details>

<details>

<summary> Lösung </summary>

Setze $ y(t_{wurf}) = 0 $:

$$ 0 = -\frac{1}{2} \cdot 9,81 \frac{m}{s^2}\cdot t^2 + 2,75 \frac{m}{s} \cdot t $$

$$ t_{wurf\,1} = 0\,\,\mathrm{(Startpunkt)}$$

$$ t_{wurf\,2} = \frac{2\cdot 2,75 \frac{m}{s}}{9,81 \frac{m}{s^2}} = 0,561 s$$

Berechne $ x(t_{wurf\,2}) $:

$$ x(t_{wurf}) = 1,65 \frac{m}{s} \cdot t_{wurf\,2} = 0,925\,m$$

</details>

</div>


6. Zeichne in das y(x)-Diagramm des Experiments die Flugbahn anhand der hier berechneten Daten. Nutze als Zeitschritte z.B. 0,05 s und die Bewegungsgleichungen aus 2. <br> Diskutiere Ursachen für die Unterschiede der beiden Graphen.

<div style="text-indent:10%">

<details>

<summary> Hinweis </summary>

Berechne für Zeitschritte von 0,05s x(t) und y(t) und trage die Punkte in das Diagramm ein.

</details>

<details>

<summary> Lösung </summary>

![Loesung_x_y](https://diversewolken.ddns.net/nextcloud/index.php/s/DqKyz8DiaDCfgi5/download)

</details>

<details>

<summary> Diskussion Unterschiede </summary>

In der Auswertung des Diagramms ergab sich eine Beschleunigung von ca. $-11,5 \frac{m}{s^2}$. Der hier berechnete Graph nutzt als Beschleunigung $-9,81 \frac{m}{s^2}$.

</details>

<details>

<summary> Korrektur </summary>

![Loesung_x_y_11.5](https://diversewolken.ddns.net/nextcloud/index.php/s/MStYLTsW2CfQ27a/download "Darstellung der experimentellen x-y-Graphen (exp), der theoretischen x-y-Graphen mit Beschleunigung $g=-9,81\frac{m}{s^2}$ (theor_9.81) und der theoretischen x-y-Graphen mit Beschleunigung $a=-11,5\frac{m}{s^2}$ (theor_11.5)")

</details>

</div>

## Simulation: Die Momentangeschwindigkeit


<iframe src="https://www.geogebra.org/classic/gcs9yuyv?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

---

{{1-2}}
**********
__Beispiel: x(t) und v(t) mit Ansteigsdreieck:__

<iframe src="https://www.geogebra.org/classic/kpmbbr8v?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
**********
---

{{2}}
**********
__Beispiel: x(t) und v(t) mit Anstiegsdreieck (mit Zoom)__

<iframe src="https://www.geogebra.org/classic/gpbcwtqx?embed" width="100%" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
**********

### Übung: Zuordnung Graphen

<p class="newspaper">

Gegeben sind folgende v(t)-Graphen für 7 verschiedene Fälle.

![Faelle_vt](https://diversewolken.ddns.net/nextcloud/index.php/s/L8Y8XrqrZpBX6Tt/download)

<p class="cb">

Ordne im folgenden Bild die x(t) Fälle den v(t) Fällen zu.

<iframe src="https://learningapps.org/watch?v=pd58g8qzt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

</p>

</p>

## 3.7 Die Momentangeschwindigkeit

![Tafelbild_Momentangeschwindigkeit](https://diversewolken.ddns.net/nextcloud/index.php/s/2gC5MmDGj7DoSqy/download)


### Übung: Zuordnung Graphen

<p class="newspaper">

Gegeben sind folgende v(t)-Graphen für 7 verschiedene Fälle.

![Faelle_vt](https://diversewolken.ddns.net/nextcloud/index.php/s/L8Y8XrqrZpBX6Tt/download)

<p class="cb">

Ordne im folgenden Bild die x(t) Fälle den v(t) Fällen zu.

<iframe src="https://learningapps.org/watch?v=pd58g8qzt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

</p>

</p>


### Abituraufgabe 1 Bewegungsvorgänge

1. 1. Ein Pkw fährt auf der Autobahn mit der konstanten Geschwindigkeit von 130 km/h. In der Entfernung von 200 m nimmt der Fahrer die elektronische Verkehrsleiteinrichtung wahr, die die Höchstgeschwindigkeit 80 km/h vorschreibt und auf einen Unfall hinweist. Nach der Reaktionszeit 0,8 s betätigt der Fahrer die Bremse. Die Verzögerung erfolgt gleichmäßig. Der Pkw erreicht exakt beim Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit. <br> Zeichnen Sie ein s(t)- und ein v(t)-Diagramm für den Zeitraum vom Erkennen der Anzeige bis zum Passieren der Verkehrsleiteinrichtung. Berechnen Sie die notwendige Bremsbeschleunigung und die Bremszeit. (5BE)

---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Reaktionsweg: $s_{R}$, 28.9 , $m$)

@rangeQuiz2(Bremsweg: $s_{brems}$, 171.1 , $m$)

---

__Endergebnisse:__

@rangeQuiz2(Bremsbeschleunigung: $a_{brems}$, -2.4 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.9 , $s$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

Es liegen zwei Bewegungsabschnitte vor: Innerhalb der Reaktionszeit $t_R= 0,80 s$ erfolgt die Bewegung zunächst geradlinig gleichförmig mit der Anfangsgeschwindigkeit $v_0 = 130 km/h$. Während des zweiten Abschnittes verringert sich die Geschwindigkeit während der Bremszeit $t_B$_ linear bis zur vorgeschriebenen Höchstgeschwindigkeit $v_H = 80 km/h$.

</details>

<details>

<summary> Hinweis 2 </summary>

Im v-t-Diagramm wird also zunächst wegen der Konstanz der Geschwindigkeit wäh­rend der Reaktionszeit eine Parallele zur Abszissenachse gezeichnet, anschließend ein Stück einer fallenden Geraden. <br> Im s-t-Diagramm erscheint zunächst eine steigende Gerade, die in eine nach unten geöffnete Parabel übergeht. Der Anstieg dieses Parabeiabschnittes verringert sich, darf aber am Ende noch nicht den Scheitel dieser Parabel erkennen lassen.<br> Beachten Sie: Es gilt v = Also entspricht im s-t-Diagramm dem steigenden Parabei­stück mit abnehmendem Anstieg im v-t-Diagramm die fallende Gerade. Und da die
Geschwindigkeit am Ende des zweiten Abschnittes nicht Null beträgt, befindet sich ent­sprechend am Ende des Parabeiastes noch nicht der Scheitel!

</details>

<details>

<summary> Lösung Diagramme </summary>

![Diagramm_L_1.2](https://diversewolken.ddns.net/nextcloud/index.php/s/F8LAqziiJ2HTBiQ/download)

</details>

<details>

<summary> Hinweis 3: Berechnungen </summary>

Wir betrachten hier __lediglich den Bremsvorgang__. Für den Bremsweg $s_{Brems}$ ergibt sich 171,1 m. Die Geschwindigkeit verringert sich von 36,1m/s (130 km/h) auf 22,2 m/s (80 km/h). Man stellt die Bewegungsgleichungen s(t) und v(t) für den Bremsvorgang auf und ermittelt die Unbekannten t und a.

</details>

<details>

<summary> Lösungen: Berechnungen </summary>

Allgemein:

$$ s(t) = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t $$

$$ v(t) = a \cdot t + v_0 $$

Eingesetzt bedeutet das:

$$ 171,1 m = \frac{1}{2} \cdot a \cdot t^2 + 36,1\frac{m}{s} \cdot t $$

$$ 22,2 \frac{m}{s} = a \cdot t + 36,1 \frac{m}{s} $$

Der CAS bietet als Lösungen: $a=-2,38 \frac{m}{s^2}$ und $t=5,87 s$.

</details>



</div>

---

1. 2. Der Fahrer hält nach dem Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit 80 km/h zunächst ein. Durch das Geschehen an der Unfallstelle abgelenkt, bemerkt er jedoch ein 30 m vor ihm mit der Geschwindigkeit 30 km/h gleichförmig fahrendes Fahrzeug sehr spät. Er leitet nach Reaktionszeit 1,0 s eine Vollbremsung ein. Die Verzögerung erfolgt wiederum gleichmäßig. Berechnen Sie die Bremsverzögerung, die mindestens notwendig wäre, um einen Auffahrunfall zu vermeiden. Ein Ausweichen ist nicht möglich. (3BE)


---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Abstand nach Reaktion: $s_{A}$, 16.1 , $m$)

---

__Endergebnisse:__

@rangeQuiz2(minimale Bremsbeschleunigung: $a'$, -6 , $\frac{m}{s^2}$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

![H1_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/pjQocKxARbQKKi6/download)

</details>

<details>

<summary> Hinweis 2 </summary>

![H2_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/HwgKG7CQHTG87rr/download)

</details>

<details>

<summary> Hinweis 3 & Lösung</summary>

![H3_L1.3](https://diversewolken.ddns.net/nextcloud/index.php/s/2HqqGAtQJQz8cfi/download)

</details>

</div>

---

1. 3. Der Unfall war nicht zu verhindern und der Pkw mit der Masse 1,1 t prallte auf das vorausfahrende Fahrzeug mit der Masse 1,8 t. Die Geschwindigkeit des Pkw betrug unmittelbar vor dem Aufprall 40 km/h. Beim Aufprall setzte der Bremsvorgang aus und die beiden Fahrzeuge verhakten sich. Berechnen Sie den Betrag der während des Zusammenstoßes verrichteten Verformungsarbeit. (3BE)

---

<div style="margin-left:10%">

__Zwischenlösungen:__

@rangeQuiz2(Geschwindigkeit nach Zusammenstoß: $v'$, 9.39 , $\frac{m}{s}$)

---

__Endergebnisse:__

@rangeQuiz2(Verformungsarbeit: $W$, 2600 , $J$)

---

__Hilfestellungen:__

<details>


<summary> Hinweis 1 </summary>

Für die gemeinsame Geschwindigkeit $v'$ nach dem Stoß gilt:

$$ v' = \frac{m_1\cdot v_1 + m_2 \cdot v_2}{m_1+m_2} = 9,39 \frac{m}{s} $$

</details>

<details>

<summary> Hinweis 2 </summary>

Der Betrag der Verformungsarbeit $W$ ergibt sich aus der Differenz der kinetischen Energien vor und nach dem Stoß.

$$ W = \frac{1}{2} \cdot m_1 \cdot v_1^2 + \frac{1}{2} \cdot m_2 \cdot v_2^2 - \frac{1}{2} \cdot (m_1+m_2) \cdot v'^2 = 2,6 kJ $$

</details>

</div>


### Abituraufgabe 2 Bewegungsvorgänge

In der Vorbereitungsphase eines Autorennens finden Tests statt. 

2. 1. Zunächst werden die Bremsen des Rennwagens A getestet. Dazu wird der Wagen von 230 km/h auf 80 km/h gleichmäßig abgebremst. Aus den elektronisch über­mittel­ten Daten wird der Bremsweg 240 m bestimmt. <br> Berechnen Sie die Beschleunigung und die Bremszeit. Zeichnen Sie ein zugehöriges s(t)-Diagramm. (6 BE)

---

<div style="margin-left:10%">

__Endergebnisse:__

@rangeQuiz2(Beschleunigung: $a$, -7.5 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.6 , $a$)

---

__Hilfestellungen:__

<details>

<summary> Hinweis 1 </summary>

Wenden Sie die vollständigen Bewegungsgleichungen auf den Rennwagen A an. 

</details>

<details>

<summary> Lösung Diagramm </summary>


![L_Diagramm_H1_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/oZXtydeE2KQgP2p/download)


![L_Diagramm_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/YZAcS83Xd64Nybp/download)

</details>

</div>

---

2. 2. Danach wird der Rennwagen B getestet. Der Rennwagen beschleunigt aus der Ruhe he­r­aus auf die Endgeschwindigkeit $v_1$. Die Geschwindigkeit nimmt linear mit dem zu­rück­gelegten Weg zu. <br> Begründen Sie, dass die Beschleunigung nicht konstant ist. 	(2 BE)


---

<div style="margin-left:10%">


__Hilfestellungen:__

<details>

<summary> Hinweis 1</summary>

![H1_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/BHsxffnyDFjLG5a/download)

</details>

<details>

<summary> Lösung</summary>

![L1_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/RoseCfNeNfHxiwK/download)

</details>

</div>

---

2. 3. Nun werden beide Fahrzeuge gleichzeitig getestet. <br> Rennwagen A und Rennwagen B passieren gleichzeitig ein und denselben Ort mit der Ge­schwindigkeit 180 km/h bzw. 200 km/h. Ab diesem Zeitpunkt ($t = 0$) treten beim Renn­wagen B Motorprobleme auf und dessen Geschwindigkeit sinkt danach ge­mäß der in der Tabelle dargestellten Daten.

<div style="margin-left:10%">

|         |      |      |      |     |     |    |
| t in s  | 0    | 5    | 10   | 15  | 20  | 25 |
| v in m/s| 55,6 | 35,6 | 20,0 | 8,9 | 2,2 | 0  |


Die Geschwindigkeit von Rennwagen A bleibt konstant und er überholt Rennwagen B we­gen dessen Motorschadens. Weisen Sie nach, dass dies etwa nach 2,7 s geschieht. (4BE)

</div>


---

<div style="margin-left:10%">



__Hilfestellungen:__

<details>

<summary> Hinweis 1</summary>

Den Nachweis des Überholens können Sie führen, indem Sie zeigen, dass sich beide Fahrzeuge zum Zeitpunkt $t_Ü = 2,7s$ am gleichen Ort befinden. 

</details>

<details>

<summary> Lösung Teil A</summary>

![L1_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/XqGj6J8W3TTyXF9/download)

</details>

<details>

<summary> Lösung Teil B</summary>

![L2_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/QEBAgfKodnbDHsj/download)

</details>

</div>

### Übung 3. (auf Zeit) - Gleichungssysteme lösen

@timer(30,00)

<p style="margin-right:250px">

<p style="color:blue">

Die folgenden Übungsaufgaben sollen das zügige Lösen von Gleichungssystemen für kinematische Aufgabenstellungen trainieren.
 
Notiere die Bewegungsgleichungen und löse die Aufgabe mit dem CAS. Überprüfe deine Lösungen hier.

</p>

3. 1. Zwei Körper (A und B) beginnen ihre Bewegung zum Zeitpunkt t=0s am Ort x=0m. Körper A führt eine gleichmäßig beschleunigte Bewegung aus mit der Anfangsgeschwindigkeit 0m/s. Körper B bewegt sich gleichförmig. Körper A überholt Körper B nach 100m und 30s. Ermitteln Sie Beschleunigung $a_A$ und die Anfangsgeschwindigkeit $v_{0B}$.

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort A}: 100 m = \frac{1}{2} \cdot a_A \cdot (30s))^2$$

$$ \mathrm{Ort B}: 100 m = v_{0B} \cdot 30s $$

</details>

---

@rangeQuiz2($a_{A}$, 0.222 , $\frac{m}{s^2}$)

@rangeQuiz2($v_{0B}$, 3.33 , $\frac{m}{s}$)

</p>

3. 2. (Aus Abi2) In der Vorbereitungsphase eines Autorennens finden Tests statt. <br> Zunächst werden die Bremsen des Rennwagens A getestet. Dazu wird der Wagen von 230 km/h auf 80 km/h gleichmäßig verzögert abgebremst. Aus den elektronisch über­mittel­ten Daten wird der Bremsweg 240 m bestimmt. <br> Berechnen Sie die Beschleunigung und die Bremszeit.

<div style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort}:  240 m = \frac{1}{2} \cdot a \cdot t^2 + 63,9 \frac{m}{s} \cdot t$$

$$ \mathrm{Geschwindigkeit}: 22,2 \frac{m}{s} = a \cdot t + 63,9 \frac{m}{s} $$

</details>

---

@rangeQuiz2(Beschleunigung: $a$, -7.47 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.57 , $a$)

</div>

---

3. 3. Ein Ball wird aus einer Höhe $h_0 = 5m$ mit einer Anfangsgeschwindigkeit $v_0$ senkrecht nach oben geworfen. Der Ball schlägt mit einer Geschwindigkeit von 15 m/s auf den Boden auf. Reibung wird vernachlässigt. Ermittle Anfangsgeschwindigkeit $v_0$ und Flugzeit $t_{Flug}$. <br> @color(Achte auf die Vorzeichen der Zahlenwerte., red)

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort}:  0 = \frac{1}{2} \cdot -9,81 \frac{m}{s^2}\cdot t^2 + v_0 \cdot t + 5m$$

$$ \mathrm{Geschwindigkeit}: -15 \frac{m}{s} = -9,81\frac{m}{s^2} \cdot t + v_0 $$

</details>

---

@rangeQuiz2($v_0$, 11.265 , $\frac{m}{s}$)

@rangeQuiz2($t$, 2.677 , $s$)

</p>

3. 4. Zwei Motoradfahrer fahren auf geradliniger Strecke. Beide befinden sich wie dargestellt zum Zeitpunkt t=0s an den Markierungen A bzw. B. <br> P ist in Fahrtrichtung 50m von M entfernt. Im Punkt M hat A eine Geschwindigkeit von 90 km/h und verzögert gleichmäßig. Im Punkt P hat B eine Geschwindigkeit von 72 km/h und verzögert gleichmäßig mit 1 m/s². Ermitteln $a_A$ derart, dass A und B zu einem Zeitpunkt dieselbe Geschwindigkeit und denselben Ort haben. Ermittle den zugehörigen Abstand s zwischen B und dem Treffpunkt.

![Pitty_713](https://physikaufgaben.de/bild/a713_1.gif)<!-- style="max-width:80%;margin-left:10%"-->

---

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{A}: x_A(t) = \frac{1}{2}\cdot a_A \cdot t^2 + 25 \frac{m}{s} \cdot t \hspace{1cm} v_A(t) = a_A \cdot t + 25 \frac{m}{s} $$

$$ \mathrm{B}: x_B(t) = \frac{1}{2}\cdot (-1 \frac{m}{s^2}) \cdot t^2 + 20 \frac{m}{s} \cdot t + 50m \hspace{1cm} v_B(t) = (-1 \frac{m}{s^2}) \cdot t + 20 \frac{m}{s}  $$

$$ \mathrm{Setze} : x_A(t) = x_B(t) \hspace{1cm} \mathrm{und} \hspace{1cm} v_A(t) = v_B(t) $$

</details>

---

@rangeQuiz2($a_{A}$, -1.25 , $\frac{m}{s^2}$)

@rangeQuiz2($t$, 20 , $s$)

@rangeQuiz2($s$, 200 , $m$)

</p>

---

3. 5. __(Wdh. Abi 1)__ Ein Pkw fährt auf der Autobahn mit der konstanten Geschwindigkeit von 130 km/h. In der Entfernung von 200 m nimmt der Fahrer die elektronische Verkehrsleiteinrichtung wahr, die die Höchstgeschwindigkeit 80 km/h vorschreibt und auf einen Unfall hinweist. Nach der Reaktionszeit 0,8 s betätigt der Fahrer die Bremse. Die Verzögerung erfolgt gleichmäßig. Der Pkw erreicht exakt beim Passieren der Verkehrsleiteinrichtung die vorgegebene Höchstgeschwindigkeit. <br> Berechnen Sie für den Bremsvorgang die notwendige Bremsbeschleunigung und die Bremszeit.

<p style="margin-left:5%">

__Endergebnisse:__

<details>

<summary> Bewegungsgleichungen </summary>

$$ \mathrm{Ort:} 171,1 m = \frac{1}{2} \cdot a \cdot t^2 + 36,1\frac{m}{s} \cdot t $$

$$ \mathrm{Geschwindigkeit}: 22,2 \frac{m}{s} = a \cdot t + 36,1 \frac{m}{s} $$

</details>

---

@rangeQuiz2(Bremsbeschleunigung: $a_{brems}$, -2.4 , $\frac{m}{s^2}$)

@rangeQuiz2(Bremszeit: $t_{brems}$, 5.9 , $s$)

</p>

</p>

## 3.8 Der zurückgelegte Weg

![Tafelbild_ZurückGelegterWeg1](https://diversewolken.ddns.net/nextcloud/index.php/s/9tGYWwXJPn6ZL5C/download)

![Tafelbild_ZurückGelegterWeg2](https://diversewolken.ddns.net/nextcloud/index.php/s/nesaB4QNpTNKrs8/download)

![Tafelbild_ZurückGelegterWeg3](https://diversewolken.ddns.net/nextcloud/index.php/s/B6qat3Gjn7tA5DG/download)

### Aufgabe 4 - Zurückgelegter Weg

> 4. 1. Zu einer geradlinigen Bewegung gehört das Zeit-Geschwindigkeits-Diagramm der folgenden Abbildung: <br> ![v-t-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/8PB92pbssc5MoMo/download)<!-- style="max-width:80%"-->

> 4. 1. 1. Berechnen Sie die Beschleunigungen in den drei Zeitintervallen.

<p style="margin-left:10%">

@rangeQuiz2($a_1$, 1 , $\frac{m}{s^2}$)

@rangeQuiz2($a_2$, 0.333 , $\frac{m}{s^2}$)

@rangeQuiz2($a_3$, -4 , $\frac{m}{s^2}$)

<details>

<summary> Hinweis 1</summary>

Nutzen Sie die Formel für die gleichmäßig beschleunigte Bewegung 

$$ a = \frac{\Delta v}{\Delta t} $$

</details>

<details>

<summary> Hinweis 2</summary>

Ermitteln Sie für jedes Intervall die Geschwindigkeitsänderung $\Delta v$ und die dafür benötigte Zeit $\Delta t$.

Für $a_1$ gilt: In $\Delta t=2s$ ändert sich die Geschwindigkeit um $\Delta v = 2 \frac{m}{s}$.

</details>

</p>

> 4. 1. 2. Berechnen Sie die Teilwege ($s_1,\, s_2,\, s_3$), sowie den Gesamtweg.

<p style="margin-left:10%">

@rangeQuiz2($s_1$, 4 , $m$)

@rangeQuiz2($s_2$, 10.5 , $m$)

@rangeQuiz2($s_3$, 2 , $m$)

@rangeQuiz2($s_{ges}$, 16.5 , $m$)

<details>

<summary> Hinweis 1</summary>

Der zurück gelegte Weg entspricht der Fläche unter dem v(t)-Graphen.

</details>

<details>

<summary> Hinweis 2</summary>

Ermitteln Sie für die Intervalle geometrisch die Fläche unter den Graphen

</details>

<details>

<summary> Lösung $s_1$</summary>

Die Fläche ergibt sich aus einem Rechteck ($2s\cdot 1\frac{m}{s}=2m$) und einem rechtwinkligen Dreieck ($\frac{1}{2}$2s\cdot 2\frac{m}{s}=2m$). Somit ergibt sich $s_1=4m$



</details>

</p>



> 4. 2. ![Dragster](https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/NOX_2019_TF_MajaUdtjan.jpg/330px-NOX_2019_TF_MajaUdtjan.jpg) Beim Dragster-Rennen ist es das Ziel, eine Strecke von 1/4 Meile (402,34m) aus dem Stand in möglichst kurzer Zeit zu überwinden. Die Fahrzeuge beschleunigen dabei durchgängig und es treten nicht gleichmäßig beschleunigte Bewegungen auf. <br> Das Fahrzeug beginnt seine Bewegung zum Zeitpunkt t=0s am Ort s=0m. Für den deutschen Rekord ($t_{ges}=7,34s$), soll der Geschwindigkeits-Zeit-Graph mit folgender Funktion näherungsweise beschrieben werden:
>
> $$ v(t) = -1,125\frac{m}{s^3}\cdot t^2 + 20,44 \frac{m}{s^2} \cdot t $$

---

> 4. 2. 1. Ermitteln Sie die Endgeschwindigkeit in der Einheit $\frac{km}{h}$.

<p style="margin-left:10%">

@rangeQuiz2($v_{end}$, 321.91, $\frac{km}{h}$)

<details>

<summary> Hinweis 1</summary>

Die Geschwindigkeit, welche nach der Zeit $t_{ges}$ erreicht worden ist.

</details>

<details>

<summary> Hinweis 2</summary>

Setzen Sie die $t_{ges}$ in die Formel für die Geschwindigkeit ein.

</details>

</p>

---

> 4. 2. 2. Ermitteln Sie einen Ausdruck für a(t).

<p style="margin-left:10%">

<details>

<summary> Hinweis 1</summary>

Die Beschleunigung a(t) ist definiert als die Ableitung der Geschwindigkeit nach der Zeit t.

</details>

<details>

<summary> Hinweis 2 / Lösung</summary>

Leiten Sie die Funktion $ v(t) = -1,125\frac{m}{s^3}\cdot t^2 + 20,44 \frac{m}{s^2} \cdot t $ nach der Zeit ab.

$$\frac{\mathrm{d} v}{\mathrm{d} t} = -2.25\frac{m}{s^3}\cdot t + 20,44 \frac{m}{s^2} $$

$$ \boxed{a(t)=-2.25\frac{m}{s^3}\cdot t + 20,44 \frac{m}{s^2}} $$

</details>

</p>

> 4. 2. 3. Begründen Sie anhand der Lösung von 4.2.2. dass es sich nicht um eine gleichmäßig beschleunigte Bewegung handeln kann.

<p style="margin-left:10%">

<details>

<summary> Hinweis 1</summary>

Überprüfen Sie, ob die Beschleunigung konstant ist.

</details>

<details>

<summary> Hinweis 2 / Lösung</summary>

Der Graph der Beschleunigung ist eine lineare Funktion mit einem Anstieg -2,25, daher ist die Beschleunigung nicht konstant, sondern sinkt.

$$ \boxed{a(t)=-2.25\frac{m}{s^3}\cdot t + 20,44 \frac{m}{s^2}} $$

</details>

</p>

> 4. 2. 4. Zeigen Sie näherungsweise, dass das Fahrzeug nach 7,34s die Vierteilmeilendistanz überwunden hat.

<p style="margin-left:10%">

<details>

<summary> Hinweis 1</summary>

Die zurückgelegte Strecke s entspricht der Fläche unter dem v(t)-Graph.

</details>

<details>

<summary> Hinweis 2 </summary>

Nutzen Sie den CAS um zu zeigen, näherungsweise folgendes gilt:

$$ \int_0^{7,34s}{v(t)dt}=402,32m $$

</details>

<details>

<summary> Lösung </summary>

$$ \int_0^{7,34}{(-1,25\cdot t^2+20,44\cdot t) dt}=402,34 $$

</details>

</p>

> 4. 2. 5. Ermitteln Sie Strecke und Geschwindigkeit, die nach 4,88s erreicht wurden.

<p style="margin-left:10%">

@rangeQuiz2($v$, 72.956 ,$\frac{m}{s}$)

@rangeQuiz2($s$, 199.8 ,$m$)

</p>

### Abituraufgabe Baustellenfahrten

@timer(05,00)

@timer2(35,00)

<p style="margin-right:200px">

Auf Autobahnen kommt es wegen Baustellen zu Geschwindigkeitsbegrenzungen und
Veränderungen der Verkehrsführung. Dabei kann z. B. eine Richtungsfahrbahn geteilt
und ein Fahrstreifen auf die Gegenfahrbahn geführt werden.

Die Bewegung der Fahrzeuge auf der Autobahn wird modellhaft durch die Bewegung
von Massepunkten auf einer horizontalen Ebene vereinfacht.
Die Abbildung zeigt das Prinzip der Verkehrsführung.

![Abituraufgabe_Baustelle](https://diversewolken.ddns.net/nextcloud/index.php/s/7ye8j9Wn6JAd9G9/download)

Die Geschwindigkeitsbegrenzung für den Fahrstreifen auf der Richtungsfahrbahn Ost beträgt 60km∙h⁻¹, auf den anderen drei Fahrstreifen gilt die Höchstgeschwindigkeit 80km∙h⁻¹. Die Geschwindigkeitsbegrenzung gilt jeweils auf beiden Richtungsfahrbahnen in Fahrtrichtung ab dem Anfang des Baustellenbereichs.

_Hinweis:_ Der von den Fahrzeugen im Baustellenbereich zurückgelegte Weg ist geringfügig länger als 1400m, die zugehörige Differenz darf vernachlässigt werden.

Ein Lieferwagen (Lw) fährt in Richtung Osten mit der konstanten Geschwindigkeit 60 km∙h⁻¹. Zum Zeitpunkt t=0 wird er am Beginn des Baustellenbereichs von
einem Pkw überholt, welcher die zweite Fahrspur (Überholspur) befährt.
Der Fahrer des Pkw hält sich nicht an die Geschwindigkeitsbegrenzung und fährt zu diesem Zeitpunkt mit der Geschwindigkeit 110km∙h⁻¹, er bremst das Fahrzeug sofort gleichmäßig auf 80 km∙h⁻¹ ab und legt dabei 200m zurück.

---

1. 1. Ermitteln Sie die Beschleunigung des Pkw beim Abbremsen und die Bremszeit.

<p style="margin-left:10%">

@rangeQuiz2($t_{brems}$, 7.579 , $s$)

---

@rangeQuiz2($a_{Pkw}$, -1.1, $\frac{m}{s^2}$)

---

<details>

<summary> Hinweis 1</summary>

Stellen Sie die Bewegungsgleichungen $s(t)$ und $v(t)$ für den Pkw auf, setzen Sie bekannte Werte ein und lösen Sie das Gleichungssystem mit dem CAS.

</details>

---

<details>

<summary> Hinweis 2 </summary>

Für s(t) gilt: $200m = \frac{1}{2} \cdot a \cdot t^2 + \frac{110}{3,6} \frac{m}{s} \cdot t$

Für v(t) gilt: $\frac{80}{3,6}\frac{m}{s} = a \cdot t + \frac{110}{3,6}\frac{m}{s}$

</details>

---

<details>

<summary> Lösung </summary>

$ t = 7,579 s$

$a = -1,1 \frac{m}{s^2}$

</details>

</p>

---

1. 2. Der Pkw bewegt sich 200 m nach Beginn des Baustellenbereichs gleichförmig mit der Geschwindigkeit 80 km∙h⁻¹ . Er passiert zum Zeitpunkt $t_1$ das Ende des Baustellenbereichs. Ermitteln Sie den Abstand von Lieferwagen und Pkw für den Zeitpunkt $t_1$.

<p style="margin-left:10%">

__Zwischenergebnis:__

@rangeQuiz2($t_{1}$, 61.579 , $s$)

---

__Endergebnis:__

@rangeQuiz2($s_{Pkw-Lw}$, 373.68 , $m$)

---

<details>

<summary> Hinweis 1</summary>

Stellen Sie die Bewegungsgleichungen $s_{Pkw}(t)$ für die Bewegung nach dem Bremsvorgang auf. Ermitteln Sie die Zeit $t'$, die der Lieferwagen für die gleichförmige Bewegung der Reststrecke benötigt.

@rangeQuiz2($t'$, 54 , $s$)

</details>

---

<details>

<summary> Hinweis 2 </summary>

Für die gleichförmige Bewegung des Pkw gilt:

$$ 1400 m = \frac{80}{3.6}\frac{m}{s}\cdot t' + 200 m $$

$$ t' = 54s $$.

Diese Zeit muss zu der Bremszeit hinzugefügt werden um den Zeitpunkt $t_1$ zu berechnen.

</details>

---

<details>

<summary> Lösung </summary>

$ t_1 = 61,579s $

Der Lieferwagen führt ebenfalls eine gleichförmige Bewegung aus.

$ s_{Lw}(t) = \frac{60}{3.6}\frac{m}{s} \cdot t $

Setzt man hier die Zeit $t_1 = 61,579s$ ein, so ergibt sich der Weg des Lw zu 1026,32m. Somit ist der Abstand der Fahrzeuge 373,68 m.

</details>

</p>

---

1. 3. Auf der Richtungsfahrbahn West hat sich ein Stau wegen eines defekten Lkw gebildet. Der defekte Lkw steht genau in der Mitte des Baustellenbereichs und blockiert die beiden nördlichen Fahrstreifen. Ein Fahrzeug des Pannendienstes (Pd) durchfährt die Rettungsgasse mit der konstanten Geschwindigkeit 25km∙h⁻¹. Zum Zeitpunkt t=0 ist es noch 500 m von dem defekten Lkw entfernt. <br> Ermitteln Sie den Abstand $s_2$ vom defekten Lkw, wo sich Pd und Lw treffen.

<p style="margin-left:10%">

__Zwischenergebnis:__ (Treff-Zeitpunkt von Pd und Lw)

@rangeQuiz2($t_2$, 50.82, $s$)

__Endergebnis:__ Abstand von Lkw und Lw/Pd-Treffpunkt

@rangeQuiz2($s_2$, 147 , $m$)

<details>

<summary> Hinweis 1</summary>

Stellen sie für den Pd und den Lw die Bewegungsgleichungen s(t) auf und setzen Sie diese gleich. Achten Sie auf die Vorzeichen der Geschwindigkeiten und eventuelle Parameter $s_0$.

</details>

---

<details>

<summary> Hinweis 2 </summary>

Beide Fahrzeuge bewegen sich gleichförmig aufeinander zu.<br> Für den Lw: $s_{Lw}(t) = \frac{60}{3,6}\frac{m}{s} \cdot t$ <br> und für den Pd: $s_{Pd}(t) = -\frac{25}{3,6}\frac{m}{s}\cdot t + 1200m$

</details>

---

<details>

<summary> Lösung </summary>

Setzt man $s_{Lw}(t_2) = s_{Pd}(t_2)$ so ergibt sich als Lösung

$$ t_2 = 50,82s $$

Der Lw hat zu diesem Zeitpunkt $t_2$ die Strecke

$$ s_{Lw}(t_2) = 847 m $$

zurück gelegt. Der Abstand zum defekten Lkw beträgt demnach

$$ s_{2} = 847 m - 700 m = 147 m$$

</details>

</p>



## 3.9 Demonstationsexperiment - Waagerechter Wurf

![Tafelbild_WaagerechterWurf1](https://diversewolken.ddns.net/nextcloud/index.php/s/Non6oniz9pCTxST/download)

![Tafelbild_WaagerechterWurf2](https://diversewolken.ddns.net/nextcloud/index.php/s/L5JtoxPf4SE8ZoJ/download)

__Wurfparabeln: Experiment (Viana2) vs. Bewegungsgleichgung__

<p class="newspaper">

![Wurfparabeln](https://diversewolken.ddns.net/nextcloud/index.php/s/eLP2B5Aa4oxPmBY/download)<!-- style="width:100%"-->

<p class="cb">

- gemessene Wurfparabel y(x) und aus Startwerten berechnete Parabel y(x) stimmen gut überein 

- Abweichungen können auf Messunsicherheiten und nicht berücksichtigte Kräften (z.B. Luftreibung) zurück geführt werden

</p>

</p>

## 3.10 Herleitung der Wurfparabel y(x) für waagerechten Wurf

![Tafelbild_HerleitungWp](https://diversewolken.ddns.net/nextcloud/index.php/s/eWNsWrs6NSEgxPG/download)

## 3.11 Zerlegung des Geschwindigkeitsvektors für den waagerechten Wurf

![Tafelbild_ZerlegungV](https://diversewolken.ddns.net/nextcloud/index.php/s/NGJLZ9ifYLfEeyR/download)

### Aufgaben Wurfbewegungen

__Routine Metzler S. 31 / 1__

<details style="margin:5%">

<summary> Lösung </summary>

<br>
Für $v_0 = 5\frac{m}{s}$:

| t /s     | $x_{t}$ / m| $y(t)$ / m |
| 0,1      | 0,5        | 0,05       |
| 0,5      | 2,5        | 1,23       |
| 1        | 5          | 4,91       |
| 1,5      | 7,5        | 11,04      |
| 2        | 10         | 19,62      |  

<br>

Für $v_0 = 10\frac{m}{s}$:

| t /s     | $x_{t}$ / m| $y(t)$ / m |
| 0,1      | 1        | 0,05       |
| 0,5      | 5        | 1,23       |
| 1        | 10        | 4,91       |
| 1,5      | 15        | 11,04      |
| 2        | 20        | 19,62      | 

<br>

_Diagramm:_

![Lsg_Metzler_S31_1](https://diversewolken.ddns.net/nextcloud/index.php/s/PzJen3Nsxcefxjx/download)



</details>


---

__Metzler S. 31 / 3__

<p style="margin:5%">

a) Überprüfen

@rangeQuiz2($h$, 19.62 ,$m$)

@rangeQuiz2($t_{flug}$, 2 , $s$)

---

b)

@rangeQuiz2($v_{end}$, 28.02 ,$\frac{m}{s}$)

@rangeQuiz2($\alpha$, 44.45 , $^\circ$)

---

c) 

<details>

<summary> Lösung allgemein </summary>

zu a)

$$ h = \frac{g\cdot x^2_E}{2v_0^2}  $$

$$ t_{flug} = \sqrt{\frac{2h}{g}}  $$

oder 

$$ t_{flug} = \frac{x_E}{v_0} $$

zu b)

$$ v = \sqrt{v_0^2+(g\cdot t)^2} $$

$$ \tan \alpha = \frac{g \cdot t}{v_o} $$

</details>

</p>

---

__Metzler S. 31 / 4__

<p style="margin:5%">

a) Überprüfen

@rangeQuiz2($v_{0}$, 17.29 ,$\frac{m}{s}$)

---

b)

@rangeQuiz2($h$, 6.29 , $m$)

---

c)

@rangeQuiz2($t$, 2.27 , $s$)


---

<details>

<summary> Hinweise zur Lösung </summary>

![Lsg_Metzler_S31_4](https://diversewolken.ddns.net/nextcloud/index.php/s/rPEmDFpYi7DtoW9/download)

_Hinweise zum CAS: cos(40) und sin(40) ausrechnen und in Gleichung eingeben _

![Lsg_Metzler_S31_4_CAS](https://diversewolken.ddns.net/nextcloud/index.php/s/7sDfT3gi3s6jCoL/download)


</details>

</p>

---

__Metzler S. 31 / 5__

<p style="margin:5%">

<details>

<summary> Lösung allgemein </summary>

$$ \mathrm{(I)\ \ \ } x = v_0 \cdot \cos\alpha \cdot t $$

$$ \mathrm{(II)\ \ \ } y = \frac{1}{2}\cdot g \cdot t^2 + v_0 \cdot \sin\alpha \cdot t$$


_Stelle Glg. (I) nach t um:_

$$ t = \frac{x}{v_0 \cdot \cos\alpha} $$

_Setze t in Glg. (II) ein:_

$$ y = \frac{1}{2}\cdot g \cdot \red{\Big(\frac{x}{v_0 \cdot \cos\alpha}\Big)^2} + v_0 \cdot \sin\alpha \cdot \red{\Big(\frac{x}{v_0 \cdot \cos\alpha}\Big)}$$

$$ \boxed{y = \frac{1}{2} \cdot \frac{g}{(v_0 \cdot \cos\alpha)^2} \cdot x^2 + \tan\alpha \cdot x}$$

</details>

</p>


---

__Metzler S. 31 / 6*__

<p style="margin:5%">

a) Überprüfen

@rangeQuiz2($h$, 2.04 ,$m$)

---

b)

@rangeQuiz2($v_0$, 13.01 , $\frac{m}{s}$)

---

<details>

<summary> Lösung allgemein </summary>

$$ v_0 = \frac{b}{\cos\alpha}\cdot\sqrt{\frac{g}{2(b\tan\alpha-h)}} $$


__Umformung:__



</details>


</p>

### Game Wurfparabel

??[WurfGame](https://www.geogebra.org/classic/w3y2kjzp?embed)