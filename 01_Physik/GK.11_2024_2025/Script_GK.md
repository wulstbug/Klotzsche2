
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
}
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@orange
<bdi style="color:orange">@0</bdi>
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

@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0$\ =\ $
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

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->

# Grundkurs Physik 2024/2025 - Skript

@uhr

# LB I - Mechanische Grundlagen

@color(__Checkliste zur Klausur__,red)

__Energie:__

- Energieformen erkennen und zuordnen [Übung Zuordnen Energieformen](#übung-zuordnung-energieformen)
- Formeln für Energieformen zur Berechnung nutzen [1.2/1.3]
- Energieerhaltungssatz kennen [LB S. 6 unten]

__Reibung:__

- Reibungsarten erkennen und zuordnen [Übung Zuordnen Energieformen](#übung:-zuordnung-von-reibungsarten) 
- Unterscheiden von erwünschter und unerwünschter Reibung [Übung Zuordnen Energieformen](#übung:-zuordnung-von-reibungsarten) 
- Beschreibung des Einfluss der Reibung qualitativ [->1.8.4] und quantitativ [->1.8.5]

__Kräfte:__

- Kennen Newton'schen Gesetze [->1.9.2]
- Darstellung von Kräften als Kraftpfeil [->1.9.3]
- Addition und Zerlegung von Kräften z.B. an der Schiefen Ebene [->1.9.4 & 1.9.5.]

__Kreisbewegung:__

- Kennen der Bedingung einer gleichförmigen Kreisbewegung (Zentripetalkraft) und deren Berechung

__Vermischte Aufgaben:__

- Siehe [Übungsaufgaben Lernbereich Mechanische Grundlagen](#übungsaufgaben-lernbereich-mechanische-grundlagen)


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

## Lösungen Lehrbuchaufgaben

@color(_Auf Wunsch hier ein paar Lösungen zu Übungsaufgaben.<br><br> MfG CG_<br><br>, orange)

---

__LB S. 26 Aufgabe 7__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB26_7](https://diversewolken.ddns.net/nextcloud/index.php/s/7sgBcLeK3iSG6Ab/download)<!-- style="max-width:80%"-->

</details>


</div>

---

__LB S. 26 Aufgabe 12__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB26_12](https://diversewolken.ddns.net/nextcloud/index.php/s/rxXaawKKw8ciAk3/download)<!-- style="max-width:80%"-->

</details>


</div>

---


__LB S. 28 Aufgabe 23__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB28_23](https://diversewolken.ddns.net/nextcloud/index.php/s/BJbaEwW2RwWgAxp/download)<!-- style="max-width:80%"-->

</details>


</div>

---



__LB S. 28 Aufgabe 25__

<div style="text-indent:10%"> 

<details>

<summary> Lösung a) </summary>

![Lsg_LB28_25a](https://diversewolken.ddns.net/nextcloud/index.php/s/qRNqZPY4Ex7aJ4S/download)<!-- style="max-width:80%"-->

</details>

<details>

<summary> Lösung b-d) </summary>

![Lsg_LB28_25bcd](https://diversewolken.ddns.net/nextcloud/index.php/s/gykGqzePijz3ZwS/download)<!-- style="max-width:80%"-->

</details>

</div>

---

__LB S. 28 Aufgabe 26__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB28_26](https://diversewolken.ddns.net/nextcloud/index.php/s/56bGefCmtXM4L73/download)<!-- style="max-width:80%"-->

</details>

</div>

---

@color(nicht Klausurrelevant, red)

__LB S. 69 Aufgabe 11__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB69_11](https://diversewolken.ddns.net/nextcloud/index.php/s/4WSTFyJzB4CkmZd/download)<!-- style="max-width:80%"-->

</details>

</div>


# Grundkurs Physik 2024/2025 - LB II: Das elektrische Feld

![Blitzeinschläge](https://img.welt.de/img/wirtschaft/webwelt/mobile218083858/8146580597-ci23x11-w2000/Out-Of-The-Blue.jpg)

@color(__Checkliste zur Klausur__,red)

__Grundlagen Elektrizität [1.1]:__

- Kennen des Atomaufbaus, Elementarteilchen, Ladungszustände

- Kennen des Begriffs Elektrische Ladung, Kraftwirkungen auf elektrisch geladene Körper [Aufgabe 2]

__Grundlagen Elektrizität [1.2]:__

- Kennen des Begriffs und der Bedeutung des elektrischen Feldes

- Berechnung des elektrischen Feldes als Kraft auf Probeladung 

- Kennen von Eigenschaften elektrischer Felder und Arten von elektrischen Feldern 

__Kondensator [1.3/1.4]:__

- Kennen des Begriffs und Nutzen von Kondensatoren, Plattenkondensator als spezielle Bauform

- Berechnung des elektrischen Feldes eines Plattenkondensators und dessen Eigenschaften

- Kennen des Begriffs Kapazität als Fähigkeit Ladung zu Speichern, Berechnung allgemein und bei Plattenkondensator [-> Aufgabe 1]

- Kraftwirkung auf elektrische Ladungen im Feld eines Kondensators [-> Aufgabe 3/4]

__Energie im elektrischen Feld [1.5]:__

- Berechnung der Feldenergie

- Abhängigkeiten der im Kondensator gespeicherten Energie und der Kapazität des Kondensators [-> Aufgabe 5]

- Potentielle Energie einer Probeladung im elektrischen Feld eines Kondensators

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
> $\hspace{1cm}$ @color(_Hinweis: Im folgenden werden wir den Buchstaben **Q** für die Ladung auf dem Kondensator und den Buchstaben **q** für die Ladung eines Teilchens im elektrischen Feld verwenden_, orange)
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
> _Für die einfachste Bauform eines Kondensators [siehe 1.3](#13-der-kondensator) kann man die Kapazität wie folgt berechnen:_
> 
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

{{5}}
*********
__Beispiel:__ _Ermittle die Kapazität des Plattenkondensators auf dem Lehrertisch. Komm dazu in kleiner Gruppe nach vorn und bestimme die notwendigen Werte._

<p class="newspaper">

geg.:

<div style="text-indent:10%">

$A$ = <bdi style="color:orange"> $28\,cm \cdot 28\,cm = 0,28 \cdot 0,28\,m^2 = 0,0784 m^2$</bdi>

$d$  <bdi style="color:orange"> $\approx 1,5\,cm = 0,015 m$ </bdi>

$\varepsilon_r$ = <bdi style="color:orange"> $ = 1$ </bdi>

</div>

<p class="cb">

ges.:

<div style="text-indent:10%">

$C$

</div>

Lsg.:

<div style="text-indent:10%">

$C = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} $

$C \approx $  <bdi style="color:orange"> $ 4,6 \cdot 10^{-11} F $ = $ 46\,pF$  </bdi>

<bdi style="color:orange">Lösungen $ C = 2 \cdot 10^{-11}\,F$ bis $ 8 \cdot 10^{-11}\,F $ sind akzeptabel</bdi>

Beispiel: Taschenrechner:

![GTR](https://diversewolken.ddns.net/nextcloud/index.php/s/939gMiCMEoNn7bL/download)<!-- style="width:80%" -->

</div>

</p>

</p>

*********


### Aufgabe 2. Elektrische Ladung

__Löse LB. S. 122 6/8__  [Nutze hierfür __1.1 Grundlagen Elekrizität__](#1.1-grundlagen-elektrizität)

<div style="text-indent:10%">

Überprüfe deine Lösungen

<details>

<summary> Lösung S.122/6 </summary>

$N=\frac{0,1 C}{1,602\cdot10^{-19}C}\approx6,242 \cdot 10^{17} \textbf{Elektronen}$

</details>

<details>

<summary> Lösung S.122/8  </summary>

a) negativ

b) $Q = N \cdot e = 3,1\cdot10^{10} \cdot 1,602\cdot10^{-19} C = 4,966\cdot10^{-9} C \approx 5 nC $

</details>

</div>

### Aufgabe 3. Spannung am Kondensator*

__Bestimme die Spannung, die am Kondensator aus Aufgabe 1 [siehe 1.3 Der Kondensator](#1.3.-der-kondensator) anliegen muss, damit auf ein Elektron eine Kraft von 5 nN wirkt.__

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

Nutze Lösung der [Aufgabe 1.](#aufgabe-1.-plattenkondensator) und stelle die Formel nach U um.

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

## 1.5 Energie im elektrischen Feld

> Im elektrischen Feld eines Kondensators ist Energie gespeichert und wird als __elektrische Feldenergie $E_{Feld}$__  bezeichnet.
>
> $$ \boxed{E_{Feld} = \frac{1}{2}\cdot Q \cdot U} $$
>
> $$ \boxed{E_{Feld} = \frac{1}{2}\cdot C \cdot U^2} $$
>
> $\hspace{1cm}$ $C$ ... Kapazität des Kondensators $\big[ F \big]$
>
> $\hspace{1cm}$ $Q$ ... im dem Kondensator gespeicherte Ladung $\big[ C \big]$
>
> $\hspace{1cm}$ $U$ ... am Kondensator anliegende Spannung $\big[ V \big]$

### Aufgabe 5: Feldenergie im Kondensator

5.1. Ergänze folgende Aussage: Um die Feldenergie eines Kondensators zu erhöhen kann man:

     <!-- data-solution-button="off" -->
     [[ ]] die Spannung verringern
     [[X]] die Spannung erhöhen
     [[X]] ein Dielektrikum zwischen die Platten des Kondensators einbringen
     [[ ]] ein Dielektrikum zwischen den Platten des Kondensators entfernen
     [[ ]] die elektrische Feldenergie ist eine Konstante und kann nicht verändert werden
     [[?]] Nutze die zweite Formel für die Feldenergie. Überprüfe ob eine Veränderung von Spannung und Kapazität die elektrische Feldenergie vergrößert oder verkleinert. Überprüfe auch die Formel zur Berechnung der Kapazität und den Einfluss eines Dielektrikums.

5. 2. Ergänze folgende Aussage: Wird bei einem Kondensator mit einer festen Kapazität die Spannung verdoppelt so

     <!-- data-solution-button="off" -->
     [(X)] verdoppelt sich die Feldenergie
     [( )] vervierfacht sich die Feldenergie
     [( )] bleibt die Feldenergie gleich
     [( )] halbiert sich die Feldenergie
     [( )] viertelt sich die Feldenergie
     [[?]] Nutze die zweite Formel für die Feldenergie. Wähle Beispielwerte für die Spannung und Kapazität. Verdopple die Spannung und überprüfe den Einfluss auf das Ergebnis

5. 3. Wahr oder falsch? Bringt man die Platten eines Kondensators näher zusammen, steigt die Kapazität.

     <!-- data-solution-button="off" -->
     [(X)] wahr
     [( )] falsch

5. 4. Wahr oder falsch? Verkleinert man die Plattenfläche eines Kondensators so steigt die Kapazität.

     <!-- data-solution-button="off" -->
     [( )] wahr
     [(X)] falsch

5. 5. An einem Plattenkondensator ($A$ ... Flächeninhalt der Platte, $d$ ... Abstand der Platten, Luft zwischen den Platten), soll eine feste Spannung $U$ angelegt werden. Markiere die Formel zur Berechnung der Ladung $Q$ auf den Platten.

     <!-- data-solution-button="off" -->
     [( )] $Q = \dfrac{\varepsilon_0 \cdot \varepsilon_r \cdot A}{d \cdot U} $
     [( )] $Q = \varepsilon_0 \cdot \varepsilon_r \cdot A \cdot d \cdot U $
     [( )] $Q = \dfrac{d \cdot U}{\varepsilon_0 \cdot \varepsilon_r \cdot A} $
     [( )] $Q = \dfrac{d}{\varepsilon_0 \cdot \varepsilon_r \cdot A \cdot U} $
     [(X)] $Q = \varepsilon_0 \cdot \varepsilon_r \cdot \dfrac{A}{d} \cdot U $     
     [[?]] Nutze die allgemeine Formel für die Kapazität ([1.4](#1.4.-die-kapazität)) und die spezielle Formel für die Kapazität des Plattenkondensators.
     [[?]] Setze beide Formeln gleich und stelle sie nach der Ladung $Q$ um

5. 6. Ein Plattenkondensator der zwischen den Platten mit Luft gefüllt ist hat eine Kapazität von 1 nF. Dann wird ein Stoff zwischen die Platten geschoben und die Kapazität erhöht sich auf den Wert 2,3 nF. Benenne den Stoff, der zwischen die Platten geschoben wurde.

     <!-- data-solution-button="off" -->
     [[ Paraffin ]]
     [[?]] Überprüfe in der Formel zur Berechnung der Kapazität eines Plattenkondensators [-> 1.4], welche physikalische Größe sich auf ein Material bezieht.
     [[?]] Das Material zwischen den Platten wird durch die Dielektizitätszahl $\varepsilon_r$ repräsentiert. Nutze die Formelsammlung für die Dielektrizitätszahl verschiedener Materialen.
     [[?]] Die Dielektrizitätszahl verschiedener Materialien wird in der Formelsammlung auf Seite 54 aufgeführt. Überprüfe, welches Material eine Dielektrizitätszahl von 4 besitzt.


5. 7. [LEIFI-Quiz zur Kondensatorformel](https://www.leifiphysik.de/elektrizitaetslehre/kondensator-kapazitaet/aufgabe/quiz-zur-kondensatorformel)

## 1.6 Potentielle Energie elektrischer Ladungen im Feld eines Plattenkondensators

![Tafelbild_potEnergie_EFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/Po989qzJJYmz4AJ/download)

### Aufgabe zur elektrischen potentiellen Energie

6. Wir betrachten ein Elektron im elektrischen Feld eines Plattenkondensators. Im Raum zwischen den Platten sei Vakuum, die Platten haben eine Querschnittsfläche von $0,02\,m^2$, einen Abstand von $10\,cm$. Am Kondensator sei eine Spannung von $500\,V$ angelegt.

---

6. 1. Gib die elektrische Ladung und die Masse des Elektrons an.

     ---

     __Ergebnisse:__

     _Hinweis: 10er-Potenzen (z.b: $10^{-9}$ können hier mit dem Buchstaben $\footnotesize\textbf{E}$ angegeben werden (wie im CAS EXP-Taste)._

     ![GTR](https://diversewolken.ddns.net/nextcloud/index.php/s/939gMiCMEoNn7bL/download)<!-- style="width:80%" -->

@rangeQuiz2($\hspace{1cm}$ $q$, 1.602E-19, C)

---

@rangeQuiz2($\hspace{1cm}$ $m_e$, 9.109E-31, kg)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

siehe Formelsammlung _Naturkonstanten_

</details>

</div>

6. 2. Bestimme den Wert des elektrische Feldes innerhalb des Kondensators.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $E_{el}$, 5000, $\frac{V}{m}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis </summary>

siehe Formelsammlung _Elektrisches Feld im Plattenkondensator_

</details>

</div>

---

6. 3. Ermittle die elektrische Kraft, die auf das Elektron wirkt und vergleiche sie mit der Gewichtskraft, die auf das Elektron wirkt.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $F_{el}$, 8.01e-16, $N$)

@rangeQuiz2($\hspace{1cm}$ $F_{g}$, 8.936e-30, $N$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zum Vergleich</summary>

Die elektrische Kraft $F_{el}=8.01\footnotesize\textbf{E}-16\,N$ ist viel viel größer, als die Gewichtskraft $F_g=8,94\footnotesize\textbf{E}-30\,N$. 

Mit anderen Worten, die Gewichtskraft kann man für dieses Beispiel vernachlässigen.

</details>

</div>

---

6. 4. Ermittle die potentielle elektrische Energie, die dem Elektron hinzugefügt wird, wenn es von der positiven Platte des Kondensators zur negativen Platten _angehoben_ wird.

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $E_{pot\ el}$, 8.01e-17, $J$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Berechnung</summary>

siehe Skript 1.6: $E_{pot\,el} = F_{el} \cdot d$

</details>

</div>

---

6. 5. Wenn das Elektron an der negativen Platten angekommen ist, wird es aus der Ruhe heraus losgelassen. Ermittle die Beschleunigung, mit welcher das Elektron beschleunigt wird. Ermittle auch die Geschwindigkeit, die es besitzt, wenn es bei der positiven Platten ankommt (nutze dafür die Energieerhaltung). <br> _Hinweis: Hier kommen sehr große Werte heraus._

     ---

     __Ergebnisse:__   

@rangeQuiz2($\hspace{1cm}$ $a$, 8.794e14, $\frac{m}{s^2}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Beschleunigung</summary>

Die Beschleunigung lässt sich nach dem zweiten Newton'schen Gesetz berechnen.

<details>

<summary> Berechung zur Beschleunigung</summary>

$$ F_{el} = m_e \cdot a$$ 

$$ a = \frac{F_{el}}{m_e} = \frac{8,01 \cdot 10^{-16} N}{9,11 \cdot 10^{-31} kg}$$ 

$$ a = 8,79 \cdot 10^{-14} \Big[ \frac{N}{kg} = \frac{m}{s^2} \Big] $$ 

</details>

</details>

</div>

---

@rangeQuiz2($\hspace{1cm}$ $v$, 1.326e7, $\frac{m}{s}$)

<div style="text-indent:10%"> 

<details>

<summary> Hinweis zur Geschwindigkeit</summary>

Setze die potentielle elektrische Energie aus 6.4 mit der kinetischen Energie gleich und löse nach der Geschwindigkeit auf.

<details>

<summary> Berechung zur Geschwindigkeit</summary>

$$ E_{pot\,el} = E_{kin}$$ 

$$ E_{pot\,el} = \frac{1}{2}\cdot m_e \cdot v^2$$ 

$$ v = \sqrt{ \frac{2\cdot E_{pot\,el}}{m_e}} = \sqrt{ \frac{2\cdot 8,01 \cdot 10^{-17} J}{9,019 \cdot 10^{-31} kg}} $$ 

$$ v = 1,326 \cdot 10^{7} \frac{m}{s} $$

</details>

</details>

</div>

### Aufgabe 7. Pendel im elektrischen Feld

7. Elektrisches Feld mit Probeladung: LB. S. 123/15

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


### Lösungen Lehrbuchaufgaben

__LB S. 123 Aufgabe 15__

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

---

__LB S. 123 Aufgabe 17__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB123_17](https://diversewolken.ddns.net/nextcloud/index.php/s/9wA3JnFcLnmWqEZ/download)<!-- style="width:80%"-->

</details>


</div>

---

__LB S. 124 Aufgabe 23__

<div style="text-indent:10%"> 

<details>

<summary> Lösung </summary>

![Lsg_LB123_17](https://diversewolken.ddns.net/nextcloud/index.php/s/JRCxMQoBCgFDWcW/download)<!-- style="width:80%"-->

</details>

</div>

## Rückgabe Klausur 11.1

@uhr

<details>

<summary> Notenspiegel </summary>

![Verteilung](https://diversewolken.ddns.net/nextcloud/index.php/s/HtKkrqECSCnpkEm/download)

__Korrekturzeichen:__

- __ug:__ ungenau

- __uv:__ unvollständig

- __Bg:__ fehlende oder falsche Begründung

</details>

## Sim1 Elektronische Schaltkreise mit Kondesatoren

??[PhET-Kondensator1](https://phet.colorado.edu/sims/html/capacitor-lab-basics/latest/capacitor-lab-basics_all.html?locale=de)


## Sim2 Elektronische Schaltkreise mit Kondensatoren

??[PhET-Kondensator2](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac/latest/circuit-construction-kit-ac_all.html?locale=de)

## 1.7 Elektronische Schaltkreise mit Kondensatoren

@color(_Hinweis: Für die folgenden Unterrichtseinheiten werden wir mit dem Formelzeichen $Q$ immer die Ladung auf den Platten des Kondensators bezeichnen._,darkgrey) 

<br>

__Wiederholung:__ Schließen wir den Kondensator an eine Gleichspannungsquelle (Spannung $U-$) an, so fließen elektrische Ladungen auf den Kondensator. Im Kondensator wird die Ladungsmenge $Q$ gespeichert.



<p class="newspaper">

{{1}}
***********

__Ladung $Q$__

<p style="margin-left:5%">

Die Ladung $Q$ beschreibt Anzahl überzähliger Elemtarladungen $e$.

_Einheit: 1C (1 Coulomb)_

$$ \boxed{1 e = 1,6 \cdot 10^{-19} C} \,\,\,\mathrm{oder}\,\,\, \boxed{1C = 6,24 \cdot 10^{18} e}$$

</p>

---

***********

{{2}}
***************

__Spannung $U$__


<p style="margin-left:5%">

Die Spannung $U$ beschreibt den @color(das Potential bzw. den Antrieb für das Fließen von Ladungsträgern, orange). 
Je größer die Spannung, desto größer ist die gespeicherte Ladung.

_Einheit: 1V (1 Volt)_

</p>

---

***************

{{3}}
***************

__Stromstärke $I$__

<p style="margin-left:5%">

Die Stromstärke $I$ beschreibt <bdi style="color:orange">die Menge der elektrischen Ladungen $Q$, die pro Sekunde durch einen Leiterquerschnitt fließen</bdi>.

_Einheit: 1A (1 Ampere)_

_Eine Stromstärke von 1A bedeutet, dass pro Sekunde eine Ladung von 1 C fließt._

$$ \Big[ A = \frac{C}{s} \Big] $$

</p>

--- 

***************

{{4}}
***************

__Gespeicherte Energie $E_{Feld}$__

<p style="margin-left:5%">

Die im Kondensator (im elektrischen Feld) gespeicherte Energie $E_{Feld}$ wird berechnet mit

$$ E_{Feld} = \frac{1}{2}\cdot Q \cdot U $$

$$ E_{Feld} = \frac{1}{2}\cdot C \cdot U^2 $$

_Einheit: 1J (1Joule)_

</p>

***************



<p class="cb">

__Schaltplan zum Laden des Kondensators__

![Schaltkreis_Kondensator1](https://diversewolken.ddns.net/nextcloud/index.php/s/ARdjFMxTDoDoAWz/download)

</p>

</p>

### 1.7.1 Experiment: Vorübung zur Schulung mit Cassy

__Aufgabenstellung:__ Nimm mit die U-I-Kennlinie für einen ohmschen Widerstand ($R=512\Omega$) auf. Variiere die Spannung in Schritten von 1 V im Intervall 0 - 10 V.


<p style="color:blue">

__Durchführung:__ _(muss nicht notiert werden)_ 

1. Übernimm Überschrift und Aufgabenstellung auf eine neue Seite.

2. Übernimm den Schaltplan und die zugehörige Tabelle für die Messwerte.

3. Stelle das Cassy-Messgerät anhand der Erklärungen ein.

4. Variiere die Spannung an der Spannungsquelle von 0..10V in Schritten von 1 V. Notiere Spannung und Stromstärke an Cassy-Messgerät.

5. Zeichne eine U-I-Kennlinie: Zeichne dazu ein Diagramm (x-Achse: U in V | y-Achse: I in A).

6. Öffne die nächste Seite: @color(_1.7.2 Automatische Messwert-Erfassung mit Cassy_,darkgreen). Folge den Anweisungen und wiederhole die Messung mit einer Automatischen Messwert-Aufname.

</p>

<p class="newspaper">

__Schaltkreis:__

![Schaltkreis_Exp1](https://diversewolken.ddns.net/nextcloud/index.php/s/rAwYZqysffqknd6/download)

{{0-1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | |
| 1 | |
| 2 | |
| .. | |
| 9 | |
| 10 | |
************

{{1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | 0,002 |
| 1 | 0,004 |
| 2 | 0,006 |
| 3 | 0,008 |
| ..| .. |
| 9 | 0,018 |
| 10 | 0,02 |
************

<p class="cb">

__Diagramm Kennlinie:__

{{0-1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/Z9at8rKH75N4Agt/download)
*************

{{1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/ztd7ScndfNAYNqM/download)
*************

<details  style="color:blue">

<summary>__Einstellen des Cassy-Messgerätes:__</summary>

_(muss nicht notiert werden)_

1. Schließe den blauen Anschluss (_I_) an den Minuspol der Spannungsquelle. Der schwarze Anschluss wird an den Widerstand angeschlossen.

2. Schalte das Cassy-Messgerät ein. Im oberen linken Bereich des Fensters sind die messbaren Größen dargestellt. Deaktiviere mit [Cursor-Rad + OK] die Spannung und aktiviere die Stromstärke.

![VGl-Cassy1](https://diversewolken.ddns.net/nextcloud/index.php/s/e7eaHcHB4YkGf95/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Klicke auf das Symbol für Stromstärke (I) und stelle für den (Mess-)Bereich [-0,03A .. 0,03A] ein. Wechsle zurück Anzeige der Stromstärke. Achte auf: __Nullpunkt links__.

![VGl-Cassy2](https://diversewolken.ddns.net/nextcloud/index.php/s/JiSJbjqy3SkS2CN/download)<!-- style="max-width:80%;margin-left:10%" -->

</details>

</p>

</p>

### Einführungsvideo zu Mobile-Cassy 2

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

### 1.7.2 Automatische Messwerterfassung mit Cassy:

In dieser Messreihe wird die Kennlinie vom Cassy-Messgerät automatisch aufgenommen.

1. Schalte die Spannungsquelle ab.

2. Verbinde mit einem weiteren Kabel den @color(roten Pol __U__, red) des Cassy-Gerätes mit einem Kontakt hinter dem Widerstand.

![VGl-Cassy3](https://diversewolken.ddns.net/nextcloud/index.php/s/LxJxpcGsAmAeJJt/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Erweitere deine angezeigten Messwerte auf Spannung U und Stromstärke I. Achte auf __Bereich 0V .. 10V__ und __Nullpunkt links__.

![VGl-Cassy4](https://diversewolken.ddns.net/nextcloud/index.php/s/sXkCT7eGYWyrCYX/download)<!-- style="max-width:80%;margin-left:10%" -->

4. Wechsle zur Anzeige von Spannung und Stromstärke. Schalte die Spannungsquelle ein und vergleiche drei Messwertpaare der angezeigten Daten mit den Daten deiner Messwerttabelle (oben). <br> @color(Stimmen sie überein, red) nimmt Cassy nun korrekt Spannung und Stromstärke auf.

5. Stelle die Spannung an der Spannungsquelle auf 0 V.

6. Wähle nun oben rechts den __Diagramm Modus__. Stelle für die x-Achse die Spannung und für die y-Achse die Stromstärke ein. 

![VGl-Cassy5](https://diversewolken.ddns.net/nextcloud/index.php/s/4nJbMTEEjwz3SJd/download)<!-- style="max-width:80%;margin-left:10%" -->

7. Starte die automatische Messwerterfassung -> Wechsel auf Uhr oben links. 

![VGl-Cassy6](https://diversewolken.ddns.net/nextcloud/index.php/s/cHFbdz2ZQJGFTsE/download)<!-- style="max-width:80%;margin-left:10%" -->

8. Drehe die Spannung an der Spannungsquelle langsam von 0 V -> 10 V und beobache die dargestellten Messwerte. Vergleiche deine Darstellung mit dem hier gezeigten Erwartungsbild.

![VGl-Cassy7](https://diversewolken.ddns.net/nextcloud/index.php/s/f93rWiDbtDkR6Jj/download)<!-- style="max-width:80%;margin-left:10%" -->

9. @color(Dieses Diagramm und dein Messwertdiagramm sollten übereinstimmen., red)

### 1.7.3 Aufgaben zur Berechnung an Kondensatoren

1. Ein Plattenkondensator mit Luft gefüllt besteht aus zwei kreisförmigen Platten mit dem Radius 5,5 cm. Die Platten haben einen Abstand von 7,0 cm. 

1. 1. Ermitteln Sie die Kapazität des Kondensators in pF.

@rangeQuiz2($\hspace{1cm}$ $C$, 1.2, $pF$)

<details style="margin-left:10%">

<summary> Lösung 1.1 </summary>

$$C = 8,86\cdot 10^{-12} \cdot \frac{\pi (5,5\cdot 10^{-3})^2}{7\cdot 10^{-2}} \hspace{1cm} \Big[ \frac{A\cdot s}{V\cdot m} \frac{m^2}{m} = \frac{A\cdot s}{V} = \frac{C}{V} = F \Big]$$

</details>

---

1. 2. Geben Sie zwei Möglichkeiten an, wie die Kapazität vergrößert werden kann, ohne das die geometrischen Größe der Platten verändert wird.

<details style="margin-left:10%">

<summary> Lösung 1.2 </summary>

- Stoff mit höherer Dielektrizitätskonstante einfügen

- Plattenabstand s verkleinern

</details>

---

2. Ein Kondensator hat einen Kapazität von 200µF. Ermitteln Sie die Ladung Q, welche sich auf dem Kondensator befindet, wenn er an eine Spannung von 14 V angeschlossen wird.

@rangeQuiz2($\hspace{1cm}$ $Q$, 2.8E-3, $C$)

---

3. Die in einem Kondensator bei einer Ladespannung von 8,0 V gespeicherte elektrische Feldenergie $E_{Feld}$ soll für die Zündung einer Blitzlichtlampe genutzt werden. Für den Lichtblitz wird eine elektrische Energie von 20 mJ benötigt. Berechnen Sie die Kapazität des Kondensators in der Einheit µF.

@rangeQuiz2($\hspace{1cm}$ $C$, 625, $\mu F$)

<details style="margin-left:10%">

<summary> Lösung 3 </summary>

$$ E_{Feld} = \frac{1}{2} \cdot C \cdot U^2 $$

$$ C = \frac{2 \cdot 0,02 J}{8V^2} = 0,000625 F = 625 µF $$

</details>

## 1.8 Lade und Entladevorgang eines Kondensators

@uhr

<p style="color:blue; margin-right:200px">

Ziel der folgenden Einheit ist die __theoretische, simulierte und experimentelle__ Untersuchung des Ladevorgangs an einem Kondensator.

{{1}}
********
1. __Theorie:__ Schaltplan, physikalische Größen, theoretische Beschreibung
********

{{2}}
********
2. __Simulation:__ Konstruktion des Schaltplans in einer Simulation, Untersuchung der Entladekurve und Einfluss der physikalischen Größen.
********

{{3}}
********
3. __Experiment:__ Aufbau der Schaltung. Messung der relevanten Daten und deren Verarbeitung mit Tablet oder Laptop.
********

{{4}}
********
4. __Auswertung:__ Auswertung der Messungen. Vergleich der experimentelle Daten mit theoretischen und simulierten Ergebnissen.
********

</p>


### 1.8.1 Theoretische Beschreibung des Ladevorgangs an einem Kondensator

__Schaltplan:__ Lade- und Entladevorgang eines Kondensators

<p class="newspaper">

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/mK4zfakTRqYPmG3/download)

<p class="cb">

__Ladekreis__ 

- Wird der Ladekreis geschlossen, so fließen elektrische Ladungen (angetrieben durch die Spannung) von den Polen auf die Platten des Kondensators <br> @color(-> die Ladung $Q$ auf den Kondensatorplatten wird größer, orange)

- da sich gleichnamige Ladungen auf den Kondensatorplatten abstoßen, sinkt die Anzahl der Ladungsträger die pro Sekunde auf die Kondensatorplatten fließen <br> @color(-> während des Ladevorgangs nimmt die Ladestromstärke $I$ ab, orange)

- der zeitliche Verlauf der Stromstärke $I(t)$ kann mit <br> $$ I(t) = I_0 \cdot e^{-\frac{1}{R\cdot C}\cdot t} $$ <br> beschrieben werden. Hierbei gilt $ \hspace{0.5cm} I_0 = \dfrac{U}{R} $

- Beispielhafter Graph $I(t)$ -> die Stromstärke I nimmt mit der Zeit exponentiell ab <br> ![Ladekurve_1](https://diversewolken.ddns.net/nextcloud/index.php/s/knoEKKZaKBL9q6w/download)

</p>

</p>

### 1.8.2. Simulation

_Aufgaben:_ 

1. Erstelle anhand des Schaltplans (siehe 1.8.1) in der Simulation einen Lade- und Entladekreis für einen Kondensator. <br> Link: [Simulation-Ladekurve](https://phet.colorado.edu/sims/html/circuit-construction-kit-ac/latest/circuit-construction-kit-ac_all.html?locale=de) <br>  Wähle in der Simulation die Option __Labor__.

<details style="margin-left:10%">

<summary> Lösungshinweis bei Problemen </summary>

![LösungLadekurve](https://diversewolken.ddns.net/nextcloud/index.php/s/gsJ8NSCt5DsgXcm/download)

</details>

---

2. Beobachte, wie die Stromstärke mit zunehmender Ladung auf den Kondensatorplatten abnimmt.

---

3. Nutze das Stromstärke Diagramm um eine simulierte Messung durchzuführen. Erstelle davon einen Screenshot.

---

### Tutorial Oszilloskop-Modus mit Cassy 2

!?[Tutorial Oszilloskop](https://www.youtube.com/watch?v=5vfNUj-2P4M)

### Experimentierüberblick

__Lernziele:__

- Cassy mit Tablet verbinden

- Ladekurve im Cassy mit Osszilloskopmodus aufnehmen

- Zeitkonstante berechnen

- Messparameter einstellen lernen (ohne Trigger)

- gespeicherte Ladung bestimmen

- Auswertung der Messdaten

__Physikalische Inhalte:__

- Kondensator C = 4600 µF, Ohmscher Widerstand R = 1 kOhm

- Zeitkonstante für Laden/Entladen $\tau=R\cdot C$

- Ladungsbestimmung via Berechnung $Q=C\cdot U$

- Ladungsbestimmung bei verschiedenen Spannungen mit Hilfe der Ladekurve

- Vergleichendes Diagramm erstellen

__Lernhilfen:__

- LB S. 75 Protokollgestaltung

- LB S. 76/77 Messfehler bei physikalischen Messungen

- Anleitung für Verbindung von Tablet und Cassy

- Anleitung zur Steuerung von Cassy

- Anleitung zum Aufbauen des Versuchs

## 1.9 Experiment Entladevorgang eines Kondensators

__Aufgabenstellung:__ Untersuche den Entladevorgang eines Kondesators mit Hilfe der elektronischen Messwerterfassung ***Mobile Cassy 2***.

__Teilaufgaben:__ (_können_ in selbst gewählter Reihenfolge bearbeitet werden)

- [ ] Inhalten eines Protokolls notieren

- [ ] Vorbetrachtungen zum Versuch vornehmen und notieren

- [ ] ***Mobile Cassy 2*** mit Tablet verbinden

- [ ] Einstellen der Parameter am Cassy

- [ ] Schaltkreis zur Messung aufbauen @color(und von Lehrkraft abnehmen lassen, red)

- [ ] Messwerte aufzeichnen

- [ ] Daten auswerten und Ergebnisse analysieren

- [ ] Ergebnisse formulieren

### Inhalte eines Protokolls

Nutzen Sie Lehrbuch Seite 75 und erarbeiten Sie sich die wesentlichen Inhalte eines Protokolls

### Vorbetrachtungen zum Versuch

<p class="newspaper">

__Schaltplan:__

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/JqJRbJpBMJXNwTq/download)

<p class="cb">

__Ladekreis__ 

Der Kondensator wird in dieser Schaltung direkt über die Spannungsquelle und ohne ohmschen Widerstand aufgeladen.

__Entladekreis:__

Wird der Entladekreis geschlossen, fließt die auf dem Kondensator gespeicherte Ladung $Q$ über den ohmschen Widerstand $R$ ab. Dabei wird mit der elektronischen Messwerterfassung _Cassy_ der Entladestrom $I$ in Abhängigkeit der Zeit $t$ aufgenommen. Die gesamte Messzeit wird mit $T$ bezeichnet (s.u.).

{{1}}
*****
__Ermittlung der Ladung $\,Q$:__

Die vom Kondensator abgeflossene Ladung $Q$ entspricht im @color(Zeit-Stromstärke-Diagramm, blue) der <bdi style="color:red"> __Fläche unter dem Graphen $I(t)$__</bdi>.
*****

{{1-2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/Q9MwZdw5ZxwfrcN/download)<!-- style="max-width:80%; margin:5%"-->
*****

{{2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/GSN44xxcqTH4HH6/download)<!-- style="max-width:80%; margin:5%"-->

Die Fläche unter dem $I(t)$ Graphen kann mit Hilfe des Cassy-Messgerätes ausgewertet werden.

*****

{{3}}
*****
__Ermittlung der Messdauer $T$ für Cassy:__

Für die Kombination aus Kondensator (Kapazität $C$) und ohmscher Widerstand (Widerstand $R$) kann eine Zeitkonstante $\tau$ ermittelt werden: 

$$ \boxed{\tau = R \cdot C} \Rightarrow \boxed{T = 4 \cdot \tau} $$

Als Messdauer $T$ für die elektronische Erfassung wird eine Zeit von @color($4\tau$,red) empfohlen. Nach dieser Zeit sind ca. $98,2\%$  der Gesamtladung Q abgeflossen.
*****

</p>

</p>

### Anleitung zur Verbindung von Cassy und Tablet

__Grundlage:__ Jedes __Mobile Cassy 2__-Messgerät (im Folgenden mit _Cassy_ bezeichnet) kann mit Hilfe einer W-Lan Verbindung über das Tablet ferngestuert werden. Dabei können Messparameter eingestellt, Messungen gestartet und Messdaten abgespeichert werden. Hier wird das Tablet mit dem Cassy verbunden.

__Arbeitsablauf:__

- nach Einschalten von _Cassy_ baut das Gerät selbstständig eine W-Lan Verbinung auf

- wechseln Sie auf dem Cassy zum Menu Einstellungen (oben rechts) 

- wählen Sie QR-Code anzeigen, wechseln Sie zu AP_Daten und scannen Sie den angezeigten QR-Code mit dem Tablet -> das Tablet wird sich mit dem Cassy verbinden

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/cbw8JJBd7AAetEz/download)<!-- style="max-width:300px; margin-left:20%"-->

- wenn ihr Tablet mit dem _Cassy_-WLan verbunden ist, öffnen Sie einen neuen Tab im Safari-Webbrowser und öffnen Sie folgende Adresse [http://10.10.10.1](http://10.10.10.1)

![Cassy-WLan](https://diversewolken.ddns.net/nextcloud/index.php/s/zgynA6RKTTEaM4Y/download)<!-- style="max-width:80%; margin:5%"-->

- zu sehen ist die Live-Anzeige des Spannungssensors <br>-> aktivieren Sie am Cassy die Stromstärkemessung und deaktivieren Sie die Spannungsmessung <br> -> Überprüfen Sie die Veränderung auf Ihrem Tablet

![Cassy-WLan2](https://diversewolken.ddns.net/nextcloud/index.php/s/8ZjcN5DZqk6frXw/download)<!-- style="max-width:80%; margin:5%"-->

### Einstellen der Messparameter am Cassy

__Grundlage:__ Hier werden die Messparameter eingestellt

__Arbeitsablauf:__

- wechseln Sie auf der linken Seite zu Einstellungen

- hier müssen Sie den Messbereich für die Stromstärke einstellen __0,03 A__ und den Nullpunkt (des Diagramms) auf __links__ setzen(_Hinweis: diese Einstellung kann auch im Cassy direkt vorgenommen werden_)

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/KQLjMB5CoYRR34o/download)<!-- style="max-width:80%; margin:5%"-->

- wechseln Sie auf der linken Seite zu ***Diagramm*** und vergleichen Sie Ihre Anzeige

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9APdepf3in8wQ86/download)<!-- style="max-width:80%; margin:5%"-->

### Aufbau der Messchaltung

$ \red{\boxed{\mathrm{Es\ muss\ keine\ Gewalt\ angewendet\ werden.}}}$

__Grundlage:__ Für diesen Versuch ist der Schaltplan in den Vorbetrachtungen des Versuchs gezeichnet. 

__Materialien:__ Sie erhalten einen Kondensator mit der Kapazität $4700 \mu F$ und einen ohmschen Widerstand mit $1000 \Omega$.

---

<H4>Schaltung: </H4>

__Ladekreis:__

- die Pole der Spannungsquelle werden über den Wechselschalter direkt an den Kondensator angeschlossen

<p style="margin-left:5%">

$ \red{\boxed{\mathrm{ACHTUNG:\ + Platte\ des\ Kondensators\ mit\ \oplus der\ Spannungs-Quelle\ verbinden}}}$

<details>

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_1](https://diversewolken.ddns.net/nextcloud/index.php/s/SMpRaWdBfXBPDSW/download)<!-- style="max-width:80%; margin:5%"-->

</details>

</p>

---

Entladekreis:

- der Widerstand wird in Reihe zum Kondensator angeschlossen

- in Reihe zum Widerstand folgt das _Cassy_

- achten Sie beim Anschluss des _Cassy_, dass der blaue Anschluss in Richtung $\ominus$-Pol der Spannungsquelle und der schwarze Anschluss in Richtung des $\oplus$-Pols der Spannungsquelle zeigt

<details style="margin-left:5%">

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_2](https://diversewolken.ddns.net/nextcloud/index.php/s/m2KAErdZKRTMFi5/download)<!-- style="max-width:80%; margin:5%"-->

</details>

- lassen Sie sich die Schaltung von der Lehrkraft abnehmen

### Aufnahme der Entladekurve

$ \red{\boxed{\mathrm{Die Schaltung\ muss\ abgenommen\ worden\ sein.}}}$

__Grundlage:__ Hier wird der Kondensator zunächst geladen. Dann wird die automatische Messung mit dem _Cassy_ gestartet und die Entladekurve wird aufgezeichnet.

- legen Sie den Wechselschalter in die Ladeposition

- schalten Sie die Spannungsquelle ein und wählen eine Spannung von 10 V

- starten Sie anschließend die Messung auf dem _Cassy_ indem Sie oben auf __"Messzeit nicht vorgegeben"__ klicken, legen Sie anschließend den Schalter um

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/dDiiE3cYDgGqM3W/download)<!-- style="max-width:80%; margin:5%"-->

- stoppen Sie die Messung nach etwa $T=4\tau$ (4 charaktieristischen Zeiteinheiten)

- achten Sie darauf, dass die eigentliche Entladung erst beginnt, wenn Sie den Schalter umlegen


### Auswertung einer Messung

__Grundlage:__ Hier werden die Messdaten ausgewertet.

__Ermittlung der geflossenen Ladung:__

- wählen Sie unter Auswertungen (unterhalb des Diagramms) den Menupunkt _"Fläche zur x-Achse"_

- angezeigt wird die geflossene Ladung in der Einheit $A\cdot s = C$ 

- notieren Sie den Messwert

![Cassy_-_Auswertung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/BXHx8eeCy8oXBSD/download)<!-- style="max-width:80%; margin:5%"-->

__Diagramm zeichnen aus einzelnen Messwerten:__

- wechseln Sie auf der linken Seit zum Reiter __Tabelle__

- notieren Sie in einer Messwerttabelle __t in s__ und __I in A__ und übernehmen Sie 10 charakteristische Messwerte

- zeichnen Sie anschließend den I(t)-Graph für Ihre Messwerte in das Protokoll

## 1.10 Untersuchungen am Entladevorgang eines Kondensators

@timer(60,00)

### Teil 1 - Wiederholung (ca. 20 min)

<details>

<summary>
</summary>

<p style="margin-left:5%">

__Aufgabenstellung:__ 

- [ ] @color(Bauen Sie den Entladekreis eines Kondensators anhand der Erklärungen 1.9 auf. , blue)

- [ ] @color(Lassen Sie sich die Schaltung abnehmen. ,red)

- [ ] @color(Ermitteln Sie die auf dem Kondensator gespeicherte elektrische Ladung. ,blue)

- [ ] @color(Überprüfe Sie mit Hilfe der Kontrollboxen Ihre Messwerte. Achten Sie dabei auf die geforderten Einheiten. ,blue)

__Daten/Messwerte zur Kontrolle:__ 

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 1000 , $\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4.7 , $mF$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 4.7 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 18.8 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.01 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

</p>

</details>

---

### Teil 2 - neuer Widerstand (ca. 20min)

<details>

<summary>
</summary>

<p style="margin-left:5%">

__Aufgabenstellung:__ 

- [ ] @color(Lassen Sie sich von der Lehrkraft einen neuen Widerstand $470\Omega$ aushändigen. , blue)

- [ ] @color(Tauschen Sie die Widerstände aus., blue)

- [ ] @color(Widerholen Sie den Experimentierablauf. Überprüfen Sie die neuen Parameter anhand der Kontrollwerte., blue)

- [ ] @color(Notieren Sie sich Ihre Werte zur Messung mit dem neuen Widerstand., red)

__Daten/Messwerte zur Kontrolle:__ 

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 0.47 , $k\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4700 , $\mu F$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 2.209 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 8.836 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.0213 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

- [ ] @color(Sollten Sie noch mehr als 30min Restzeit zur Verfügung haben: Wiederholen Sie die Messung für einen $2.2 k\Omega$-Widerstand., blue)

<details>

<summary> __Daten/Messwerte zur Kontrolle:__ </summary>

<p style="margin-left:5%">

Ladespannung U:

@rangeQuiz2(U, 10 , $V$)

Elektrischer Widerstand: 

@rangeQuiz2(R, 2200 , $\Omega$)

Kapazität des Kondensators:

@rangeQuiz2(C, 4700 , $\mu F$)

Zeitkonstante der RC-Reihenschaltung (_RC: Widerstand-Kondensator_)

@rangeQuiz2($\tau$, 10.34 , $s$)

Vorgegebene Messzeit für die Entladung:

@rangeQuiz20($T$, 41.36 , $s$)

Maximalwert der elektrischen Stromstärke:

@rangeQuiz20($I$, 0.0045 , $A$)

Während Messzeit abgeflossene Ladung:

@rangeQuiz20($Q$, 0.0475 , $C$)

</p>

</details>

</p>

</details>

---

### Teil 3 - Vergleich (mind. 20 min)

<details>

<summary>
</summary>

<p style="margin:5%">

- [ ] @color(Vergleichen Sie für beide Messungen folgende Werte in einer Tabelle. Ergänzen Sie diese Tabelle in Ihren Aufzeichnungen. , blue)


{{0-1}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | ..                 | .. | .. | .. | .. |
| Teil 2  | ..                 | .. | .. | .. | .. |
| @color(_optional_, darkgrey) | ..                 | .. | .. | .. | .. |
************

{{1-2}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | .. | .. | .. |
| Teil 2  | 10                 | 470 | .. | .. | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | .. | .. | .. |
************

{{2-3}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | .. | .. |
| Teil 2  | 10                 | 470 | 0,021 | .. | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | .. | .. |
************

{{3-4}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | 18,8 | .. |
| Teil 2  | 10                 | 470 | 0,021 | 8,8 | .. |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | 41,4 | .. |
************

{{4}}
************
<!-- data-type="none" -->
|         | Ladespannung in V  | Widerstand in $\Omega$ | Maximale Stromstärke | Entladezeit in s | Gespeicherte Ladung in C | 
|         | $U$ in V  | $R$ in $\Omega$ | $I_{max}$ in A | $T$ in s | $Q$ in C | 
| Teil 1  | 10                 | 1000 | 0,01 | 18,8 | 0,047 |
| Teil 2  | 10                 | 470 | 0,021 | 8,8 | 0,047 |
| @color(_optional_, darkgrey) | 10                 | 2200 | 0,0045 | 41,4 | 0,047 |
************

- [ ] <bdi style="color:blue">Überprüfen Sie den Zusammenhang von Ladespannung, Kapazität und gespeicherter Ladung. Formulieren Sie ein Ergebnis.</bdi> 


{{5}}
********
@color(Der Widerstand hat keinen Einfluss auf die gespeicherte Ladung. Die gespeicherte Ladung kann mit der Formel $Q=C\cdot U$ berechnet werden. , orange)
********

- [ ] <bdi style="color:blue">Stellen Sie anhand Ihrer Daten eine Vermutung über den Einfluss des eingesetzten Widerstands $R$ beim Entladen des Kondensators auf. Gehen Sie dabei auf Ladespannung, Entladezeit, maximale Stromstärke und gespeicherte Ladung ein. Formulieren Sie ein Ergebnis</bdi>

{{6}}
********
@color(Je größer der Widerstand desto langsamer erfolgt die Entladung. Die Entladezeit kann mit $T=4\cdot \tau = 4 \cdot R \cdot C$ berechnet werden. , orange)
********


- [ ] @color(Überprüfen Sie den Zusammenhang von Ladespannung Widerstand und maximaler Stromstärke. Formulieren Sie ein Ergebnis, blue)

{{7}}
********
@color(Der Zusammenhang von Widerstand R Ladespannung U und maximaler Stromstärke folgt dem ohmschen Gesetz $R=\frac{U}{I_{max}}$. , orange)
********


</p>

</details>

## Rückgabe Protokoll 11.1

@uhr

<details>

<summary> Notenspiegel </summary>

![Verteilung](https://diversewolken.ddns.net/nextcloud/index.php/s/LDXKwH4bE47Ak5M/download)

__Korrekturzeichen:__

- __ug:__ ungenau

- __uv:__ unvollständig

- __Bg:__ fehlende oder falsche Begründung

</details>

# Grundkurs Physik 2024/2025 - LB III Das Magnetische Feld

![MagnetischesFeld](https://www.mozaweb.com/de/mozaik3D/FOL/termeszet/foldi_magneses_mezo/960.jpg)

{{1}}
***********
> __Das magnetische Feld__ ist, ebenso wie das elektrische Feld, @color(ein Modell, red) um den Einfluss von @color(magnetischen Kräften im Raum um einen Magneten, blue) darzustellen.
***********

## 1.1 Vergleich von elektrischen und magnetischen Feldern

<p class="newspaper3">

__Name__

<p class="cb">

__Elektrisches Feld__


<p class="cb">

__Magnetisches Feld__

</p>

</p>

</p>

---

<p class="newspaper3">

_Ursache sind_

<p class="cb">

{1}{__elektrische Ladungen Q__}

<p class="cb">

{2}{__Dauermagnete__ und __bewegte elektrische Ladungen (elektrischer Strom)__}

</p>

</p>

</p>

---

<p class="newspaper3">

_Darstellung durch_

<p class="cb">
{{3}}
********
Elektrische Feldlinien

![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)
********
<p class="cb">
{{4}}
********
Magnetische Feldlinien

![WikimediaMagnetischesFeld](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0c/VFPt_cylindrical_magnet_thumb.svg/1280px-VFPt_cylindrical_magnet_thumb.svg.png)
********
</p>

</p>

</p>

---

<p class="newspaper3">

_Verdeutlicht wird die_

<p class="cb">

{5}{__Wirkung der elektrischen Kraft__ auf eine <span style="color:orange">positive Probeladung</span>.}

<p class="cb">

{6}{__Wirkung der magnetischen Kraft__ auf einen @color(anderen Magneten,orange) oder auf @color(eine bewegte Ladung, orange).}

</p>

</p>

</p>

---

<p class="newspaper3">

_Eigenschaften sind_

<p class="cb">
{{7}}
********
- Feldlinien verlaufen von @color($\oplus$, red) nach @color($\ominus$, blue)

<br>

- elektrischen Kräfte wirken __entlang (d.h. tangetial)__ der Feldlinien

- je dichter die Feldlinien, desto größer die Kraft
********

<p class="cb">

{{8}}
********
- Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, blue)

- magnetische Kräfte mit Hilfe der Feldlinien ableitbar (siehe __Lorentzkraft__)

- je dichter die Feldlinien, desto größer die Kraft

- Feldlinien sind @color(__immer__,red) geschlossen (kein Anfang oder Ende)

- sie verlaufen außerhalb des Magneten von @color(__N__,red)->@color(__S__, blue) und innerhalb von @color(__S__, blue)->@color(__N__,red)
********

</p>

</p>

</p>

---

{{9}}
********

@color(Selbstständiges Arbeiten, blue)

<p style="margin-left:5%">

<br>

@color(__Aufgabe:1.1__ Ergänze diese Übersicht zu magnetischen Feldern durch eine eigene Recherche. Zeichne dazu einige Arten von Magneten und die zugehörigen Felder in deinen Hefter., blue)

<br>

@color(__Aufgabe 1.2.__ Ergänze diese Übersicht mit zwei Beispielen für homogene magnetische Felder. Wiederhole die Definition von __homogen__., blue)

<br>

@color(__Aufgabe 1.3.__ Ergänze diese Übersicht mit Erklärungen zur anziehenden und abstoßenden Kraftwirkung zwischen Magneten., blue)

<br>

<bdi style="color:blue">__Aufgabe 1.4.__ Notiere Stichpunkte zum Erdmagnetfeld. Gehe dabei auf die Lage der magnetischen Pole, das Feldlinienbild und die Funktion als Schutzschild für die Erde ein.</bdi>

<br><br>

@color(Nutze hierfür z.B. folgende Quellen:, blue)

<br>

- [Arten von Magneten](https://www.abi-physik.de/buch/das-magnetfeld/dauer--und-elektromagnete/)

- [Homogene Felder](https://www.abi-physik.de/buch/das-magnetfeld/homogenes-magnetfeld/)

- LB S. 102, 103, 104

</p>

---

********


{{10}}
********
!?[XeniusMagnetismusUnsichtbareKraft](https://www.youtube.com/watch?v=mlt9JcRpzYg)
********

{{11}}
********
<p class="newspaper3">

_Arten von Feldern_

<p class="cb">

homogenes Feld (im Plattenkondensator)

![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)


<p class="cb">

homogenes Feld (im Inneren eines Hufeisenmagneten)

![HomogenesFeld](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-spule.png)

homogenes Feld (im Inneren einer Spule)

![HomogenesFeldHufeisenmagnet](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-1.png)

</p>

</p>

</p>

---
********

### Aufgaben zur Überprüfung

1. Das Magnetfeld der Erde gleich dem eines/r .. <br>
_Hinweis: Die folgenden Formen der magnetischen Felder solltest du im Hefter haben._

<!-- data-solution-button="off" -->
[( )] Hufeisenmagneten
[(x)] Stabmagneten
[( )] Stromdurchflossenen Leites
[( )] Stromdurchflossenen Spule

---

2. Das hier gezeigte Magnetfeld gehört zu einem/r

![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)

<!-- data-solution-button="off" -->
[(x)] Hufeisenmagneten
[( )] Stabmagneten
[( )] Stromdurchflossenen Leiters
[( )] Stromdurchflossenen Spule

---

3. Welche der folgenden Aussagen über das Erdmagnetfeld ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Der magnetische Nordpol der Erde befindet sich nahe dem geografischen Südpol.
[[ ]] Das Erdmagnetfeld schützt die Erde vor kosmischer Strahlung.
[[x]] Die Stärke des Erdmagnetfelds ist überall auf der Erde gleich.
[[ ]] Die Polarität des Erdmagnetfelds kann sich im Laufe der Zeit umkehren.

---

4. Erkunden Sie, ob auch andere Planeten ein Magnetfeld besitzen.

---

5. Markieren Sie das Magnetfeld eines stromdurchflossenen Leiters.

<!-- data-solution-button="off" -->
[( )] ![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)
[( )] ![Stabmagnet](https://www.abi-physik.de/images/devpages/stabmagnet.png)
[(x)] ![Leiter](https://www.abi-physik.de/images/devpages/leiter.png)
[( )] ![Spule](https://www.abi-physik.de/images/devpages/spule.png)

---

6. Dauermagnete (Permanentmagnete) sind Stoffe, die ihre Umgebung dauerhaft magnetisch beeinflussen. Sie bestehen aus.. (_Vgl. LB S. 102_)

<!-- data-solution-button="off" -->
[[ ]] Magnesium
[[x]] Eisen
[[ ]] Aluminium
[[ ]] Zink
[[ ]] Kupfer
[[ ]] Zinn
[[x]] Cobalt
[[x]] Nickel

---

7. Der magnetische Nordpol der Erde befindet sich in der Nähe des

<!-- data-solution-button="off" -->
[( )] geographischen Nordpols
[(x)] geographischen Südpols
[( )] Nullmeridians
[( )] Äquators

---

8. Durch welche Anordnung könnten die abgebildeten Magnetfelder erzeugt worden sein (siehe LB S. 124/Aufgabe 27).

a)

<!-- data-solution-button="off" -->
[[ ]] Hufeisenmagneten
[[x]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

b)

<!-- data-solution-button="off" -->
[[x]] Hufeisenmagneten
[[ ]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

---

9. Welcher der folgenden Prozesse erzeugt kein Magnetfeld?

<!-- data-solution-button="off" -->
[[ ]] Ein elektrisch geladenes Teilchen bewegt sich mit konstanter Geschwindigkeit.
[[ ]] Ein stromdurchflossener Leiter.
[[x]] Ein statischer elektrischer Dipol.
[[ ]] Eine Spule mit wechselndem Strom.

---

10. Welche Aussage über Magnetfeldlinien ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Magnetfeldlinien sind geschlossene Kurven und haben keinen Anfang und kein Ende.
[[ ]] Magnetfeldlinien verlaufen außerhalb eines Magneten vom Nordpol zum Südpol.
[[x]] Magnetfeldlinien können sich in einem homogenen Magnetfeld überschneiden.
[[ ]] Die Dichte der Magnetfeldlinien gibt die Stärke des Magnetfeldes an.

11. Welche der folgenden Aussagen ist korrekt?

<!-- data-solution-button="off" -->
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist entlang der Leiterachse ausgerichtet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist radial nach außen gerichtet.
[[x]] Das Magnetfeld um einen stromdurchflossenen Leiter ist kreisförmig und konzentrisch um den Leiter angeordnet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter existiert nur, wenn der Strom sinusförmig wechselt.


## 1.2 Berechnungen des magnetischen Feldes - Die magnetische Flussdichte B

<p class="newspaper">

__Magnetisches Feld__

<p class="cb">

__Elektrisches Feld__

</p>

</p>

---

{{1}}
********
<p class="newspaper">

Die __magnetische Flussdichte__ $B$ beschreibt die Stärke und Richtung des magnetischen Feldes in einem Punkt. Sie wird definiert durch die Kraft auf eine bewegte Ladung oder einen stromdurchflossenen Leiter:

$$ \boxed{B = \frac{F}{I \cdot l}}$$

- $F$: Magnetische Kraft [Newton, $N$]
- $I$: Stromstärke [Ampere, $A$]
- $l$: Leiterlänge [Meter, $m$]

<p class="cb">

Die elektrische Feldstärke $E$ berechnet sich aus der Kraft $F$ auf eine elektrische Ladung $Q$.

$$ \boxed{E = \frac{F}{Q}} $$

- $F$: Elektrische Kraft [Newton, $N$]
- $Q$: Ladung im Feld [Coulomb, $C$]


</p>

</p>

---
********

{{2}}
********
<p class="newspaper">

__Einheit__: [1 Tesla = 1 T]

$$\Big[T=\dfrac{N}{A \cdot m}\Big]$$

<p class="cb">

__Einheit__: $$\Big[\dfrac{N}{C}=\dfrac{V}{m}\Big]$$

</p>

</p>

---
********


### 1.2.2 Übung: Berechnung der magnetischen Flussdichte

<bdi style="color:blue">__Löse die folgenden Aufgaben, indem du die gegebene Formel anwendest__.</bdi>

#### Aufgabe 1.2.1
Ein gerader Leiter mit einer Länge von 2 m wird von einem Strom von 5 A durchflossen. Er befindet sich in einem Magnetfeld mit einer Flussdichte $B$. Die magnetische Kraft auf den Leiter beträgt 0,5 N. Berechne $B$!

@rangeQuiz2(B, 0.05, T)

#### Aufgabe 1.2.2
Ein stromdurchflossener Leiter (Länge $ℓ = 1,5 \, m$, Stromstärke $I = 3 \, A$) befindet sich in einem Magnetfeld mit $B = 0,2 \, T$. Berechne die magnetische Kraft $F$ auf den Leiter.

@rangeQuiz2(F, 0.9, N)


#### Aufgabe 1.2.3
Ein Leiter der Länge $ℓ = 3 \, m$ und Stromstärke $I = 2 \, A$ erfährt eine magnetische Kraft von $F = 0,6 \, N$. Berechne die magnetische Flussdichte $B$.

@rangeQuiz2(B, 0.1, T)

#### Aufgabe 1.2.4 

__Analyse von Änderungen__

Ein stromdurchflossener Leiter befindet sich in einem Magnetfeld. Die Stromstärke $I$ wird verdoppelt, während die Leiterlänge $ℓ$ und die magnetische Flussdichte $B$ unverändert bleiben. Wie ändert sich die magnetische Kraft $F$?

<!-- data-solution-button="off" -->
[[ ]] Sie bleibt gleich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie halbiert sich.  
[[ ]] Sie vervierfacht sich. 

---

<!-- data-solution-button="off" -->
Die magnetische Flussdichte $B$ wird auf das Doppelte erhöht, während Stromstärke $I$ und Leiterlänge $ℓ$ konstant bleiben. Was passiert mit der magnetischen Kraft $F$?

[[ ]] Sie bleibt gleich.  
[[ ]] Sie halbiert sich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie vervierfacht sich.  




## 1.3 Berechnungen der magnetischen Flussdichte B in einer langen Spule

<p class="newspaper">

__Magnetisches Feld__

![FeldInSpule](https://diversewolken.ddns.net/nextcloud/index.php/s/z7CNJzqkxjf4bf7/download)

<p class="cb">

__Elektrisches Feld__

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

</p>

</p>

---

{{1}}
*****
<bdi style="color:red"> Die Felder in einer langen Spule (magnetisches Feld) und einem einem Kondensator (elektrisches Feld) sind näherungsweise __homogen__. </bdi>

---
*****



{{2}}
********

<p class="newspaper">

Die magnetische Flussdichte $B$ innerhalb einer __langen, stromdurchflossenen Spule__ wird durch folgende Formel beschrieben:

$$
\boxed{B = \mu_0 \cdot \mu_r \cdot \frac{N\cdot I}{ℓ}}
$$

- $B$: Magnetische Flussdichte [ Tesla, $T$]
- $\mu_0$: Magnetische Feldkonstante $\boxed{\mu_0 = 1,26 \cdot 10^{-6} \frac{V \cdot s}{A \cdot m}}$
- $\mu_r$: Magnetische Permeabilität des Mediums [einheitenlos -> FS S.54]
- $N$: Anzahl der Windungen der Spule
- $ℓ$: Länge der Spule [Meter, $m$]
- $I$: Stromstärke [Ampere, $A$]

<p class="cb">

{{3}}
********

Die elektrische Feldstärke E innerhalb eines Plattenkondensators wird durch folgende Formel beschrieben:

$$ \boxed{E = \dfrac{U}{d}} $$

- $U$: Spannung zwischen den Platten $\big[ V \big]$ 
- $d$: Abstand der Platten $\big[ m \big]$ 

********

</p>

</p>

********

### Aufgaben zur B-Feld Berechnung an Spulen

<bdi style="color:blue">__Löse die folgenden Aufgaben, indem du die gegebene Formel zur _langen Spule_ anwendest__.</bdi>

#### Aufgabe 1.3.1  
Eine Spule hat $N = 800$ Windungen und eine Länge von $ℓ = 0,4 \, m$. Sie wird von einem Strom mit $I = 3 \, A$ durchflossen. Die Spule ist luftgefüllt ($\mu_r = 1$). Berechne die magnetische Flussdichte $B$ im Inneren der Spule.  

@rangeQuiz2(B, 0.00754, T)

#### Aufgabe 1.3.2  
Eine Spule mit $N = 500$ Windungen und $ℓ = 0,5 \, m$ erzeugt eine magnetische Flussdichte von $B = 2,51 \, mT$. Berechne die Stromstärke $I$, die durch die Spule fließt.  

@rangeQuiz2(I, 2, A)

#### Aufgabe 1.3.3  

Eine Spule hat $N = 1000$ Windungen und eine Länge von $ℓ = 1 \, m$. Der Strom beträgt $I = 4 \, A$. Wie verändert sich die magnetische Flussdichte $B$, wenn: 

1. Die Anzahl der Windungen $N$ verdoppelt wird?  
2. Der Strom $I$ halbiert wird?  
3. Die Länge der Spule $ℓ$ verdreifacht wird?

<!-- data-solution-button="off" -->
[[x]] 1. Verdoppelt sich, 2. halbiert sich, 3. verringert sich auf ein Drittel.  
[[ ]] 1. Verdoppelt sich, 2. bleibt gleich, 3. verringert sich auf die Hälfte.  
[[ ]] 1. Bleibt gleich, 2. halbiert sich, 3. verringert sich auf ein Viertel.  
[[ ]] 1. Verringert sich, 2. bleibt gleich, 3. bleibt gleich.

#### Aufgabe 1.3.4  

Eine luftgefüllte Spule hat $N = 1000$ Windungen, $ℓ = 0,8 \, m$ und $I = 2 \, A$. Im Innenraum der Spule wird ein Material mit einer unbekannten relativen Permeabilität $\mu_r$ ersetzt, wodurch die magnetische Flussdichte $B$ auf $1,7 \, T$ ansteigt. Berechne $\mu_r$.  

@rangeQuiz2($\mu_r$, 539.7, -)

Um welchen ferromagnetischen Stoff könnte es sich handeln?

<!-- data-solution-button="off" -->
[[Eisen]]

#### Aufgabe 1.3.5

Die magnetische Flussdichte $B$ in einer luftgefüllten Spule beträgt $1,26 \, mT$. Die Spule hat $N = 400$ Windungen und eine Länge von $ℓ = 0,5 \, m$. Berechne den Strom $I$, der durch die Spule fließt?  

@rangeQuiz2(I, 1.25, A)

### Übungen zum magnetischen Feld allgemein

@timer(15,00)

<br>

<br>

<br>

__Grundwissen Magnetismus__

??[LueckentextMagnetismus](https://learningapps.org/1319776)

__Grundwissen magnetisches Feld__

??[LueckentextMagnetfeld](https://learningapps.org/35523603)

__Fragen zu magnetischen Experimenten__

??[MagnetischeExperimente](https://www.leifiphysik.de/elektrizitaetslehre/permanentmagnetismus/aufgabe/quiz-zu-magnetischen-eigenschaften)

## 1.4 Schülerexperiment: Messungen der magnetischen Flussdichte

__Teil 1: Bestimmung der magnetischen Flussdichte des Erdmagnetfeldes__

> Aufgabe: Bestimme mit Hilfe des Magnetfeldsensors an dem Cassy-Gerät die magnetische Flussdichte $B_{Erde}$ des Erdmagnetfeldes.

__Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$__

> Aufgabe: Bestimme die magnetische Feldkonstante $\mu_0$ mit Hilfe der Messung der magnetischen Flussdichte B an einer Spule.

@color(Führe die beiden Messungen durch. Erstelle jeweils ein Kurzprotokoll, blue).

_optional (min. 15min)_

__Teil 3: Überprüfung der Proportionalität von $B$ ~ $N$__

> Aufgabe: Überprüfe experimentell die Proportionalität der magnetischen Flussdichte $B$ und der Windungszahl $N$


### Experiment Teil 1: Erdmagnetfeld

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__1.1 Vorbereitung:__

> - recherchiere im Internet die Stärke der magnetischen Flussdichte $B_{Erde}$ des Erdmagnetfeldes in Deutschland
>
> - notiere den Wert und die Quelle
>
> $$ B_{Erde} = ... $$
>
> - erhalte von der Lehrkraft einen Magnetfeldsensor und ein Cassy-Messgerät
>
> - schließe de Magnetfeldsensor an das Cassy-Messgerät (__linke Seite -> Kanal A__) an und lass dir die aktuelle magnetische Flussdichte B anzeigen
>
> - wechsle im Menu zu den Einstellungen von B und
>
>      - wähle als Messmethode axial
>
>      - wähle als Messbereich 0 - 10 mT

__1.2 Durchführung:__

> - bestimme mit dem Cassy-Messgerät die natürliche magnetische Feldstärke an zwei Punkten im Physikraum und an anderen Orten im Schulhaus
>
> - notiere dir kurz Stichpunkte zu deinem Messablauf
>
> - erstelle dabei folgende Tabelle
>
> - fülle die Messwerte mit den Ergebnissen

__1.3 Ergebnisse:__

|    | Ort der Messung | magnetische Flussdichte B |
|:--:|:---------------:|:-------------------------:|
| 1  | |
| 2  | |
| 3  | |
| 4  | |

__1.4 Auswertung:__

> - ermittle den Mittelwert deiner Messungen und notiere dein Ergebnis:
>
> Das natürliche Magnetfeld der Erde hat am Gym.Klotzsche den mittleren Wert:
> $$B_{Erde} \approx ... $$
>
> Vergleiche den Wert mit dem recherchierten Ergebnis aus den Vorbetrachtungen in 1.1 in einem Satz.

### Experiment Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__2.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - stelle die Formel nach $\mu_0$ um und notiere die Berechnungsvorschrift für $\mu_0$
>
> $$ \boxed{\mu_0 = ... } $$
>
> - notiere die Bedeutung der Formelzeichen
>
> Die magnetische Feldkonstante $\mu_0$ hat den theoretischen Wert
>
> $$ \boxed{\mu_0 = ... } $$
>
> - emittle mit Hilfe der Formelsammlung den Wert von $\mu_0$ und notiere ihn
>
>> Um die magnetische Feldkonstante $\mu_0$ zu bestimmen, müssen die fehlenden Werte der Formel aus 1.1 gemessen werden. Um den Einfluss von Messfehlern zu reduzieren, wird die Messung für __dreimal__ durchgeführt.

__2.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - nutze in den Einstellungen des Cassy-Messgerätes zur magnetischen Flussdichte B die Möglichekeit, dass Erdmagnetfeld zu korrigieren: Wähle dazu: __Korrektur: Offset und stelle den Wert so ein, dass das Gerät ungefähr $\pm$ 0,01 mT anzeigt. Der Offset muss mit OK bestätigt werden (kleines Häkchen).__
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BestimmungMu0](https://diversewolken.ddns.net/nextcloud/index.php/s/ndXRogTZJCCDByY/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V
>
> - bestimme für drei verschiedene Windungszahlen ($N=800,\, 1600,\, 2400$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die @color(gesamte,red) Spule aufgewickelt)
>
>     - die Stromstärke $I$ 
>
>     - die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule vorsichtig nach dem Ort mit der maximalen Flussdichte, red)
>
> - notiere alle Messwerte in einer Tabelle

__2.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| # | $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
|:--:|:--:|:--:|:--:|:--:|
| 1 | 800 | <input type="number" default="0" id="l" min="0" max="10" size="5"> | <input type="number" default="0" id="I" min="0" max="10" size="5"> | <input type="number" default="0" id="B" min="0" max="10" size="5"> |
| 2 | 1600 |  |  |
| 3 | 2400 |  |  |

{{1}}
***************
__2.4 Gemeinsame Auswertung:__

>__Lsg.:__
>
> $\hspace{0.2cm}$ $\mu_0 =$ {2}{$\frac{B \cdot ℓ}{I \cdot N}$}
{{3}}
***********
> $\hspace{0.2cm}$ __Für Messung #1:__
>
> $\hspace{0.2cm}$ $\mu_0 = $ <script input="button">
    let N = 800;
    let I = document.getElementById("I").value;
    let l = document.getElementById("l").value;
    let B = document.getElementById("B").value;
    let mu = (B*l)/(I*N) 
    if ((isNaN(mu))||(mu==0)) "..."
    else mu.toExponential(2)
 </script> $\frac{V\cdot s}{A \cdot m}$

<details style="margin-left:0.2cm">

<summary> Tabellenwert </summary>

> $\mu_0 = 1,26\cdot 10^{-6} \frac{V\cdot s}{A \cdot m}$

</details>
***********



***************

__2.4 Auswertung:__

> - ermittle aus den Messungen #1-3 und der Formel aus 2.1 jeweils die magnetische Feldkonstante $\mu_0$ und notiere deine Ergebnisse
>
> - ermittle aus den Werten für $\mu_0$ den Mittelwert, notiere dein Endergebnis und vergleiche ihn mit dem theoretischen Wert aus 2.1 (in einem Satz)

__wenn noch min. 15 min Zeit ist:__

> - schau dir Experiment Teil 3 an, du kannst direkt mit der Durchführung (unterhalb der Abnahme) beginnen und die Werte notieren

### Experiment Teil 3: Überprüfung der Proportionalität $B$ ~ $N$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__3.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - notiere die Bedeutung der Formelzeichen
>
> - aufgrund der Formel kann man erkennen, dass die Flussdichte $B$ im Inneren der Spule proportional zur Anzahl der Windungen $N$ sein sollte
>
> - um die Proportionalität von $B$ ~ $N$ zu überprüfen, muss die magnetische Flussdichte $B$ für verschiedene Windungszahlen $N$ bestimmt werden. Dabei muss die Stromstärke $I$ konstant gehalten werden. In einem $B(N)$-Diagramm sollte sich näherungsweise eine Ursprungsgerade ergeben.

__3.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BpN](https://diversewolken.ddns.net/nextcloud/index.php/s/e5eGt4GAqkdK7ws/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V zunächst
>
> - bestimme für drei verschiedene Windungszahlen ($N=2400,\, 1600,\, 800$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die halbe Spule aufgewickelt)
>
>     - bestimme die Stromstärke $I$ für die erste Messung mit $N=2400$
>
>     - bestimme die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule nach dem Ort mit der maximalen Flussdichte, red)
>
>     - verändere bei deiner zweiten Messung mit $N=1600$ die Spannung soweit, dass die Stromstärke $I$ mit der ersten Messung identisch ist
>
>     - wiederhole die Messung für $N=800$
>
> - notiere alle Messwerte in einer Tabelle

__3.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
| :---: | :---: | :---: | :---: |
| 2400  | 0 | 0 | 0 |
| 1600  | 0 | 0 | 0 |
| 800   | 0 | 0 | 0 |

__3.4 Auswertung:__

> - erstelle aus den Messwerten ein Diagramm in dem du die Windungszahl $N$ auf der x-Achse und die magnetische Flussdichte auf der y-Achse einträgst
>
> - markiere in deinem Diagramm die drei Messpunkte #1-3, sowie den Punkt (0|0)
>
> - verbinde die Messpunkte mit einer Ausgleichsgeraden
>
> - überprüfe ob diese Ausgleichsgerade die Messergebnisse in guter Näherung darstellt, notiere einen Ergebnissatz

## 1.5 Materie im magnetischen und elektrischen Feld

<p class="newspaper">

__Magnetisches Feld__

<p class="cb">

__Elektrisches Feld__

</p>

</p>

---

Wird ein __Stoff (d.h. Materie)__ in ein magnetisches oder elektrisches Feld eingefügt, so verändert der Stoff die Stärke des Feldes, beschrieben durch 

<p class="newspaper">

die @color(magnetische Permeabilität $\mu_r$, orange) (-> FS. S 54).

<p class="cb">

die @color(Dielektrizitätszahl $\varepsilon_r$, orange) (-> FS. S 54).

</p>

</p>

---

__Beispiele:__

<p class="newspaper">

Cobalt: $\mu_r \approx 80-200$

Eisen: $\mu_r \approx 250-680$

Nickel: $\mu_r \approx 280-2500$

<p class="cb">

Glas: $\varepsilon_r \approx 5-16$

Bariumtitanat: $\varepsilon_r \approx 100-1000$

Wasser: $\varepsilon_r \approx 81$

</p>

</p>

---

__In beiden Beispielen__ richten sich elementare Strukturen des Material im umliegenden Feld aus.

<p class="newspaper">

@color(Elementar,red)@color(magnete,green) richten sich aus (__Magnetisierung__)

![ElementarMagnete](https://diversewolken.ddns.net/nextcloud/index.php/s/7H9rDQfp9fsAixS/download)

<p class="cb">

@color(Elementare,red) @color(Dipole, green) richten sich aus (__Polarisierung__)

![ElementareDipole](https://diversewolken.ddns.net/nextcloud/index.php/s/XfwLBXEkJSMJPTL/download)

</p>

</p>

---

__Unterschied:__

Während ferromagnetische Stoffe (Eisen, Cobalt, Nickel) das magnetische Feld __verstärken__, wird das elektrische Feld durch ein Dielektrikum (z.B. Glas, Wasser) __geschwächt/gedämpft__.

### Aufgabe zum magnetischen Feld

1. Eine Spule ist 9cm lang, hat 1500 Windungen und wird von einem Strom der Stärke 1,52 A durchflossen. Im Innern der Spule wird die magnetische Flussdichte 2,54 T gemessen.<br> Weise rechnerisch nach, dass sich im Innern der Spule nicht ausschließlich Luft befindet.

<details style="margin-left:10%">

<summary> Hilfe: Hinweis Zur Lösung</summary>

Ermitteln Sie die magnetische Flussdichte im Inneren der Spule unter der Annahme, dass diese mit Luft gefüllt ist. Vergleichen Sie Ihr Ergebnis mit der Angabe aus der Aufgabe und schlussfolgern Sie auf das vorhandene $\mu_r$.

</details>

<details style="margin-left:10%">

<summary> Rechenweg </summary>

![Abi21_Lsg2.1_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/4dsX4QKj4FgWz6q/download)

</details>

<details style="margin-left:10%">

<summary> Begründung </summary>

![Abi21_Lsg2.1_Begründung](https://diversewolken.ddns.net/nextcloud/index.php/s/som5GarSYN8yHPR/download)

</details>

<details style="margin-left:10%">

<summary> Alternativer Lösungsweg </summary>

Stelle die Formel für $B$ nach $\mu_r$ um, nutze für für B=2,54T und zeige, dass $\mu_r > 1$ gilt.

Hier ist: $\mu_r \approx 85$ 

</details>


---

2. Eine andere Spule hat 50 Windungen, ist 20 cm lang und ist ausschließlich mit Luft gefüllt. Die Flussdichte im Inneren der Spule beträgt 0,63 mT. Gib die Stromstärke an. <br> Die Spule wird nun auf 40 cm gedehnt, dabei ändert sich die Flussdichte im Inneren der Spule, Stromstärke und Windungszahl bleiben konstant.<br> Zeiche den Graphen $B = B(ℓ)$ für das Intervall 20cm bis 40cm.

@rangeQuiz2($\hspace{1cm}$ $I$, 2, $A$)

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zur Stromstärke</summary>

Nutzen Sie die Formel zur Berechnung der magnetischen Flussdichte und ermitteln Sie den fehlenden Wert der elektrischen Stromstärke.

</details>

<details style="margin-left:10%">

<summary> Rechenweg Stromstärke </summary>

![Abi21_Lsg2.2_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/Xd5nS692Wwd97cD/download)

</details>

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zum Graph</summary>

Nutze Sie die Formel für die magnetische Flussdichte, ermittlen Sie die Funktion $B(ℓ)$, setzen Sie die gegebenen Werten ein und erstellen Sie eine Datentabelle | $ℓ$ | $B(ℓ)$ | für den Bereich 20cm bis 40 cm.

</details>

<details style="margin-left:10%">

<summary> Berechnungen für den Graph $B(ℓ)$ </summary>

![Abi21_Lsg2.2_Berechnung_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/mddY9WFHAT59ofx/download)

</details>

<details style="margin-left:10%">

<summary> Datentabelle und Graph $B(ℓ)$ </summary>

<p class="newspaper">

<!-- data-type="none" -->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |

<p class="cb">

<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="ℓ in m"
     data-ylabel="B in mT"
-->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |


</p>

</p>

</details>

# LB IV - Geladene Teilchen in statischen Feldern

![ProtonCollisionCern](https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg)

## 1.1. Geladene Teilchen in statischen Magnetfeldern

_Tafelbildvideo zur Lorentzkraft:_

!?[TB_Video_Lorentzkraft](https://youtu.be/f0BNQ6uSvIQ)

<br>

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Lorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/tE56E3MWpqtozxx/download)

</details>

## 1.2. Hand-Regel zur Richtungsbestimmung der Lorentzkraft

_Bitte anschauen und ausprobieren_

!?[HandRegel](https://www.youtube.com/watch?v=snM3g4zWeNw)

__Bemerkungen zur Lorentzkraft:__

_Bitte Lückentext und weiteres probieren_

@color(siehe LB. S. 110, blue)

??[Lorentzkraft_LearningApps](https://learningapps.org/4454537)

__Tafelbild:__

![TB_KräfteAufBewegteElektrischeLadungen](https://diversewolken.ddns.net/nextcloud/index.php/s/aBZZK9rneamRSyf/download)


### Übungsaufgaben zur Lorentzkraft

1. Bitte schau dir zunächst dieses kleine Quiz zur Richtungsbestimmung der Lorentz-Kraft an.

      [QuizZurLorentzkraftRichtung](https://www.leifiphysik.de/elektrizitaetslehre/bewegte-ladungen-feldern/aufgabe/quiz-zu-bewegten-ladungen-im-magnetfeld)

      _Hinweis: Die magnetischen Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, green)._

---

2. Berechne für das Beispiel im Tafelbild die Lorentzkraft, wenn die Geschwindigkeit des Elektrons $v_e = 1\cdot 10^5 \frac{m}{s}$ und die magnetische Flussdichte $B = 0,2 mT$ beträgt.

<p style="margin-left:10%">

__Endergebnis:__

@rangeQuiz2($F_L$, 3.204e-18 , $N$)

__Zwischenwert:__

@rangeQuiz2($q_e$, 1.602e-19 , $C$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Ermittle mit der Formelsammlung die Ladung eines Elektrons $q_e$. Setze diese Werte in die Formel für die Lorentzkraft ein.

</details>

<details>

<summary> __Lösung__ </summary>

Die Bedingung Geschwindigkeit steht senkrecht auf Feldlinien ist gegeben.

$$F_L = q_e \cdot v_e \cdot B$$

$$ F_L = 1,602\cdot10^{-19}C \cdot 1\cdot 10^5 \frac{m}{s} \cdot 0,2 \cdot 10^{-3} T $$

$$ \underline{F_L = 3,204\cdot 10^{-18} N}$$

</details>


</p>

---

3. Die Lorentzkraft wirkt in jedem Moment senkrecht zur Flugbahn des Elektrons. Nenne die Form der Flugbahn auf der sich das Elektron bewegt, wenn eine Kraft immer senkrecht zur Bewegungsrichtung wirkt.

<p style="margin-left:10%">

- [( )] geradlinig
- [( )] parabelförmig
- [(x)] kreisförmig
- [( )] eckig

</p>

---

4. Die Flugbahn eines Elektrons in einem statischen magnetischen Feld ist eine Kreisbahn. Die Lorentzkraft $F_L$ wirkt als Zentritedalkraft $F_Z$ (siehe LB I, Kreisbewegung). Ermittle den Radius der Kreisbahn für die Aufgabe 2.

<p style="margin-left:10%">

@rangeQuiz2($r$, 0.00284 ,$m$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Um die Kreisbahn zu berechnen muss man (wie in der Aufgabe beschrieben) die Formel für die Zentripetalkraft $F_Z$ gleich der Formel für die Lorentzkraft $F_L$ setzen. $F_Z$ wurde in __LB I -> Kreisbewegung__ notiert.

<details style="margin-left:10%">

<summary> __Hinweis zur Formel__ </summary>

$F_Z = F_L$

$\hspace{2cm}$ mit $\boxed{F_Z = \dfrac{m\cdot v^2}{r}}$ und $\boxed{F_L = q \cdot v \cdot B}$

$ \dfrac{m\cdot v^2}{r} = q \cdot v \cdot B$

$\hspace{2cm}$ Nun noch nach $r$ umstellen und ausrechnen.

</details>

</details>

<details>

<summary> __Lösung__ </summary>

Aus dem Ansatz: 
$$F_Z = F_L$$

wobei die Zentripetalkraft $F_Z$ gleich 

$$F_Z = \dfrac{m\cdot v^2}{r}$$ 

und die Lorentzkraft $F_L$ gleich

$$F_L = q \cdot v \cdot B$$

ergibt sich für $r$

$$ r = \dfrac{m\cdot v}{q\cdot B}$$

mit den Werten:

$$ m_e = 9,11\cdot10^{-31} kg$$

$$ q_e = 1,602\cdot10^{-19} C$$

$$ v_e = 1 \cdot 10^5 \frac{m}{s}$$

$$ B = 0,2 mT = 0,2 \cdot 10^{-3} T$$

$$\boxed{\underline{\Rightarrow r = 2,84\cdot10^{-3} m}}$$

</details>

</p>

### Demonstrationsexperiment: Kräfte auf bewegte elektrische Ladungen in Magnetfeldern

@color(siehe LB. S. 110, blue)

![FotoLorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/mLFceeEL2jP7BDC/download)


## 1.3. Flugbahn von Elektronen in einem statischen, homogenen Magnetfeld

@color(siehe LB. S. 110, blue)

![TB_Flugbahn_Elektron_Magnetfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/gmPT93dWaFALw3f/download "Herleitung des Flugbahnradius")



### Aufgaben zur Vorbereitung der LK

#### 1. Vermischte Aufgaben

1. 1. Welche Eigenschaften muss ein Elektromagnet haben, der ein möglichst starkes Magnetfeld erzeugt?

<p style="margin-left:10%">

<details>

<summary> Hinweis </summary>

Untersuchen Sie den Einfluss der physikalischen Größen zur Berechnung der magnetischen Flussdichte $B$ in einer schlanken Spule.

</details>

<details>

<summary> Lösung </summary>

- Große Windungszahl $N$
- Kurze Baulänge $ℓ$
- Eisenkern
- Große Stromstärke $I$ (dicker Draht)

</details>

</p>

1. 2. In einer Spule (relative Dielektrizitätszahl = 1) mit 800 Windungen, einer Länge von 5 cm und einem Widerstand von 45 Ohm soll ein magnetisches Feld mit einer magnetischen Flussdichte von 12mT erzeugt werden. <br> a) Berechne die Spannung, die an die Spule angelegt werden muss. <br> b) Geben Sie zwei Möglichkeiten an, mit der man die magnetische Flussdichter verdoppeln kann.

<p style="margin-left:10%">

@rangeQuiz2($U$,26.786,$V$)

<details>

<summary> Zwischenergebnis </summary>

@rangeQuiz2($I$,0.595, $A$)

</details>

<details>

<summary> Hinweis a) </summary>

Ermittlen Sie zunächst die elektrische Stromstärke $I$, die fließen muss, damit das geforderte Magnetfeld erzeugt werden kann. <br> Nutzen Sie im Anschluss den Zusammenhang von Spannung $U$, Stromstärke $I$ und Widerstand $R$ um die Spannung zu ermittlen.

</details>

<details>

<summary> Lösung a) </summary>

<p class="newspaper">

geg.: 

<p style="margin-left:10%">

$B = 12 mT = 12 \cdot 10^{-3} T$

$N = 800$

$\mu_r = 1$

$R = 45 \Omega$

$ℓ=5cm = 5\cdot10^{-2}m$

</p>

ges.: $I$, $U$

<p class="cb">

Lsg.:

$B = \mu_0 \cdot \mu_r \cdot \frac{N\cdot I}{ℓ}$

$I = \dfrac{B \cdot ℓ}{\mu_0\cdot \mu_r \cdot N}$

$I=0,595 A$

$R=\frac{U}{I}$

$U=26,8V$

</p>

</p>

</details>

<details>

<summary> Lösung b) </summary>

Aus der Gleichung der magnetischen Flussdichte für eine lange Spule kann man entnehmen:

1. Die Stromstärke kann verdoppelt werden (entspricht einer Spannungsverdopplung, da I ~ U)

2. Die Windungszahl kann verdoppelt werden.

3. Die Länge der Spule kann halbiert werden.

4. In die Spule kann ein Stoff mit µ = 2 eingeführt werden. 

Bei jeder der 4 Möglichkeiten bleiben die anderen Größen konstant.

</details>

</p>

1. 3. LB S. 126 / 37 a)

<details style="margin-left:10%">

<summary> Lösung </summary>

Treten die Elektronen senkrecht zu den Feldlinien des homogenen Magnetfelds ein (Bild 1 und 2), so bewegen sie sich auf einer Kreisbahn. -> Kreisbewegung

Werden die Ladungsträger parallel zum Magnetfeld eingeschossen (Bild 3), dann ist die auf die Elektronen wirkende Lorentzkraft und somit die Ablenkung null. Die Bahnform ist eine Gerade. -> gleichförmige Bewegung

Treten die Elektronen schräg in das Magnetfeld ein (Bild 4), so bewegen sie sich auf einer spiralförmigen Bahn. Es liegt eine ungestörte Überlagerung einer gleichförmigen geradlinigen Bewegung und einer gleichförmigen Kreisbewegung vor.
</details>

#### 2. Aus Abi GK-2013

2. ![Kreisbahn](https://diversewolken.ddns.net/nextcloud/index.php/s/yZwLi4z7RWqTDkG/download) Geladene Teilchen bewegen sich im zeitlich konstanten homogenen Magnetfeld senkrecht zu den Feldlinien auf einer Kreisbahn. 

2. 1. Entscheiden Sie, ob es sich um ein positiv oder negativ geladenes Ion handelt. (1BE)

<p style="margin-left:10%">

[[negativ]]

</p>

2. 2. Übernehmen Sie diese Abbildung und tragen Sie am Punkt P der Bahn die Vektoren der Bahngeschwindigkeit und der wirkenden Lorentzkraft an. Begründen Sie, dass sich der Betrag der Bahngeschwindigkeit durch diese Kraft nicht ändert. (3BE)

<p style="margin-left:10%">

<details>

<summary> Hinweis </summary>

Überprüfe die Handregel und die Richtung der Lorentzkraft mit Hilfe von __1.2.__

</details>

<details>

<summary> Lösung Zeichnung </summary>

![Abi13_2_Lsg](https://diversewolken.ddns.net/nextcloud/index.php/s/SbMnFEaMHdqcEPn/download)

</details>

<details>

<summary> Lösung Begründung </summary>

Die Lorentzkraft @color($F_L$,purple) wirkt immer senkrecht zur Bewegungsrichtung. Eine Kraft, die auf einen Körper senkrecht zur Bewegungsrichtung wirkt, ändert nur die Richtung der Geschwindigkeit, nicht aber der Betrag (d.h. den Wert). Der Körper bewegt sich auf einer Kreisbahn.

</details>

</p>

2. 3. Ein einfach geladenes Ion der Masse $4,98\cdot 10^{−27} kg$ bewegt sich in einem Magnetfeld der Flussdichte $0,045 T$ auf einer Bahn mit dem Radius $0,15 m$. Berechnen Sie dessen Bahngeschwindigkeit. (3 BE)

<p style="margin-left:10%">

@rangeQuiz2($v$, 216867.5, $\frac{m}{s}$)

<details>

<summary> Hinweis 1 </summary>

Eine Information zur Ladung des Ions steckt im Text.

</details>

<details>

<summary> Hinweis 2 </summary>

Das Ion ist einfach geladen.

</details>

<details>

<summary> Hinweis 3 </summary>

Die Ladung des Ions beträgt eine Elementarladung.

</details>

<details>

<summary> Hinweis 4 </summary>

Nutzen Sie die hergeleitete Formel zur Berechnung des Bahnradius.

</details>

<details>

<summary> Lösung </summary>

<p class="newspaper">

geg.: 

<p style="margin-left:10%">

$B = 0,045 T$

$m = 4,98 \cdot 10^{-27} kg$

$r = 0,15 m$

$q = 1e = 1,6\cdot10{-19} C$

</p>

ges.: $v$

<p class="cb">

Lsg.:

<p style="margin-left:10%">

$r = \dfrac{v}{B\cdot \frac{q}{m}} \hspace{0.5cm}\Big | \cdot \Big(B\cdot \frac{q}{m}\Big)$

$v = \dfrac{r \cdot B \cdot q}{m}$

$v = 216867,5 \frac{m}{s} \approx 2,17\cdot 10^5 \frac{m}{s}$

</p>

</p>

</p>


</details>

</p>

## Checkliste LK 03.03.25

__Zugelassene Hilfsmittel:__ Formelsammlung, CAS

- Grundlagen zum elektrischen Feld (Kraftwirkung auf ein geladenes Teilchen $E=F/q$, elektrisches Feld im Plattenkondensator _Art und Berechnung_)

- allgemeine Definition, Beschreibung, Eigenschaften magnetisches Feld

- Arten magnetischer Felder, Arten von Magneten, Feldlinien

- Kraftwirkung zwischen Magneten

- Eigenschaften Erdmagnetfeld (Zahlenwerte müssen nicht auswendig gelernt werdne)

- Definition und Berechnung der magnetischen Flussdichte $\vec{B}$

- Berechnung der magnetischen Flussdichte innerhalb eine langen Spule

- magnetische Flussdichte mit dem Cassy-Messgerät bestimmen (Handhabung des Messgerätes, Idee des Experiments Bestimmung der magnetischen Feldkonstante $\mu_0$ verstehen)

     __nicht notwendig:__ technische Details (Verbindung Cassy-Tablet, Aufbau eines Experiments)

- Materie im magnetischen Feld (Begriff Ferromagnetikum), elementare Wirkung eines äußeren Magnetfeldes auf einen ferromagnetischen Stoff (-> Elementarmagnete)

- Unterschiede und Gemeinsamkeiten zu einem Stoff im elektrischen/magnetischen Feld

- Kräfte auf bewegte geladene Teilchen in einem Magnetfeld -> Lorentzkraft

- Kraft auf einen Stromdurchflossenen Leiter in einem Magnetfeld -> __Handregel zur Richtungsbestimmung__ 

- Flugbahn geladener Teilchen in einem homogenen, statischen Magnetfeld 

     _Hinweis: Herleitung des Flugbahnradius muss nicht auswendig gewusst werden, nur der Ansatz sollte verstanden sein_

---

### Zur Erinnerung: Experimentvideo aus der letzten Stunde (bis 3:24 min)

!?[Fadenstrahlrohr](https://youtu.be/j5y64SPRnH0?si=MxXy0qlxifHUnRlz)

##  2. Geladene Teilchen im elektrischen Feld

![Elektrisches Feld](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/VFPt_charged_parallel_plates.svg/640px-VFPt_charged_parallel_plates.svg.png)

## 2.1. Der Millikan-Versuch

_Tafelbildvideo zum Millikan-Versuch:_

!?[Millikan-Experiment](https://www.youtube.com/watch?v=XMfYHag7Liw)

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Millikan](https://diversewolken.ddns.net/nextcloud/index.php/s/ocNCHdfqgfNNt44/download)

</details>

---

__Erklärung:__

Robert Millikan führte einen berühmten Versuch durch, um die Elementarladung $q_e$ zu bestimmen. Dabei wurden geladene Öltröpfchen in einem homogenen elektrischen Feld zwischen zwei Platten zum Schweben gebracht, indem sich die elektrische Kraft und die Gewichtskraft gegenseitig kompensieren. 

---

<p style="color:blue">

__1. Gleichung für Ladung ableiten:__ 

 - notieren Sie das genannte Kräftegleichgewicht als Gleichung

 - setzen Sie für beide Kräfte die gegebenen Formeln ein, notieren Sie für die elektrische Feldstärke die Formel im Plattenkondensator

 - stellen Sie die Gleichung nach der Ladung $q$ um

 - notieren Sie die Gleichung in Ihrem Hefter
</p>

---

<details>

<summary> __Lösung: Formel zur Bestimmung Ladung q des Öltröpfchens:__ </summary>

$$\boxed{q = m \cdot g \cdot \frac{d}{U}}$$

<p style="margin-left:10%">

$q$ ... Ladung des Öltröpfchens

$m$ ... Masse des Öltröpfchens

$U$ ... angelegte Spannung

$d$ ... Plattenabstand

</p>

</details>

---

<p style="color:blue">

__2. Berechnung der Ladung (+)__

Die Elementarladung wurde von Millikan bestimmt. Berechnen Sie die Ladung eines Öltröpfchens im Gleichgewicht, wenn die Masse $m = 2.5 \cdot 10^{-15} kg$ beträgt, Plattenabstand $d = 6 mm$ und die angelegte Spannung $U = 900 V$.

@rangeQuiz2($q$, 1.635e-19, $C$)

</p>

---

<p style="color:blue">

__3. Präzisierung des Experiments I (++)__

__Hintergrund:__ Tatsächlich konnte Milikan die Masse der Öltröpfchen nicht messen, da sie viel zu klein waren. Anstelle dessen versuchte er, den Durchmesser der Tröpfchen zu bestimmen und so mittels Kugelvolumen und der Dichte von Öl, die Masse der Öltröpfchen zu bestimmen. 

__Aufgabenstellung:__ Ermittln Sie für ein Tröpfchen, dass einen Durchmesser von 1,2µm besitzt und bei einer Spannung von 165 V (d=6mm) schwebt, die elektrische Ladung. Als Dichte kann $\rho_{Öl}=0,875 \frac{g}{cm^3}$ angenommen werden.

@rangeQuiz2($q$, 3.2e-19, $C$)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweise:__ </summary>

- ermitteln Sie aus der Formelsammlung die Formel für das Volumen einer Kugel 

- nutzen Sie den Durchmesser des Tröpfchens um dessen Volumen zu bestimmen 

- ermitteln Sie mit Hilfe von Volumen und Dichte die Masse des Tröpfchens

- berechnen Sie mit Hilfe von Masse, Spannung und Plattenabstand die Ladung

</details>

<details style="margin-left:10%">

<summary> __Lösungen:__ </summary>

$V=\frac{4}{3}\pi r^3$ 

@rangeQuiz2($V$, 9.05e-19 , $m^3$) 

@rangeQuiz2($m$,  7.972e-16 , $kg$)

Hinweis: $\rho_{Öl} = 0,875 \frac{g}{cm^3} = 875 \frac{kg}{m^3}$

@rangeQuiz2($q$, 3.2e-19, $C$)

</details>

---

<p style="color:blue">

__3. Simualtion des Experiments II (++)__

__Hintergrund:__ Wie man in der vorhigen Analyse sehen konnte, war es bei dem Versuch nicht sicher, dass das Öltröpfchen mit genau einer Elementarladung geladen war. Tatsächlich variierte die Anzahl an Elementarladungen von Tröpfchen zu Tröpfchen. Millikan konnte bei seiner Analyse allerdings zeigen, dass die Ladung der Tröpfchen keine beliebigen Werte annehmen konnte. 

__Aufgabenstellung:__ Nutzen Sie die Simulation auf LEIFI-Physik ([SIMULATION_MILIKAN](https://www.leifiphysik.de/elektrizitaetslehre/ladungen-elektrisches-feld/versuche/millikan-versuch-schwebemethode-simulation)). Bringen Sie mindestens fünf Tröpfchen nacheinander in einen Schwebezustand, notieren Sie Spannung und Tröpfchenradius und ermitteln Sie die zugehörigen Ladungen. Tragen Sie anschließend die Datenpunkte in ein Diagramm ein. 

![MILIKAN_FOTO](https://diversewolken.ddns.net/nextcloud/index.php/s/RgskbsAYNLX2ibX/download)<!-- style="max-width=500px" -->

</p>

<details>

<summary> Ergebnis des Versuchs </summary>

> Die kleinste mögliche Ladung, die für das Experiment ermittelt werden konnte betrug $1,6\cdot10^{-19}C$. Alle höheren Ladungen sind immer Vielfache dieser @color(Elementarladung $e$, red)
>
> $$ \boxed{e = 1,602\cdot10^{-19}C}$$

</details>


### KI-Aufgabe: Erkläre den Milikan-Versuch

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Prompt Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Milikan-Aufgabe:__<br> Erkläre den Milikanversuch. Gehe dazu auf folgende drei Punkte ein. <br> 1. Erkläre den Aufbau des Versuchs. Erkläre auch, wie die Messungen durchgeführt wurden. <br> 2. Beschreibe die Messungen und die Ergebnisse des Milikan-Versuchs ohne zu interpretieren oder zu schlussfolgern. <br> 3. Nenne die Schlussfolgerungen, die man aus den Ergebnissen des Milikan-Versuchs ziehen kann.

<p style="margin-left:10%">

__Prompt__

<span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre den Milikanversuch. Gehe dazu auf folgende drei Punkte ein. <br> 1. Erkläre den Aufbau des Versuchs. Erkläre auch, wie die Messungen durchgeführt wurden. <br> 2. Beschreibe die Messungen und die Ergebnisse des Milikan-Versuchs ohne zu interpretieren oder zu schlussfolgern. <br> 3. Nenne die Schlussfolgerungen, die man aus den Ergebnissen des Milikan-Versuchs ziehen kann. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>

</p>

<script input="submit" style="margin-left:10%"  default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>



---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

für eigene Geräte:

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)

## 2.2. Bewegung geladener Teilchen im elektrischen Feld

<p class="newspaper">

__Elektronenkanone__

![Elektronenkanone](https://diversewolken.ddns.net/nextcloud/index.php/s/cC5JWAYmimFKmrC/download)

_35 min_

<p class="cb">

__Ablenkröhre__

![Ablenkröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/HaNg8rpJnyZj7F5/download)

_35 min_

</p>

</p>

### 2.2.1 Beschleunigung im Längsfeld - Elektronenkanone

@timer(35,00)

__Aufbau einer Elektronenkanone__

??[VirtuelleExperiment_Elektronenkanone_Aufbau](https://virtuelle-experimente.de/kanone/klassisch/aufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de CC BY-NC-SA 3.0 DE")

<p style="color:blue">

__Aufgaben:__

1. Wähle im linken Menü _Simulation_

1. 1. Verändere die Heizspannung $U_{Heiz}$ und beobachte den Effekt auf das Experiment.

1. 2. Verändere die Beschleunigungsspannung $U_b$ und beobachte den Effekt auf das Experiment.

2. Klicke auf _weiter_ oder im linken Menü auf _Beschleunigung_.

2. 1. Die Elektronenkanone ist in eine @color(Beschleunigungszone, green) und eine @color(Flugzone, pink) aufgeteilt.

2. 2. Zeichne unter der Überschrift (siehe oben) eine Skizze der Elektronenkanone in deinen Hefter. 

2. 3. Schau dir die Herleitung der Beschleunigungsarbeit ($W_{el}$) bzw. der Geschwindigkeit der Elektronen nach der Beschleunigung an. Übernimm grundlegende Elemente der Herleitung für $v_{end}$ und die finale Formel in deinen Hefter.

2. 3. Klicke nun auf _weiter_ oder _Flugphase_. Lies dir die Anweiungen durch. Es genügt, wenn du im Hefter folgende Bemerkung unter die Herleitung notierst.

<p style="color:black">
> Wenn die Elektronen die Anode verlassen haben, bewegen Sie sich in Flugrichtung (x-Richtung) geradlinig-gleichförmig mit der Geschwindigkeit $v_{end}.$
</p>

3. Klicke nun im oberen Menü auf den Punkt _Übungen_.

3. 1. Löse _Übung Aufbau_ (Menü links)

3. 2. Löse den Lückentext.

3. 3. Löse das Quiz.

3. 4. Bearbeite die Rechenaufgaben. 

      __Aufgabe 1:__ Als __Partnerübung__, d.h. eine Person stellt die Frage und liest die Lösung, die andere Person beantwortet die Frage.

      __Aufgabe 2:__ Als __Einzelarbeit__ mit Lösungsüberprüfung und Diskussion des Lösungswegs in der Gruppe.

</p>


#### KI-Aufgabe: Beschleunigung elektrischer Ladungen im Längsfeld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem Elektronen beschleunigt werden können. <br> 2. Nenne und begründe die Art der Bewegung der Elektronen. <br> 3. Gib an, wie die Intensität des Elektronenstrahls (d.h. die Anzahl an Elektronen pro Sekunde) beeinflusst werden kann. <br> 4. Gib an, wie die Endgeschwindigkeit der Elektronen beeinflusst werden kann.

<p style="margin-left:10%">

<summary> __Prompt__ </summary>

<span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem Elektronen beschleunigt werden können. <br> 2. Nenne und begründe die Art der Bewegung der Elektronen. <br> 3. Gib an, wie die Intensität des Elektronenstrahls (d.h. die Anzahl an Elektronen pro Sekunde) beeinflusst werden kann. <br> 4. Gib an, wie die Endgeschwindigkeit der Elektronen beeinflusst werden kann. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Grundkurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
    
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)


alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


### 2.2.2 Ablenkung Querfeld - Ablenkröhre

@timer(35, 00)

__Aufbau einer Elektronen-Ablenkröhre__

??[VirtuelleExperiment_ElektronenAblenkrhre](https://virtuelle-experimente.de/e-feld/hypothesen/versuchsaufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de, CC BY-NC-SA 3.0 DE")

<p style="color:blue">

__Aufgaben:__

1. Klicke auf Zusammenfassung (linkes Menü)

1. 1. Übernimm folgenden Merksatz in deinen Hefter

<p style="color:black">
> Bewegen sich Elektronen senkrecht zu den Feldlinien durch das homogene elektrische Feld eines Plattenkondensators, werden sie aufgrund der elektrischen Kraft abgelenkt.
</p>

1. 2. Übernimm eine Skizze des Aufbaus in deinen Hefter

1. 3. Übernimm die beiden Erkenntnisse in deinen Hefter

<p style="color:black">

> Je größer die Plattenspannung $U_P$ am Kondensator desto stärker ist die Ablenkung der Elektronen
>
> Je kleiner die Beschleunigungsspannung der Elektronen (und somit deren Geschwindigkeit), desto stärker ist die Ablenkung
>
> Die Bahnform der Elektronen ist eine __Parabel__ mit der Gleichung
>
> $$\boxed{y(x) = \dfrac{U_p}{4 \cdot d \cdot U_b} \cdot x^2}$$

2. Wechsle zu den _Übungen_ (oberes Menü) und bearbeite:

2. 1. Übung Fachbegriffe

2. 2. _Optional:_ Übung Anschluss

2. 3. Mulitple Choice kurze Version

2. 4. Abituraufgaben

      - Aufgabe 2

      - Aufgabe 5 (a, b, d)

</p>

</p>


#### KI-Aufgabe: Beschleunigung elektrischer Ladungen im Querfeld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten die Bewegung eines geladenen Teilchens im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen (Querfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem eine solche Ablenkung erfolgen kann. <br> 2. Beschreibe die Art der Bewegung der elektrischen Ladungen. Gehe auf den Begriff Superposition ein. <br> 3. Gib qualitativ an, welcher Bahnform die geladenen Teilchen folgen. <br> 4. Gib an, wie die Stärke der Ablenkung der geladenen Teilchen beeinflusst werden kann.

<p style="margin-left:10%">

>__Prompt__
>
><span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen:<br> Erkläre mit eigenen Worten die Bewegung eines geladenen Teilchens im Einfluss eines homogenen elektrischen Feldes, wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen (Querfeld). Gehe dazu auf folgende Punkte ein: <br> 1. Beschreibe einen Aufbau, mit welchem eine solche Ablenkung erfolgen kann. <br> 2. Beschreibe die Art der Bewegung der elektrischen Ladungen. Gehe auf den Begriff Superposition ein. <br> 3. Gib qualitativ an, welcher Bahnform die geladenen Teilchen folgen. <br> 4. Gib an, wie die Stärke der Ablenkung der geladenen Teilchen beeinflusst werden kann. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Grundkurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>

</p>
    
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>


---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)


alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)



# LB V - Elektromagnetische Felder

!?[CG-Physics-Generator](https://www.youtube.com/watch?v=34z97ULvmpM)

## Motivation - Kraftwerke zur Energieversorgung

![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/Xbf7QmBSmwzN4GK/download)

## 1. Elektromagnetische Induktion

{{1}}
********
> __Induktion:__ Eine Spannung wird induziert, wenn sich der @color(magnetische Fluss $\Phi$,red) einer Leiterschleife oder Spule @color(ändert, red).
********

{{2}}
********
---

> __Definition:__ Der @color(magnetische Fluss $\Phi$, red) ist definiert als
>
> $$ \boxed{\red{\Phi = B \cdot A}} $$
>
> $\hspace{1cm}$ B .. magnetische Flussdichte
>
> $\hspace{1cm}$ A .. vom Magnetfeld durchsetzte Fläche
********

{{3}}
********
---

> __Induktionsspannung:__ Der Betrag der Induktionsspannung $U_{ind}$ ist definiert ergibt sich aus der Windungszahl der Spule $N$ multipliziert mit der @color(zeitlichen Änderung des magnetischen Flusses $\frac{\Delta\Phi}{\Delta t}$, red).
>
> $$ \boxed{U_{ind} = N \cdot \dfrac{\red{\Delta \Phi}}{\Delta t}} $$
********

{{4}}
********
---

__1. Schlussfolgerung:__ Je größer die Windungszahl $N$ der Spule, desto größer ist die induzierte Spannung $U_{ind}$.

---
********

<p class="newspaper">
{{5}}
********
> __Induktion durch Änderung der Fläche A__
>
> $$ \boxed{U_{ind} = N \cdot \red{B} \cdot \dfrac{\red{\Delta A}}{\Delta t}} $$
>
> __Beispiel:__ @color(Generator, blue)
********

<p class="cb">
{{6}}
********

> __Induktion durch Änderung der Flussdichte B__ 
>
> $$ \boxed{U_{ind} = N \cdot \red{A} \cdot \dfrac{\red{\Delta B}}{\Delta t}} $$
>
> __Beispiel:__ @color(Transformator, blue)
********
</p>

</p>

### 1.1. Aufgaben zum Generator


<p style="color:blue">

- [ ] Notiere das Tafelbild _1. Elektromagnetische Induktion_ in deinen Hefter

- [ ] Probiere die Aufgaben _Grundversuche Elektromagnetische Induktion_ und Fülle die Lückentexte

- [ ] Übernimm den Absatz _Aufbau eines Generators_ in deinen Hefter

- [ ] Diskutiere mit der KI im Abschnitt _Elektromagnetische Induktion_

- [ ] Nutze den Bausatz Generator und baue ein Generatormodell auf, schließe ein Cassy-Spannungsmessgerät an und miss die induzierte Spannung

- [ ] Beantworte die Fragen zum Generator 2

</p>


#### Grundversuche Elektromagnetische Induktion

@color(Nutze die drei Simulationen um die zugehörigen Lückentexte auszufüllen., blue)

[LEIFI-Lückentexte](https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-induktion/versuche/drei-grundversuche-zur-elektromagnetischen-induktion-simulationen)

#### Aufbau eines Generators

Ein einfacher __Generator__ besteht typischer Weise aus einem @color(Magneten, orange) und einer @color(Spule,orange), welche sich im Magnetfeld drehen kann.

<p class="newspaper">

__Skizze:__

![Generator_Skizze](https://asset.conrad.com/media10/isa/160267/c1/-/de/Generator/grundfunktion-eines-generators.jpg)

<p class="cb">

1. Fester Dauermagnet (kann auch Elektromagnet sein) -> @color(__STATOR__,red)

2. Magnetfeld des Dauermagneten (_nicht sichtbar_)

3. Drehbare Spule (hier nur Leiterschleife) -> @color(__ROTOR__,red)

4. Schleifringe

5. Schleifkontakte zur Spannungsabführung

_Hinweis: Magnet und Spule (d.h. **Rotor** und **Stator**) können auch vertauscht sein. Dann ist Magnet beweglich und die Spule fest._

</p>

</p>


#### KI: Elektromagnetische Induktion am Generator

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Aufgabe Induktion:__

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2">Ich werde dir jetzt 4 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10. Frage mich nach jeder Einschätzung von dir, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln.
    1. Definiere den Begriff magnetischer Fluss.
    2. Notiere, welche physikalischen Größen sich bezüglich des magnetischen Flusses ändern können, damit einer Induktionsspannung erzeugt wird.
    3. Nenne eine technische Anwendung, bei dem eine Änderung der durchsetzten Fläche eine Spule in einem Magnetfeld zu einer Induktionsspannung führt.
    4. Notiere Einflussfaktoren auf die Induktionsspannung in einem Generator.
    Alle Fragen sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.
</span>
</div>
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


#### Generator selber bauen

__Aufgabenstellung:__ Nutze in einer Gruppe von zwei Leuten den Bausatz und baue den Generator auf. Am Lehrertisch gibt es ein Demogerät. Experimentiere mit dem Generator anhand folgender Aufgaben

{{1}}
*******
__Der Generator:__

1. Schließe an den Generator das Cassy-Messgerät zur Spannungsmessung an. (nur @color(roten,red) und @color(schwarzen, black) Pol verwenden.)

2. Stelle das Cassy-Messgerät bei der Spannungseinstellung (__Messbereich__) auf -0,3 bis 0,3 V.

3. Drehe an der Welle und überprüfe die angezeigte Spannung. <br> {2}{@color(-> Das Voltmeter sollte ausschlagen.,orange)}

4. Überprüfe, ob du die maximale Spannung beeinflussen kannst.

5. Wähle das Diagramm (oben rechts) und dann die Stoppuhr (oben links) und lass dir den zeitlichen Spannungsverlauf anzeigen.

*******


#### Fragen zum Generator 2

<p class="newspaper">

3. Wahr oder falsch? Wenn sich der Generator schneller dreht, erhöht sich die elektrische Spannung.

     [(X)] wahr
     [( )] falsch

4. Wahr oder falsch? Wenn man die elektrische Spannung am Generator erhöhen will, kann man das Magnetfeld verstärken.

     [(X)] wahr
     [( )] falsch

5. Um die Spannung am Generator zu erhöhen, kann man

     [[ ]] Die Anzahl der Windungen der Spule verringern
     [[X]] Die Anzahl der Windungen der Spule vergrößern
     [[ ]] Die Querschnittsfläche der Spule verkleinern
     [[X]] Die Querschnittsfläche der Spule vergrößern

<p class="cb">

6. Wahr oder falsch? Bei einem Generator muss der Magnet fest sein (Stator) und die Spule drehend (Rotor).

     [( )] wahr
     [(X)] falsch
     
7. Welches Prinzip liegt der Stromerzeugung in einem Generator zugrunde?

     [( )] Thermische Leitung
     [(X)] Elektromagnetische Induktion
     [( )] Kernspaltung
     [( )] Schallwellen

8. Was erzeugt in einem Generator die Spannung?

     [( )]  Eine chemische Reaktion in der Spule
     [( )]  Die Erwärmung des Magneten
     [(X)] Die Bewegung einer Spule in einem Magnetfeld     
     [( )]  Die Anwesenheit eines elektrischen Leiters


</p>

</p>

### 1.2. Arbeitsaufträge zum Transformator

<p style="color:blue">

- [ ] Zeichne das Schema eines Transformators in deinen Hefter. Übernimm das Tafelbild komlett

- [ ] Bearbeite die Übungen zum Trafo

- [ ] Bearbeite die KI-Aufgaben zur Induktion

- [ ] Experimentiere mit dem Transformator


</p>

#### Wiederholungsvideo Transformator

!?[WasIStEinTransformator](https://diversewolken.ddns.net/nextcloud/index.php/s/Z6E3QPJyaTccksw/download)

#### Aufbau Transformator

<p class="newspaper">

![TB-Transformator](https://diversewolken.ddns.net/nextcloud/index.php/s/mGSfKNSR8C9s8XM/download)

<p>

__Formelzeichen:__

<p style="margin-left:10%">

$U_1$ oder $U_p$ .. Primärspannung

$U_2$ oder $U_s$ .. Sekundärspannung

$N_1$ oder $N_p$ .. Windungszahl auf Primärseite

$N_2$ oder $N_s$ .. Windungszahl auf Sekundärseite

</p>

__Funktionsprinzip:__

<p style="margin-left:10%">

Auf der Primärseite wird eine @color(__Wechselspannung__, darkblue) angelegt. Diese Wechselspannung erzeugt ein @color(__zeitlich veränderliches Magnetfeld__, orange), welches im wesentlichen im @color(__Eisenkern__, darkgray) verläuft. <br> Die @color(Sekundärspule,crimson) wird von dem Magnetfeld durchsetzt. In dieser Spule ändert sich der Magnetische Fluss $\Phi$ und somit wird eine Spannung induziert.

</p>

</p>

</p>

> Bei einem unbelasteten Transformator gilt:
>
> $$ \boxed{\dfrac{U_1}{U_2} = \dfrac{N_1}{N_2}} $$

#### Übung Funktionsweise Trafo

@color(_Bringe die Sätze von links nach rechts in die richtige Reihenfolge., blue)

<iframe src="https://learningapps.org/watch?v=pyuu71zx524" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

#### Einfache Rechnungen - Transformator

1. Betrachte folgende Transformator-Daten. Entscheide, ob der Transformator zum Hoch- und Heruntertransformieren verwendet wir. <br> _Für das Übersetzungsverhältnis $n$ gilt: $n = \frac{U_p}{U_s} = \frac{N_p}{N_s}$_.

<p style="margin-left:5%;margin-right:5%">

<p class="newspaper3">

$n=5$

<!-- data-solution-button="off" -->
- [[ ]] Hochtransformiern
- [[x]] Heruntertransformieren
- [[ ]] weder noch

<p class="cb">

$N_p=1000; N_s=50000$

<!-- data-solution-button="off" -->
- [[x]] Hochtransformieren
- [[ ]] Heruntertransformieren
- [[ ]] Weder noch

<p class="cb">

$N_p=100; N_s=100$

<!-- data-solution-button="off" -->
- [[ ]] Hochtransformieren
- [[ ]] Heruntertransformieren
- [[x]] Weder noch

</p>

</p>

</p>

</p>

2. ![TrafoHaus](https://upload.wikimedia.org/wikipedia/commons/1/19/Elfmorgenbruch_220kV-Transformator.jpg) In Transformatorstationen wird die Elektrizität des regionalen Verteilnetzes mit der Mittelspannung ca. 20 kV zur Versorgung der Niederspannungsendkunden auf die im Ortsnetz verwendeten 400-V-Leiter-Leiter-Spannung transformiert. Wähle die Transformator-Einstellungen aus, die hier verwendet werden können. <br> _Hinweise: 1kV = 1000 V_

<p style="margin-left:5%;margin-right:5%">

<p class="newspaper3">

<!-- data-solution-button="off" -->
- [[x]] $N_s < N_p$
- [[ ]] $N_s = N_p$
- [[ ]] $N_s > N_p$

<p class="cb">

<!-- data-solution-button="off" -->
- [[ ]] $n=0,1$
- [[ ]] $n=10$
- [[x]] $n=50$

<p class="cb">

<!-- data-solution-button="off" -->
- [[x]] $N_p=50000; N_s=1000$
- [[ ]] $N_p=20000; N_s=100$
- [[x]] $N_p=10000; N_s=200$

</p>

</p>

</p>

</p>

3. Für einen unbelasteten Transformator sind zeilenweise die folgenden Daten bekannt. Ergänze die fehlenden Werte. Für das Übersetzungsverhältnis $n$ gilt: $n = \frac{U_p}{U_s} = \frac{N_p}{N_s}$

<p style="margin-left:5%;margin-right:5%">

---

a)

<!-- data-solution-button="off" -->
| $N_p$ | $N_s$ | $U_p$ | $U_s$ | n |
| 2500 | 500  | 100V   | [[ 20 ]] V     | [[ 5 ]] |

---

b)

<!-- data-solution-button="off" -->
| $N_p$ | $N_s$ | $U_p$ | $U_s$ | n |
| 250 | [[ 1000 ]] | [[ 10 ]] V | 40V   | 0,25 |

</p>


#### KI-Aufgaben zur Induktion

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.
</p>

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessern, oder zur nächsten Frage springen.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2">Ich werde dir jetzt 5 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10. Frage mich nach jeder Einschätzung von dir, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln.
    1. Definiere den Begriff magnetischer Fluss.
    2. Notiere, welche physikalischen Größen sich bezüglich des magnetischen Flusses ändern können, damit einer Induktionsspannung erzeugt wird.
    3. Nenne eine technische Anwendung, bei dem eine Änderung der durchsetzten Fläche eine Spule in einem Magnetfeld zu einer Induktionsspannung führt.
    4. Nenne eine technische Anwendung, bei dem die Änderung der magnetischen Flussdichte eine Spannung hervorruft.
    5. Erkläre, wie bei einem Transformator die Induktion Anwendung findet.
    Alle Fragen sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.</span>
</div>

<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)



## Checkliste Klausur 11ph3 28.04.25

__Grundlagen magnetische Kraft/magnetisches Feld:__

- Lorentzkraft auf eine bewegte Ladung im homogenen Magnetfeld (Formel und Handregeln) [Übungsaufgabe-Lorentzkraft](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/GK.11_2024_2025/LB4_GeladeneTeilchen_StatischeFelder.md#4)

- Berechnung magnetische Flussdichte B einer langen Spule (Formel steht in der Formelsammlung, sollte verstanden sein) [Übungsaufgabe-Flussdichte](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/GK.11_2024_2025/LB3_MagnetischesFeld.md#8)

__Grundlagen elektrische Kraft/elektrischen Feld:__

- Berechnung der elektrischen Kraft auf eine Ladung im elektrischen Feld (Formeln stehen in der Formelsammlung) [Übung-ElektrischeKraft](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/GK.11_2024_2025/LB2_ElektrischesFeld.md#10)

    - Berechnung des elektrischen Feldes in einem Plattenkondensator (nur 6.1 bis 6.3: [Übungen-Plattenkondensator-6.1-6.3](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/GK.11_2024_2025/LB2_ElektrischesFeld.md#21)

__Bewegung elektrischer Ladungen im B-Feld oder E-Feld:__

- Bewegung einer Ladung im homogenen Magnetfeld (inkl. Bestimmung Kreisbahnradius) [Abituraufgabe](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/GK.11_2024_2025/LB4_GeladeneTeilchen_StatischeFelder.md#9)

- Beschleunigung einer elektrischen Ladung im elektrischen Feld (Längsfeld / Elektronenkanone) [Übung-Elektronenkanone-Aufgabe-2](https://virtuelle-experimente.de/kanone/uebungen/aufgaben.php)

- e/m-Versuch: [Wdh-Video-Zum-Versuch](https://youtu.be/A8mLTfc8W7c?si=nx-6LFE48FBjRmEn) (Kombination aus Elektronenkanone und homogenem Magnetfeld in Helmholtzspulen) (Aufgabe 2 a,b,c: [Abituraufgabe-2-abc](https://virtuelle-experimente.de/b-feld/uebungen/aufgaben.php) )

__Elektromagnetische Induktion:__

- Elektromagnetische Induktion und der magnetische Fluss $\Phi$ (Definition)

- Anwendung des Induktionsprinzips bei Generator

- Anwendung des Induktionsprinzips bei Transformator

- Abhängigkeit der Induktionsspannung von der Windungszahl

- IQB: Aufgabe 1-5: [IQB-Aufgabe zur Elektro-Magnetischen-Induktion](https://www.iqb.hu-berlin.de/appsrc/taskpool/data/taskpools/getTaskFile?id=p12^InduktiversensorgA^f21968)

!?[CG-Physics-Generator](https://www.youtube.com/watch?v=34z97ULvmpM)

#### Demonstrationsexperiment A Freier Fall im Rohr

> Stabmagnet fällt einerseits durch ein metallisches Rohr (Aluminium) und andererseits durch ein Kunststoffrohr.

{{1}}
*********
---

@color(Zeichnen Sie eine Skizze des Versuchs. Beschreiben Sie jeweils Ihre Beobachtungen., blue)

---

__Skizze:__
*********

{{2}}
*********
---

__Beobachtung:__

<p class="newspaper">

__Metallrohr__

<p class="cb">

__Kunststoffrohr__

</p>

</p>

---
*********

{{3}}
*********
__Vorläufige Erklärung:__

> - das metallische Rohr wirkt wie eine Spule mit einer Windung
>
> - durch die Bewegung der magnetischen Kugel ändert sich _lokal_ der magnetische Fluss in der Röhre, es wird eine @color(Spannung induziert, red)
>
> - durch die induzierte Spannung @color(fließt _kreisförmig_ ein Strom und erzeugt ein Magnetfeld,red)
>
> - das @color(induzierte Magnetfeld, red) wechselwirkt mit dem Magnetfeld der Kugel und @color(bremst die Kugel, blue)
*********

### 1.3. Lenz'sche Regel - Richtung der Induktionsspannung

> Die induzierte Spannung ist immer @color(so gerichtet, red), dass sie ihrer Ursache @color(entgegen, red) wirkt.

> $$ \boxed{U_{ind} = \red{\textbf{-}}\, N \cdot \dfrac{\Delta\Phi}{\Delta t} $$

__Beispiel:__ Fallende Kugel 

__Ursache für Induktion:__ Bewegung der Kugel im Rohr

__Anwendung der Lenz'schen Regel:__ Die induzierte Spanung (und daher das induzierte Magnetfeld) ist so gerichtet, dass es der Ursache (Bewegung) entgegen wirkt.

---

_Hinweise:_

- betrachten wir den @color(Betrag, red) (also den Wert) der induzierten Spannung, so genügt die Formel $N \cdot \dfrac{\Delta\Phi}{\Delta t}$

- betrachten wir die @color(Wirkung, red) der induzierten Spannung, so müssen wir die _Lenz'sche Regel_ beachten

#### Weitere Beispiele

@color(Beschreibe und erkläre die beiden Experimente in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen., blue)

#### B. Thomson'scher Ringversuch 

<p style="color:blue">
Aufgabe: Zeichne (Skizze), beschreibe (Beobachtung) und erkläre (Erklärung) das Experiment _Thomson'scher Ringversuch_ in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen.
</p>


__Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.__

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessernn.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Ich soll ein Experiment erst beschreiben und anschließend erklären. Bitte frage mich zunächst nach einer Beschreibung meiner Beobachtung. Unterstütze mich bei der Antwort, hilf mir nur, wenn ich darum bitte. Achte bei meiner Erklärung darauf, dass die Induktion einer Spannung richtig beschrieben wird und die Lenz'sche Regel korrekt erklärt wird. <br> Das Experiment ist der Thomson'sche Ringversuch. Man benutzt zwei Aluminiumringe: Der erste Ring ist vollständig, der zweite Ring hat einen Schlitz, sodass keine Ringströme fließen könnnen. Beide Ringe werden auf einen U-Kern mit Eisenjoch und einer Spule auf dem U-Kern gesteckt. An die Spule wird eine starke Wechselspannung angelegt. <br> Frage mich nun zunächst nach meiner Beobachtung des Experiments. Wenn ich eine zufriedenstellende Antwort gegeben haben, dann frage mich nach meiner Erklärung für das Experiment. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte oder zur nächsten Frage bzw. zur Einschätzung kommen möchte. <br> Alle Antworten sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir am Ende das Niveau meiner Antworten auf einer Skala von 1 bis 10 ein.</span>
</div>

<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


#### C. Magnetisches Pendel (Induktionsbremse)

<p style="color:blue">
Aufgabe: Zeichne (Skizze), beschreibe (Beobachtung) und erkläre (Erklärung) das Experiment magnetisches Pendel in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen.
</p>

__Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.__

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessernn.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Ich soll ein Experiment erst beschreiben und anschließend erklären. Bitte frage mich zunächst nach einer Beschreibung meiner Beobachtung. Unterstütze mich bei der Antwort, hilf mir nur, wenn ich darum bitte. Achte bei meiner Erklärung darauf, dass die Induktion einer Spannung richtig beschrieben wird und die Lenz'sche Regel korrekt erklärt wird. <br> Ein Aluminiumrad hängt frei auf einer Achse und kann sich drehen. Am unteren Ende des Aluminiumrades sind zwei Polschuhe eines Elektromagneten (Spule mit U-Kern) rechts und links des Rades angebracht. Liegt am Elektromagneten keine Spannung an und das Rad wird angestoßen, so dreht es sich weiter bis es nach einiger Zeit aufgrund der Reibung zum stehen kommt. Wird an den Elektromagneten eine Gleichspannung angelegt, so bremst das Rad ab. Je größer die Spannung, desto schneller wird das Rad gebremst. <br> Frage mich nun zunächst nach meiner Beobachtung des Experiments. Wenn ich eine zufriedenstellende Antwort gegeben haben, dann frage mich nach meiner Erklärung für das Experiment. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte oder zur nächsten Frage bzw. zur Einschätzung kommen möchte. <br> Alle Antworten sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir am Ende das Niveau meiner Antworten auf einer Skala von 1 bis 10 ein.</span>
</div>

<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


#### Experiment: Realer Transformator

<p class="newspaper">

__Aufgabe:__ 

Baue einen Transformator nach folgendem Vorbild auf. Nutze die Cassy-Messgeräte um Primär- und Sekundärspannung für verschiedene Kominationen aus Primär- und Sekundärwindungszahl zu untersuchen.

__Einstellungen:__

Nutze am Spannungsversorgungsgerät die Einstellung: __Wechselspannung, 6V__. Nutze am Cassy-Messgerät die Einstellung für die __Erfassung: Effektivwerte (AC+DC)__

__Analyse:__ 

Zeichne einen Graphen mit $n=\dfrac{N_1}{N_2}$ auf der x-Achse und $n'= \dfrac{U_1}{U_2}$ auf der y-Achse.

<p class="cb">

![Aufbau_Transformator](https://diversewolken.ddns.net/nextcloud/index.php/s/pmQD7JM7pBTG45k/download)

</p>

</p>

{{0-1}}
*********
<!--
     data-schow="false"
     data-title=""
     data-type="line"
     data-xlabel="N1/N2"
     data-ylabel="U1/U2"
-->
| $n=\dfrac{N_1}{N_2} $ | $U_1$ in V | $U_2$ in V | $n' = \dfrac{U_1}{U_2}$ |
| ---- | ---- | ---- | ---- |
| $\dfrac{2400}{800}=3$ | .. | .. | .. |
| $\dfrac{2400}{1600}=1,5$ | .. | .. | .. |
| $\dfrac{2400}{2400}=1$ | .. | .. | .. |
| $\dfrac{1600}{800}=2$ | .. | .. | .. |
| $\dfrac{1600}{1600}=1$ | .. | .. | .. |
| $\dfrac{1600}{2400}=0,67$ | .. | .. | .. |
| $\dfrac{800}{800}=1$ | .. | .. | .. |
| $\dfrac{800}{1600}=0,5$ | .. | .. | .. |
| $\dfrac{800}{2400}=0,33$ | .. | .. | .. |
*********

{{1-2}}
*********
<!--
     data-schow="false"
     data-title=""
     data-type="line"
     data-xlabel="N1/N2"
     data-ylabel="U1/U2"
-->
| $n=\dfrac{N_1}{N_2}$ | $U_1$ in V | $U_2$ in V | $n' = \dfrac{U_1}{U_2}$ |
| ---- | ---- | ---- | ---- |
| $\dfrac{2400}{800}=3$ | 6,5 | 2,01 | .. |
| $\dfrac{2400}{1600}=1,5$ | 6,5 | 4,05 | .. |
| $\dfrac{2400}{2400}=1$ | 6,5 | 6,07 | .. |
| $\dfrac{1600}{800}=2$ | 6,5 | 3,04 | .. |
| $\dfrac{1600}{1600}=1$ | 6,5 | 6,11 | .. |
| $\dfrac{1600}{2400}=0,67$ | 6,5 | 9,15 | .. |
| $\dfrac{800}{800}=1$ | 6,5 | 6,09 | .. |
| $\dfrac{800}{1600}=0,5$ | 6,5 | 12,25 | .. |
| $\dfrac{800}{2400}=0,33$ | 6,5 | 18,33 | .. |
*********


{{2-3}}
*********
<!--
     data-show="false"
     data-title=""
     data-type="line"
     data-xlabel="N1/N2"
     data-ylabel="U1/U2"
-->
| n | n' | n |
| ---- | ---- | ---- |
| 0 | 0 | 0 |
| 3 | 3.23 | 3 |
| 1.5 | 1.62 | 1.5 |
| 1 | 1.07 | 1 |
| 2 | 2.14 | 2 |
| 1 | 1.06 | 1 |
| 0.67 | 0.71 | 0.67 |
| 1 | 1.07 | 1 |
| 0.5 | 0.53 | 0.5 | 
| 0.33 | 0.35 | 0.33 |
*********

{{3-4}}
*********
| n | n' | n | n/n' |
| ---- | ---- | ---- | --- |
| 0 | 0 | 0 | - |
| 3 | 3.23 | 3 | |
| 1.5 | 1.62 | 1.5 | |
| 1 | 1.07 | 1 | |
| 2 | 2.14 | 2 | |
| 1 | 1.06 | 1 | |
| 0.67 | 0.71 | 0.67 | |
| 1 | 1.07 | 1 | |
| 0.5 | 0.53 | 0.5 | |
| 0.33 | 0.35 | 0.33 | |
*********

{{4}}
*********
| n | n' | n | n/n' |
| ---- | ---- | ---- | --- |
| 0 | 0 | 0 | - |
| 3 | 3.23 | 3 | 0.93 |
| 1.5 | 1.62 | 1.5 | 0.93 |
| 1 | 1.07 | 1 | 0.93 |
| 2 | 2.14 | 2 | 0.93 |
| 1 | 1.06 | 1 | 0.94 |
| 0.67 | 0.71 | 0.67 | 0.94 |
| 1 | 1.07 | 1 | 0.93 |
| 0.5 | 0.53 | 0.5 | 0.94 |
| 0.33 | 0.35 | 0.33 | 0.94 |
*********

{{5}}
*********
> Bei einem __realen unbelasteten__ Transformator gilt:
>
> $$\dfrac{U_1}{U_2} > \dfrac{N_1}{N_2}$$
*********

#### Begriffsklärung: Transformator

> __Idealer vs. realer Transformator__: Der ideale Transformator ist ein theoretisches Modell, bei dem einige Vereinfachungen (Idealisierungen) angenommen werden. <br> Zum Beispiel:
>
> - das magnetische Feld verläuft zu 100% im Inneren des Eisenkerns (d.h. die erzeugte magnetische Flussdichte in der Primärspule ist identisch mit der wirkenden magnetischen Flussdichte in der Sekundärspule)
>
> - der Draht der Wicklungen hat keinen elektrischen Widerstand (es entstehen keine Wärmeverluste)
>
> - innerhalb des Eisenkerns werden keine Wirbelströme induziert (keine Verluste, keine Hysterese)

> __Belasteter vs. unbelasteter Transformator__: Bei einem unbelasteten Trafo wird angenommen, dass im Sekundärstromkreis kein Verbraucher angeschlossen ist, d.h. es fließt kein Sekundärstrom. Die Gleichung 
>
> $$\dfrac{U_1}{U_2} = \dfrac{N_1}{N_2}$$
>
> gilt nur für einen __unbelasteten idealen Transformator__.

