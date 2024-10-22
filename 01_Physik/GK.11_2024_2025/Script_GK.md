
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

@color
<bdi style="color:@1">@0</bdi>
@end

@align
<p style="text-align: @1">@0</p>
@end

@indent
<div style="text-indent:@1">@0</div>
@end

@onload
window.LIA.settings.font_size = 2
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


@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Grundkurs Physik 2024/2025 - Skript

@uhr

# LB I - Mechanische Grundlagen

## 1.1 - Wiederholung Energieformen

__Energie__

{{1}}
*****************
> Definition: Energie beschreibt die Fähigkeit eines Körpers:
*****************
{{2}}
*****************
>- mechanische Arbeit zu verrichten (z.B. Beschleunigen oder Verformen eines Körpers)
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
>- Spannenergie (z.B. Feder, Bungeeseil)

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

## 1.2 Berechnung der kinetischen Energie

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

## 1.3 Berechnung der potentiellen Energie

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

## Arbeitsblatt: Energieformen

Übung 3: _Ergänze mit Hilfe des Tafelbildes folgendes Arbeitsblatt

1. Ergänze die Energieumwandlung der Achterbahn von $\textcircled{A}$ bis $\textcircled{D}$

2. Notiere die Berechnungsformeln der Energiformen $\textcircled{B}$ und  $\textcircled{C}$ ( $\textcircled{A}$ optional mit TW)

3. Ergänze die physikalischen Größen mit Name und Einheit

