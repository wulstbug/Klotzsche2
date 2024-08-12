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
![SchrägerWurf_Berechnungen_2](https://diversewolken.ddns.net/nextcloud/index.php/s/DzHEmS5fHtX8bdC/download)

![SchrägerWurf_Berechnungen_3](https://diversewolken.ddns.net/nextcloud/index.php/s/DzHEmS5fHtX8bdC/download)


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
> $\hspace{1cm}$ $m = 61 kg \pm 1 kg$
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
<iframe src="https://www.geogebra.org/classic/sfkffrzq?embed" width="100%" height="200" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
***************


{{7}}
***************
> $$\mathbb{L} = \{-10,64 ; 18,51\}$$
> 
> Maximal Höhe über dem Boden beträgt $45m-(25m+18,51m)=1,49m$
***************



