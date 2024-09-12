<!--
author: Christian Golnik

language: de

@style
.lia-effect__circle {
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

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Physik LK Script und Aufgaben

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


## 2.7 Reibungsarbeit

> $W_R = F_R \cdot s$


> mit:
>
> $\hspace{0.5cm}$ $W_R$ .. Reibungsarbeit in $[N]$
>
> $\hspace{0.5cm}$ $F_R$ .. Reibungskraft in $[N]$
>
> $\hspace{0.5cm}$ $s$ .. zurückgelegter Weg in $[m]$

{{1}}
*************
>> Die durch Reibungsarbeit umgwandelte Energie wird in vielen Fällen in Innere Energie umgewandelt (z.B. Wärme).Man sagt sie wird dadurch _entwertet_ (d.h. schlecht nutzbar).
*************