> ![EnergieformenA](https://diversewolken.ddns.net/nextcloud/index.php/s/3JrTCX9NRJegMnP/download)

## Lösung Arbeitsblatt Energieformen

Überprüfe die Lösung mit deinen Aufzeichnungen.

> ![EnergieformenLösung](https://diversewolken.ddns.net/nextcloud/index.php/s/yLXRoPQ8iWkni4b/download)


## 1.4. Demonstrationsexperiment Senkrechter Wurf 

__Beispiel zu Energieumwandlungen__

Beschreibung: Eine Stahlkugel wird mit Hilfe eine gespannten Feder senkrecht nach oben geschossen. Wir beschreiben diesen Versuch an drei spezifischen Punkten.

{{1}}
*************
__Versuchsaufbau:__

![Tafelbild_SenkrechterWurf](https://diversewolken.ddns.net/nextcloud/index.php/s/ac7aBYYk5sDojLN/download)
*************

{{2}}
*************
__Qualitative Analyse der Energieerhaltung:__

_Hinweis: Qualitativ bedeutet ohne Berechnung_

![Tafelbild_AnalyseEnergieerhaltung](https://diversewolken.ddns.net/nextcloud/index.php/s/y5X8EFstJe6AdwB/download)
*************


## 1.5 Messwerte und Berechnungen Senkrechter Wurf



{{1}}
*************
__Messwerte:__

![Tafelbild_MesswerteSenkrechterWurf](https://diversewolken.ddns.net/nextcloud/index.php/s/bxW7ffp28WKc8Gp/download)
*************

{{2-3}}
*******************
!?[SenkrechterWurf_Videoanalys](https://youtu.be/XVEjzYdc3rk)
*******************

{{3}}
*************
__Aufgabenstellung und Berechnungen:__

> 1. Bestimme die Masse der Kugel

> 2. Filme mit einem Smartphone den Flug der Kugel und bestimme die maximale Höhe $h_2$

> 3. Berechne für die Zustände 1,2 & 3 die Spannenergie der Feder, die potentielle Energie der Kugel und die kinetische Energie der Kugel.

Ergänze dazu die Tabelle:

| | | | |
| Nr. | $E_{sp}$ in J | $E_{pot}$ in J | $E_{kin}$ in J |
| 1 | | | |
| 2 | | | |
| 3 | | | |

> 4. Bestimme $v_3$, die Geschwindigkeit der Kugel am Punkt 3.

*************

{{4}}
***********
__Lösungsvorschlag:__

![Berechnung_Geschwindigkeitv3](https://diversewolken.ddns.net/nextcloud/index.php/s/A76awi56xDgSFmP/download)
***********

## 1.6 Energiebetrachtung unter Berücksichtigung von Reibung

## 1.7 Aufgabe

Ein Pkw fährt mit der Geschwindigkeit $72 \frac{km}{h}$. Zum Zeitpunkt t=0, am Ort s=0 betätigt der Fahrer die Kupplung, dadurch wirkt die Antriebskraft nicht mehr auf das Fahrzeug, ab diesem Moment wird die Bewegung für zwei verschiedene Fälle untersucht:

- 1. Im Fall 1 bewegt sich das Fahrzeug eine Straße mit dem Neigungswinkel 5,0° gegenüber der Horizontalen bis zum Stillstand aufwärts. Berechnen Sie den zurückgelegten Weg. Nutzen Sie den Energieerhaltungssatz. <br> _Hinweis: Die Reibung bleibt unberücksichtigt._
- 2. Im Fall 2 bewegt sich das Fahrzeug auf einer horizontalen Straße unter dem Einfluss der Reibung bis zum Stillstand. Berechnen Sie den zurückgelegten Weg. <br> _Hinweis: Die konstante Reibungszahl beträgt 0,12_ .



## 1.8 Einführung in das Thema Reibung

### 1.8.1 Definition Reibung

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

### 1.8.2 Die Reibungszahl $\mu$ - Berechnung der Reibungskraft

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

_Aufgaben 1.8.5_

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

_Aufgabe: siehe 1.8.4_

********

### 1.8.3 Zusammenfassung

Reibung ist eine fundamentale Kraft in der Physik, die der Bewegung zwischen zwei Oberflächen entgegenwirkt. Sie kann in Haft-, Gleit- und Rollreibung unterteilt werden. Die Berechnung der Reibungskraft erfolgt durch die Multiplikation des Reibungskoeffizienten mit der Normalkraft.

### 1.8.4 Qualitative Übung zur Reibung (ohne Berechnungen)

Diskutiere mit einem Partner. Stellt euch Wechselseitig die Fragen und überprüft die Antworten.

__Empfehlung: Aufgaben 113-117__

??[PittysPhysik](https://physikaufgaben.de/aufgaben_zeige_an.php?thid=1&tab=6&auswahl_t1=13&auswahl_n1=4)

### 1.8.5 Quantitative Übung zur Reibung (mit Berechnungen)

_Quantitative Aufgaben zur Reibung auf horizontalen Ebene. Bitte anklicken und allein oder in Gruppenarbeit berechnen und Lösung vergleichen._

[Leifi-Physik-Aufgabe-Reibung-1](https://www.leifiphysik.de/mechanik/reibung-und-fortbewegung/aufgabe/wohnanhaenger)

[Leifi-Physik-Aufgabe-Reibung-2](https://www.leifiphysik.de/mechanik/reibung-und-fortbewegung/aufgabe/die-verrueckte-kiste)

## 1.9 Kräfte

### 1.9.1 Defintion Kraft

Kräfte erkennt man an ihrer Wirkung. Die Wirkung von Kräften kann sein:

{{1}}
**************************
1. Ein Körper ändert seine Bewegungsform (d.h. Geschwindigkeit oder Bewegungsrichtung).

2. Ein Körper verformt sich.

3. Beides gleichzeitig.
**************************

### 1.9.2 Newtonsche Gesetze

<H3>Newton'sche Gesetze</H3>

{{1}}
**************
1. Ein kräftefreier Körper bleibt in Ruhe oder bewegt sich geradlinig mit konstanter Geschwindigkeit. <br> 
$\hspace{1cm}$ __Beispiel:__ {2}{![VoyagerSone](https://heise.cloudimg.io/width/1220/q70.png-lossy-70.webp-lossy-70.foil1/_www-heise-de_/imgs/18/3/5/4/6/9/3/7/Voyager-illustration-with-stars-16.jpg-e02f3b734d477d20.jpeg) Sonde ohne Antrieb im Weltall}
**************

<br>
<br>

{{3}}
**************************
2. Kraft gleich Masse mal Beschleunigung

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
3. Kraft gleich Gegenkraft (Wechselwirkungsgesetz)

> Eine Kraft von Körper A auf Körper B geht immer mit einer gleich großen, aber entgegen gerichteten Kraft von Körper B auf Körper A einher
**************************
{{6}}
********
$\hspace{1cm}$ __Beispiel:__ ![Gegenkraft](https://av.ph.nat.tum.de/Experiment/1000/Grafik/b1105.gif) 

********

### 1.9.3 Darstellung von Kräften

> Die Kraft ist eine __vektorielle physikalische Größe__, d.h. sie hat einen Wert (Betrag __und eine Richtung__).

_Darstellung: Kräfte (i.a. Vektorgrößen) werden mit Pfeilen dargestellt. Die Länge des Pfeils entspricht dem Wert. Die Richtung des Pfeils gibt die Wirkrichtung der Kraft an._

__Beispiel:__ Gewichtskraft $F_g$ mit Gegenkraft der Unterlage $F_U$ (3. Newton'sches Gesetz)

![GewichtskraftGegenkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/WDBCJmyZ7Q4jkrK/download)

### 1.9.4 Superposition von Kräften

> Unter der Superposition von Kräften versteht man das gleichzeitige Wirken mehrerer Kräfte. Durch Addition der Kraftpfeile kann die resultierende __Gesamtkraft $F_{ges}$__ ermittelt werden.

{{1}}
**********
__Beispiel 1:__  Ruhender Körper auf horizontaler Ebene(siehe 1.9.3)

![GewichtskraftGegenkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/WDBCJmyZ7Q4jkrK/download)
_Gewichtskraft $F_g$ und Gegenkraft $F_U$ haben den gleichen Wert (3. Newton'sches Gesetz) wirken aber in entgegen gesetzte Richtung und heben sich gegenseitig auf._ 

__=> Resultierende Kraft $F_{ges}$ ist Null, der Körper ruht (1. Newton'sches Gesetz)__
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
__Beispiel 3:__ Kräfteaddition allgmein

{4-5}{![Kräfte_Allg_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9f2c7SWt66wH2R7/download)}{5}{![Kräfte_Allg_2](https://diversewolken.ddns.net/nextcloud/index.php/s/ZwdPTzyYjoj2jaL/download)} _Wirken zwei Kräfte in beliebigen Richtungen auf denselben Körper, so addiere die Kraftpfeile durch $\textbf{Parallelverschieben}$ des Ursprungs eines Pfeils in die Spitze des anderen Pfeils. Die Gesamtkraft entsprich der Diagonale des entstandenen Parallelogramms._

__=> Gesamtkraft $F_{ges}$ kann mit Richtung und Wert geometrisch bestimmt werden.__
**********

### Aufgaben zum Thema Kräfte

![Aufgabe1](https://diversewolken.ddns.net/nextcloud/index.php/s/eEqaeWXtm6GDc9i/download)

<details>

<summary>Lösung 1 _(Hinweise für 1b findest du in 1.9.5)_ </summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/WBPp9mREz4zzdqS/download)

</details>



### 1.9.5 Kraftzerlegung an der schiefen Ebene

> __Hinweis Kräfte-Zerlegung__: Eine Gesamtkraft kann man gedanklich in Teilkräfte zerlegen, deren Addition wieder die Gesamtkraft ergibt. <br> Im Beispiel der schiefen Ebene zerlegt man die Gewichtskraft ($F_g$) in eine Teilkraft senkrecht zur Ebene ($F_N$) und eine Teilkraft parallel zur Ebene ($F_H$)

<br>

![Aufgabe_Schiefe_Ebene](https://diversewolken.ddns.net/nextcloud/index.php/s/D8zbKHyyT7xJPBz/download) An einer schiefen Ebene mit dem Neigungswinkel $\alpha$ lässt sich die Gewichtskraft $F_g$ in eine Normalkraft $F_N$ (senkrecht zur Ebene) und eine Hangabtriebskraft $F_H$ (parallel zur Ebene) zerlegen.

_Aufgabe 2: Zeichne diese Kraftzerlegung in deinen Hefter. Konstruiere anschließend folgendes Beispiel: Auf einer schiefen Ebene (30°) ruht ein Körper mit der Gewichtkraft 3000 N._ 

1. _Bestimme grafisch oder durch Berechnung die Normalkraft $F_N$_ und die Hangabtriebskraft $F_H$.

2. _Die Unterlage und Körper haben eine Haftreibungszahl $\mu_{Haft} = 0,4$ (s. 1.8.2). Bestimme die Haftreibungskraft auf der Unterlage._

3. _Ist die Hangabtriebskraft größer als die Reibungskraft, so beginnt der Körper zu rutschen. Überprüfe, ob sich der Körper bewegt._

4. _*Der Neigungswinkel $\alpha$ wird nun so verändert, sodass der Körper gerade noch ruht. Bestimme diesen Grenzwinkel $\alpha_G$, bei welchem der Körper gerade noch nicht zu rutschen beginnt._

<details>

<summary>Lösung 1</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/wtm7y9772WdKNaS/download)

</details>

<details>

<summary>Lösung 2</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/AD8EM2imFcfbFtS/download)

</details>

<details>

<summary>Lösung 3</summary>

![Lösung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/SaJ5yqyRBqLDToJ/download)

</details>

<details>

<summary>Lösung 4</summary>

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

## Übungsaufgaben Lernbereich _Mechanische Grundlagen_

_Hinweis: Das Skript enthält bereits einige Übungsaufgaben inklusive der zugehörigen Lösungen._

### 1. Kräfte, Reibung, schiefe Ebene

1. Auf einer schiefen Ebene mit dem Neigungswinkel 30°  liegt ein quaderförmiger Körper der Masse 60kg. Das Problem wird zunächst reibungsfrei betrachtet.

1. 1. Konstruiere die Ebene und den Körper. Wähle einen geeigneten Maßstab und zeichne Gewichtskraft, Hangabtriebskraft und Normalkraft maßstabsgetreu ein. Ermittle aus deiner Konstruktion durch Abmessen der Kraftpfeile die Werte der eingezeichneten Kräfte.

1. 2. Berechne die in 1.1. gezeichneten Kräfte.

1. 3. Wir betrachten den Körper nun inklusive der Reibung. Der Körper soll durch die Reibung auf der Ebene ruhen. 
1. 3. 1. Zeichne in deine Skizze die Reibungskraft als Kraftpfeil ein. Nenne die Art der Reibungskraft. Ermittle den Wert dieser Reibungskraft.

1. 3. 2. Berechne, wie groß der Haftreibungskoeffizient (die Haftreibungszahl) $\mu_{Haft}$ mindestens sein muss, damit der Körper tatsächlich nicht rutscht.

<details>

<summary> Lösung 1.1.</summary>

 ![Lsg_1.1](https://diversewolken.ddns.net/nextcloud/index.php/s/RNx7S2jKePn29dp/download)

</details>

<details>

<summary> Lösung 1.2.</summary>

Gewichtskraft $F_g = m \cdot g = 589 N$

Hangabtriebskraft $F_H = m \cdot g \cdot \sin\alpha = 294 N$

Normalkraft $F_N = m \cdot g \cdot \cos\alpha = 510 N$ 

</details>

<details>

<summary> Lösung 1.3.1.</summary>

 ![Lsg_1.3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/65gXp2kGPNgAYTF/download)

- Die Reibungskraft muss der Hangabtriebskraft (Bewegungsrichtung) entgegen gerichtet wirken.

- Da der Körper ruht, handelt es sich bei der Reibungskraft um die __Haftreibungskraft__.

- Damit der Körper ruht, müssen Haftreibungskraft und Hangabtriebskraft gleich groß sein (1. Newtonsches Gesetz)

- $F_R = F_H = 290 N$

</details>

<details>

<summary> Lösung 1.3.2.</summary>

Für die Reibungskraft an der geneigten Ebene gilt die Formel (siehe 1.8.2) 

$\hspace{1cm}$ $F_{Haft} = \mu_{Haft} \cdot F_g \cdot cos\alpha$

Diese Gleichung muss nun nach $\mu_{Haft}$ umgestellt oder mit dem CAS gelöst werden.

$\hspace{1cm}$ $\mu_{Haft} = \dfrac{F_{Haft}}{F_g \cdot \cos \alpha} = \dfrac{290 N}{589 N \cdot \cos(30^\circ)} \approx 0,58$

Die Haftreibungszahl muss mindestens 0,58 betragen.

</details>

### 2. Energieerhaltung, Reibung

| 2. Auf einer Achterbahn bewegt sich ein Körper der Masse (700 kg) mit einer Geschwindigkeit von $3,1\frac{m}{s}$ durch den Punkt A und rollt dann antriebslos über B nach C. | ![Bild_2](https://diversewolken.ddns.net/nextcloud/index.php/s/CSwQygnW7kyQ79Z/download) |

2. 1. Nennen Sie auftretende Energieumwandlungen. Gehen Sie anschließend darauf ein, wie sich die Energieumwandlungen ändern, wenn man Reibungseffekte berücksichtigt.

<details>

<summary> Lösung 2.1. </summary>

> ![Lsg_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/oeH8EcXow243D9Z/download)

</details>

---

2. 2. Berechnen Sie die Geschwindigkeit im Punkt C.

<details>

<summary> Lösung 2.2. </summary>

> ![Lsg_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/iXSDQp4jAA3RY4C/download)

</details>

---

2. 3. Bestimmen Sie die Höhe des Punktes C, die der Körper im reibungsfreien Fall maximal erreichen kann. Begründen Sie Ihren Ansatz.

<details>

<summary> Lösung 2.3. </summary>

> ![Lsg_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/NdKoiEZk68bdnj9/download)

</details>

---

2. 4. Bestimmen Sie die Maximalgeschwindigkeit der Fahrt in der Einheit km/h. Begründen Sie Ihren Ansatz.

<details>

<summary> Lösung 2.4. </summary>

> ![Lsg_2.4](https://diversewolken.ddns.net/nextcloud/index.php/s/e2fA8QNpZjxmEH9/download)

</details>

---

2. 5. Begründen Sie, warum Achterbahnen auf den Schienen mit Rädern ausgestattet sind und nicht mit Kufen (wie beim Schlitten).

<details>

<summary> Lösung 2.5. </summary>

> Um Reibungsverluste möglichst klein zu halten, sollte die Reibungskraft zwischen Schiene und Wagen sehr klein sein. Rollreibung ist viel kleiner als Gleitreibung und verursacht dadurch viel geringere Energieverluste durch Wärme.

</details>

### 3. Kreisbewegung

3. 1. Der Erdradius beträgt etwa 6370 km. Ermitteln Sie die Geschwindigkeit, mit der sich ein Punkt auf der Erdoberfläche des Äquators bei der Erddrehung bewegt? Beachten Sie: Die Erde dreht sich in einem Tag einmal um sich selbst.

<details>

<summary> Lösung 3.1. </summary>

>![Lsg_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/JDkA7GJwBgw8Led/download)

</details>

---


3. 2. Die Spitze des Minutenzeigers einer Turmuhr hat die Geschwindigkeit $1,5 \frac{mm}{s}$. Ermitteln Sie die Zeigerlänge?

<details>

<summary> Lösung 3.2. </summary>

>![Lsg_3.2](https://diversewolken.ddns.net/nextcloud/index.php/s/LQAmgYazNjHo3rD/download)

</details>


---

3. 3. Fahrradfahren/Dynamo

![A3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/Xz8KES8f8kHPE3G/download)

<details>

<summary> Lösung 3.3. </summary>

> ![Lsg_3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/XsJtHCgnrrBqPb5/download)

</details>

---

3. 4. Turbinen und Drehgeschwindigkeit

![A3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/A4yG37d3eHf6ZTL/download)

<details>

<summary> Lösung 3.4. </summary>

> ![Lsg_3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/qTEzgnK4ZZcGcxB/download)

</details>


---

3. 5. Winkelschleifer

![A3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/5xsPM2oXRNsEmzZ/download)

<details>

<summary> Lösung 3.5. </summary>

> ![Lsg_3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/dEGwgjJLZ5Lx9YY/download)

</details>


# Grundkurs Physik 2024/2025 - LB II: Das elektrische Feld

![Blitzeinschläge](https://img.welt.de/img/wirtschaft/webwelt/mobile218083858/8146580597-ci23x11-w2000/Out-Of-The-Blue.jpg)

## 1.1 Grundlagen Elektrizität

### 1.1.1 Atomaufbau

<span style="color:orange">*Ergänze und übernimm diese Wiederholung.*</span>

> Das Atom wird in zwei Grundstrukturen unterteilt

<!-- style="display: block; width: 100%; margin-left: auto;margin-right: auto;" -->
``` ascii
                  Atom
                    |
               .----o-----.             
              /            \             
             /              \           
            /                \          
           v                  v          
```
| [[ Atomkern  ]] | [[ Atomhülle ]] |
| :--: | :--: |




> Darin enthalten sind die Elementarteilchen mit ihren jeweiligen elektrischen Ladungszuständen

| Atomkern | elektrische Ladung |  Atomhülle |
|:--:|:--:|:--:|
| | ![Elektron](https://diversewolken.ddns.net/nextcloud/index.php/s/Bnw2kL8nFrErwXP/download)<span class="green">[[ negativ ]]</span> | <span class="green">[[ Elektron ]]</span> |
| <span class="red"> [[ Proton ]]</span> | ![Proton](https://diversewolken.ddns.net/nextcloud/index.php/s/fs9TTTmjnwRDNm5/download)<span class="red">[[ positiv ]]</span> | |
| [[ Neutron ]] | ![Neutron](https://diversewolken.ddns.net/nextcloud/index.php/s/YJnsjw6546zn55P/download)neutral | |

Beispiele: 

Das Kohlenstoffatom besitzt [[ 6 ]] Protonen im Kern, wohingegen ein Aluminiumatom [[ 13 ]] Protonen enthält. Die Protonenzahl wird durch die [[ Ordnungszahl ]] festgelegt.

{{1}}
************
<span style="color:orange">*Schau dir zur Veranschaulichung noch einmal die verschiedenen Atom-Modelle (LB S. 93) an.*</span>
![ModelleAtomaufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/Mw2YQeHk4bA3aaL/download)

************

### 1.1.2 Elektrisch geladene Atome und Körper

<span style="color:orange">*Ergänze und übernimm diese Wiederholung.*</span>

> Ein neutrales (nicht geladenes) Atom besitzt die [[ gleiche ]] Anzahl an Elektronen und Protonen. Ist die Anzahl der geladenen Elementarteilchen nicht gleich, so wird es als [[ Ion ]] bezeichnet. Das gleiche gilt für elektrisch geladene Körper. Negativ geladene Körper enthalten mehr [[ Elektronen ]] als Protonen und bei positiv geladenen Körpern ist es umgekehrt.

Negativ geladene Ionen nennt man [[ Anionen ]].

Positiv geladene Ionen nennt man [[ Kationen ]]

Beispiele:

Kohlenstoff mit 7 Elektronen ist elektrisch einfach [[ negativ ]] geladen. 

Germanium mit 34 Elektronen ist elektrisch [[ zwei ]]-fach [[ negativ ]] geladen.

__Übung:__

<iframe src="https://learningapps.org/watch?app=21709772" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### Physikalische Beschreibung der elektrischen Ladung

<span style="color:orange">*Nutze LB S. 88. Ergänze und übernimm dieses Tafelbild.*</span>

> Definition: Die elektrische Ladung eines Körpers gibt an, wie groß sein Elektronenüberschuss oder sein Elektronenmangel ist.
>
> __Formelzeichen: [[ Q ]]__
>
> __Einheit: 1 [[ C ]] ( [[ Coulomb ]] )__

Ein Elektron besitzt die kleinst mögliche Ladungsmenge, man nennt das eine __[[ Elementarladung ]] ($e$)__.

> $$ 1\,e = 1,602\cdot10^{-19} C $$

Die Anzahl $N$ der überzähligen Elementarladungen $e$ ergibt demnach die elektrische Ladung $Q$ eines Körpers. 

> $$Q = N \cdot e $$

### 1.1.3 Kräfte zwischen elektrisch geladenen Körpern

> Zwischen geladenen Körpern wirken elektrische Kräfte. Dabei stoßen sich gleichnamig geladene Körper ab, wohingegen sich ungleichnamig geladene Körper anziehen.

<span style="color:orange"> _Ergänze mit Hilfe des LBs die wirkenden Kräfte Kraftpfeile. Übernimm die Zeichnung in deinen Hefter._</span>
![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/Bwpb4qQF7jRzHYk/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

<details>

<summary> Lösung </summary>

![EStatKräfte](https://diversewolken.ddns.net/nextcloud/index.php/s/3bj6ESWb8DdS5m3/download)<!-- style="display: block; margin-left: auto;margin-right: auto;" -->

</details>

## 1.2 Das elektrische Feld

Im Raumbereich um einen __geladenen Körper__ wirkt auf einen anderen geladen Körper eine elektrische __Kraft__ ([Simulation elektrischer Kräfte](https://www.geogebra.org/classic/vbw299uv?embed)).

{{1}}
***********
> Um die Kraftwirkung im gesamten Raum zu __illustrieren__ wird der Begriff <span style="color:orange">elektrisches Feld</span> eingeführt.
***********

{{2}}
***********
> Das __elektrische Feld__ verdeutlicht die Kraftwirkung auf eine <span style="color:orange">positive Probeladung</span>, dargestellt durch so genannte <span style="color:orange">Feldlinien.</span> 
***********


{{3}}
***********
__Beispiele für elektrische Felder:__

| Radialfeld<br>(_inhomogen_) |  Dipolfeld<br>(_inhomogen_) | Homogenes Feld |
| {4}{![Radialfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/3r6ngsjZkRr4RD6/download)} | {5}{![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)} | {6}{![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)} |
| {4}{einzelne Punktladung} | {5}{zwei ungleichnamige Punktladungen} | {6}{Plattenkondensator} |

***********

{{7}}
***********
__Es gelten folgende Vereinbahrungen:__

- Feldlinien verlaufen von <span style="color:red">__Plus__</span> nach <span style="color:darkgreen">__Minus__</span>.

- die Richtung der Feldlinie gibt die Kraftrichtung auf eine <span style="color:red">__positive Probeladung__</span> an

- je dichter die Feldlinien in einem bestimmten Gebiet, desto größer ist die dort wirkende Kraft

- in einem __homogenen Feld__ (z.B. innerhalb eines Plattenkondensators) ist der Betrag der wirkenden Kraft überall gleich

- elektrische Feldlinien beginnen/enden senkrecht an einer Oberfläche
***********

{{8}}
***********
> __Quellen und Senken elektrischer Felder:__
>
> Elektrische Feldlinien beginnen an positiven Ladungen <span style="color:red">__(Quelle)__</span> und enden an negativen Ladungen <span style="color:darkgreen">__(Senke)__</span>
***********

{{9}}
***********
<span style="color:orange">_Aufgabe: Zeichne das elektrische Feld einer positiv geladenen Punktladung, welche zentral vor einer negativ geladenen Kondensatorplatte positioniert ist. Bei Fragen nutze folgende Hinweise._</span>

<details>

<summary> Hinweis: Anordnung der Ladungen </summary>

![Aufgabe_1_L1](https://diversewolken.ddns.net/nextcloud/index.php/s/3mH8ApKdxxj52dJ/download)

</details>

<details>

<summary> Hinweis: Lage der Feldlinien </summary>

![Aufgabe_1_L2](https://diversewolken.ddns.net/nextcloud/index.php/s/DF6TktoF9Xgyg5A/download)

</details>
***********


### Kurze Wiederholung zum elektrischen Feld

<p style="color:orange"> Bitte schau dir folgendes Video an. Bis zur Minute 3:00 ist es Wiederholung, dann folgenden Fakten zum elektrischen Feld, welche wir noch nicht besprochen haben. Du kannst es dir zur Information ansehen, musst du aber nicht. </p>

!?[ElektischesFeld](https://www.youtube.com/watch?v=EN6dTZH-HDs)

### 1.2.1 Berechnung des elektrischen Feldes

Die Stärke des elektrischen Feldes $\vec{E}$ berechnet sich aus der Kraft $\vec{F}$ auf eine elektrische Ladung $Q$.

> $$ \vec{E} = \frac{\vec{F}}{Q} $$
>
> <div style="color:orange">_Hinweis: Die Pfeile über $\vec{E}$ und $\vec{F}$ bedeuten, dass es sich um Vektoren mit einer Richtung und einem Wert (auch Betrag genannt) handelt. Kräfte haben wir bereits als Vektoren gezeichnet._ </div>
>
> Einheit: $$\Big[\dfrac{N}{C}\Big]$$
>
> $\hspace{1cm}$  <div style="color:orange">_Hinweis: $N$ (Newton) ist die Einheit der Kraft und $C$ (Coulomb) ist die Einheit der elektrischen Ladung._ </div>

### Aufgaben zum elektrischen Feld

@uhr

<div style="color:orange">_Hinweis: Löse folgende Augaben. Du kannst auf das Glühlampensymbol klicken, wenn du Tipps benötigst, auch mehrfach._ </div>

1. Die Erde bestitz in zur Oberfläche gerichtetes elektrisches Feld, das an der Oberfläche eine Stärke von $ 130 \dfrac{N}{C} $ besitzt.

1. 1. Welches Vorzeichen hat die demzufolge die Ladung der Erde.

        <!-- data-solution-button="off" -->
        [( )] positiv
        [(X)] negativ
        [( )] kann man nicht sagen
        [[?]] Achte auf die Richtung der Feldlinien im Aufgabentext. Vergleiche die Richtung mit der Richtungsvorgabe für Feldlinien (siehe 1.2)
        [[?]] Feldlinien beginnen bei positiven und enden bei negativen Ladungen

---


1. 2. Eine Tischtennisball mit einer metallischen Oberfläche sei elektrisch negativ aufgeladen. Entscheide, ob der Tischtennisball von der Erde abgestoßen oder angezogen wird.

        <!-- data-solution-button="off" -->
        [( )] angezogen
        [(X)] abgestoßen
        [[?]] Die Erde ist, wie in 1.1. überlegt negativ geladen. Überprüfe die Kraftwirkung auf den negativ geladenen Tischtennisball.

---

1. 3. Die Ladung des Tischtennisballs beträgt $Q = 0,1\cdot10^{-3} C =  5 mC $. Ermittle den Wert der Kraft $\vec{F}$, mit welche auf den TT-Ball wirkt.<br>(_Hinweis: Zwischen Zahl und Einheit bitte kein Leerzeichen._)

        [[ 0,013N ]]
        [[?]] Die Formel zur Berechnung der Kraft findest du in Abschnitt 1.2.1.
        [[?]] Stelle die Formel $\vec{E} = \frac{\vec{F}}{Q} $ nach $\vec{F}$ um.

---

1. 4. *Der Ball hat eine Masse von 5g. Ermittle die Ladung Q, die er haben müsste, damit er über dem Erdboden schweben könnte.<br>_Gib die Antwort in der Einheit mC (Millicoulomb) an. Runde auf 2 Kommastellen._

        [[ 0,38mC ]]
        [[?]] Wenn der Ball schweben soll, muss Gewichtskraft $F_g$ und abstoßende elektrische Kraft $F_{el}$ gleich groß sein.
        [[?]] Es gilt: $F_g = m \cdot g$ und $F_{el} = E \cdot Q$.
        [[?]] Umgestellt nach $Q$: $Q=\frac{m \cdot g}{E}$
        [[?]] Lösung $Q = 0,0003773 C \approx 0,38mC$

---

2. Entscheide für die folgenden Felder, um welche Art von Feld es sich handelt.

2. 1. ![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)

        <!-- data-solution-button="off" -->
        [( )] Radialfeld
        [(X)] Dipolfeld
        [( )] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.

---

2. 2. ![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)

        <!-- data-solution-button="off" -->
        [( )] Radialfeld
        [( )] Dipolfeld
        [(X)] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.

---

2. 3. ![Radialfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/3r6ngsjZkRr4RD6/download)

        <!-- data-solution-button="off" -->
        [(X)] Radialfeld
        [( )] Dipolfeld
        [( )] Homogenes Feld
        [[?]] Vergleiche Feldtypen unter 1.2.



## Auswertung LK

__Notenverteilung: __

![Notenverteilung_LK_LB1](https://diversewolken.ddns.net/nextcloud/index.php/s/NqaDgPq9C4mDWiw/download)

Klausur: @color(11.11.,red) -> Noch drei Doppelstunden 

@color(-> Thema LB1 ist auch Teil der Klausur,red)

---

{{1}}
***********
__Lösungshinweise:__


***********

## 1.3. Der Kondensator

__Definition:__ Ein Kondenstator ist ein Bauelement zur __Speicherung von elektrischer Ladung__. Er besteht aus zwei leitenden Schichten, die durch einen Isolator (@color(Dielektrikum,orange)) voneinander getrennt sind @color([Vlg. LB S. 80], darkgrey).

Einfachste Bauform: @color(__Plattenkondensator__, orange) 


![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

{{1}}
*******
__Eigenschaften eines Plattenkondensators:__

- auf den beiden Platten eines Plattenkondensators werden __elektrische Ladungen $Q$__ gespeichert
*******

{{2}}
*******
- __das elektrische Feld__ zwischen den Platten ist @color(homogen, orange), d.h. es hat an jedem Punkt dieselbe Feldstärke $\vec{E}$
*******

{{3}}
*******
- __die Feldlinien__ zeigen von der @color(positiven, red) Platte zur @color(negativen, blue) Platte
*******

{{4}}
*******
- __das elektrische Feld__ $\vec{E}$ eines Plattenkondensators berechnet sich mit
*******

{{5}}
*******
> $$ \boxed{\vec{E} = \dfrac{U}{d}} $$
>
> $\hspace{1cm}$ $U$ ... Spannung zwischen den Platten $\big[ V \big]$ 
>
> $\hspace{1cm}$ $d$ ... Abstand der Platten $\big[ m \big]$ 

- wird in das elektrische Feld eine elektrische Ladung eingebracht, so wirkt auf die Ladung eine elektrische Kraft die mit $\vec{F}=\vec{E}\cdot q$ berechnet werden kann
*******

### Aufgabe 1. - Plattenkondensator

An einem Plattenkondensator beträgt die Spannung 1,5 kV und der Plattenabstand 3,2cm. 

Bestimme die Kraft, die auf einen Körper mit einer Ladung von 20 nC wirkt <br> @color(Hinweis: $nC=10^{-9}C$ [Nano-Coulomb], grey) <br> @color(Lösung: siehe Lehrbuch S.97, grey)


## 1.4. Die Kapazität

__Definition:__ Die @color(Kapazität, orange) eines Kondensators beschreibt seine Fähigkeit eine __Ladungsmenge Q__ zu speichern, wenn eine bestimmte __Spannung U__ angelegt wird.

{{1}}
*********
> __Formel:__ 
>
> $$ \boxed{ C = \dfrac{Q}{U} } $$
>
> $\hspace{1cm}$ $C$ ... Kapazität  
>
> $\hspace{1cm}$ $Q$ ... im Kondensator gespeicherte Ladung $\big[ C \big]$ 
>
> $\hspace{1cm}$ $U$ ... angelegte Spannung $\big[ V \big]$ 
*********

{{2}}
*********
> __Einheit der Kapazität:__  $$\textbf{1 Farad = 1 F}$$
>
> $$\Big[ F = \dfrac{C}{V} \Big] $$
*********

{{3}}
*********
> __Kapazität eines @color(Plattenkondensators, orange):__
>
> $$ \boxed{ C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} } $$
>
> <p style="text-align:center">[IQB-Formelsammlung](https://www.iqb.hu-berlin.de/abitur/abitur/dokumente/naturwissenschaften/N_Mathematischna.pdf) (S.28+54)</p>
*********

{{4}}
*********
> $\hspace{1cm}$ $C$ ... Kapazität  
>
> $\hspace{1cm}$ $\varepsilon_0$ ... elektrische Feldkonstante $\boxed{\varepsilon_0 = 8,854 \cdot 10^{-12}\,\dfrac{A\cdot s}{V \cdot m}}$
>
> $\hspace{1cm}$ $\varepsilon_r$ ... Dielektrizitätszahl [Einheitenlos] @color( - Luft/Vakuum: $\varepsilon_r=1$,blue)
>
> $\hspace{1cm}$ $A$ ... Flächeninhalt der Platte $[m^2]$
>
> $\hspace{1cm}$ $d$ ... Abstand der Platten $[m]$
*********



### Aufgabe 2. Elektrische Ladung

__Löse LB. S. 122 6/8__

<div style="text-indent:10%">

Überprüfe deine Lösungen

<details>

<summary> Lösung S.122/6 </summary>

$N=\frac{0,1 C}{1,602\cdot10^{-19}C}\approx6,242 \cdot 10^{17} \textbf{Elektronen}$

</details>

<details>

<summary> Lösung S.122/8 </summary>

a) negativ

b) $Q = N \cdot e = 3,1\cdot10^{10} \cdot 1,602\cdot10^{-19} C = 4,966\cdot10^{-9} C \approx 5 nC $

</details>

</div>

### Aufgabe 3. Spannung am Kondensator

__Bestimme die Spannung, die am Kondensator aus Aufgabe 1 anliegen muss, damit auf ein Elektron eine Kraft von 5 nN wirkt.__

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

Nutze Lösung der Aufgabe 1. und stelle die Formel nach U um.

> $1nN = 1 \cdot 10^{-9} N$

Ladung des Elektrons:

> $q=-1,602 \cdot 10^{-19}C$ (Nutze IQB-Formelsammlung -> Naturkonstanten S.50/51)

</details>

<details>

<summary> Lösung </summary>

![BildDerLösung](https://diversewolken.ddns.net/nextcloud/index.php/s/mtM5TLiakAzrisa/download)<!-- style="width:80%"-->

</details>

</div>

### Aufgabe 4. Geladenes Teilchen im Plattenkondensator

__Ein Plattenkondensator hat eine Querschnittsfläche der Platten von $50\,cm^2$. Der Abstand der Platten beträgt $2\,cm$. Der Kondensator ist horizontal aufgestellt, d.h. eine Platten unten, eine Platte oben. Zwischen den Platten sei Vakuum.__

4. 1. Bestimme die Kapazität dieses Kondensators.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.1. </summary>

Nutze die Formel zur Berechnung der Kapazität C eines Plattenkondensators. Achte auf die Umrechnungen von Fläche und Länge.

</details>

<details>

<summary> Lösung 4.1. </summary>

![Lsg_1.3_A4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/EKTW7ncRr3oSJcJ/download)<!-- style="width:80%"-->

</details>

</div>

4. 2. Zwischen den Platten befindet sich ein einzelnes Proton. Der Kondensator soll so geladen sein, dass das Proton zwischen den Platten schwebt. Zeichne dazu eine Skizze und gib die Pole an den Platten an. Zeichne die wirkenden Kräfte qualitativ ein.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.2. </summary>

Zeichne einen Plattenkondensator mit einer Platten oben und einer Platte unten. Zeichne in die Mitte das punktförmige Proton. Überprüfe, welche Kraft auf das Proton aufgrund seiner Masse wirkt. Zeichne diese Kraft ein. Da das Proton schweben soll, muss diese Kraft durch eine weitere Kraft genau aufgehoben werden. Zeichne auch diese Kraft ein. Überlege nun, wie die obere Platte geladen sein muss.

</details>

<details>

<summary> Lösung 4.2. </summary>

![Lsg_1.3_A4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/bW2JAqywjYBA2Wx/download)<!-- style="width:80%"-->

</details>

</div>

4. 3. Bestimme die Spannung, die am Kondensator angelegt werden muss, damit das Elektron schwebt.

<div style="text-indent:10%"> 

<details>

<summary> Hinweis 4.3. </summary>

Gewichtskraft und elektrische Kraft müssen gleich groß sein, damit das Proton schwebt. Recherchiere Masse $m_p$ und Ladung $q$ eines Protons mit Hilfe der IQB-Formelsammlung. Überprüfe im Skript die Formeln für Gewichtskraft und elektrische Kraft auf eine Probeladung im elektrischen Feld. Nutze die Formel für die elektrische Feldstärke in einem Plattenkondensator.

</details>

<details>

<summary> Lösung 4.3. </summary>

![Lsg_1.3_A4.3](https://diversewolken.ddns.net/nextcloud/index.php/s/Y8risbAANPaWwTq/download)<!-- style="width:80%"-->

</details>

</div>

## 1.5 Pendel im elektrischen Feld

![TB_FadenpendelElektrischesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/aB6PmLHcseFXY2Z/download)

### Aufgabe 5. Pendel im elektrischen Feld

5. Elektrisches Feld mit Probeladung: LB. S. 123/15

<div style="text-indent:10%"> 

<details>

<summary> Lösung a) </summary>

![Lsg_LB123_15](https://diversewolken.ddns.net/nextcloud/index.php/s/W3SQgTE7JErmfbb/download)<!-- style="width:80%"-->

</details>


<details>

<summary> Lösung b) </summary>

![Lsg_LB123_15](https://diversewolken.ddns.net/nextcloud/index.php/s/rjwJHMBwm3NbwrT/download)<!-- style="width:80%"-->

</details>

</div>
