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

mode: presentation

-->

# 2. Energieversorgung

@uhr

{{1}}
*****************
> __Definition:__ Energie beschreibt die Fähigkeit:
*****************
{{2}}
*****************
>- mechanische Arbeit zu verrichten (z.B. Beschleunigen, Verformen)
>- Licht auszusenden
>- Wärme abzugeben
*****************

## 2.1. Energieformen

>__Mechanische Energie:__
>
>- Kinetische Energie (Bewegungsenergie) 
>- Potentielle Energie (Lageenergie)
>- Rotationsenergie (Drehungen)
>- Spannenergie (z.B. Feder, Bungeeseil)

>- Thermische Energie (Wärmeenergie)
>- __Elektrische Energie__
>- Magnetische Energie
>- Strahlungsenergie (Lichtenergie)
>- Chemische Energie
>- Kernenergie (Atomenergie)

## 2.1. _Übung: Zuordnung Energieformen_

Übung 1: _Zuordnung Energieformen_

<iframe src="https://learningapps.org/watch?app=23986132" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

Übung 2: _Zuordnung Energieformen_
<iframe src="https://learningapps.org/watch?app=28854190" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

## 2.2 Energieerhaltungssatz

> __Energieerhaltung:__ Energie kann weder erzeugt noch vernichtet werden, sondern nur von einer Form in eine andere umgewandelt werden.

## 2.3 Energieflussdiagramme(EFD) / Energieumwandlungsketten

__Definition:__ Ein Energieflussdiagramm __EFD__(Synonym: Energieumwandlungskette) stellt Energieumwandlungen grafisch dar.

__Beispiel:__ Glühlampe

<!-- style="width:50%" -->
``` ascii
              '----------'
              |          |
           .->| Lichten. |
'--------'/   |          |
|        |    '----------'
|el. En. |  
|        |
'--------'\   '----------'
           .->|          |
              | Wärmeen. |
              |          |
              '----------'
```

## 2.4 Der Wirkungsgrad $\eta$ oder "Die Effizienz von Energiewandlern"

> Häufig kann man bei einem Energiewandler nur eine Form der umgewandelten Energie nutzen. Die anderen Energieformen gehen verloren, man sagt, sie sind __entwertet__.

> Der Wirkungsgrad $\eta$ defniert die Effizienz einer Energieumwandlung. Er ist definiert als:
>
> $$ \eta = \boxed{\dfrac{E_{nutz}}{E_{zu}}} $$
>
> mit
>
> $\hspace{1cm}$ $E_{nutz}$ .. genutzte Energie 
>
> $\hspace{1cm}$ $E_{zu}$ .. zugeführte Energie

>> Der Wirkungsgrad $\eta$ gibt an, wie effizient ein Energiewandler die zugeführte Energie in die genutzte Energie umwandelt.

### 2.4.1 Wirkungsgrad am Beispiel von Glühlampe und LED

> __Energieumwandlungen von__

<p class="newspaper">

> __Glühlampe__

{{1}}
*********
<!-- style="width:50%" -->
``` ascii
            '----------'
            | Lichten. |
           ^|----------|
'--------'/ |  5 J     |
| el. En.|  '----------'
|--------|  
|  100 J |
'--------'\ '----------'
           v| Wärmeen. |
            |----------|
            |  95 J    |
            '----------'
```
*********

<p class="cb">

> __LED__

{{2}}
*********

<!-- style="width:50%" -->
``` ascii
            '----------'
           ^| Lichten. |
'--------'/ |----------|
| el. En.|  |  40 J    |
|--------|  '----------'
|  100 J |
'--------'\ '----------'
           v| Wärmeen. |
            |----------|
            |  60 J    |
            '----------'
```

*********

</p>

</p>

> __Aufgabe:__ Bestimme den Wirkungsgrad von Glühlampe und LED.

<p class="newspaper">

{{3}}
**************

__Glühlampe__

geg.: <br>
 
$\hspace{0.5cm}$ $E_{el}$ = 100 J

$\hspace{0.5cm}$ $E_{Licht}$ = 5 J

$\hspace{0.5cm}$ $E_{therm}$ = 95 J

ges.: <br>

$\hspace{0.5cm}$ $\eta$

{{4}}
**************
Lsg.:

$\hspace{0.5cm}$ $\eta = \dfrac{E_{nutz}}{E_{zu}} = \dfrac{E_{Licht}}{E_{el}}$

$\hspace{0.5cm}$ $\eta = \dfrac{5 J}{100 J} = 0,05 = 5\%$ 
**************

**************

<p class="cb">

__LED__

{{5}}
*************
geg.: <br>
 
$\hspace{0.5cm}$ $E_{el}$ = 100 J

$\hspace{0.5cm}$ $E_{Licht}$ = 40 J

$\hspace{0.5cm}$ $E_{therm}$ = 60 J

ges.: <br>

$\hspace{0.5cm}$ $\eta$

Lsg.:
************

{{6}}
*************
$\hspace{0.5cm}$ $\eta = \dfrac{E_{nutz}}{E_{zu}} = \dfrac{E_{Licht}}{E_{el}}$

$\hspace{0.5cm}$ $\eta = \dfrac{40 J}{100 J} = 0,4 = 40\% $ 
*************


</p>

</p>

{{7}}
***********
> __Vergleich:__ Die LED wandelt die elektrische Energie viel effizienter in Licht um als die Glühlampe, denn sie hat einen höheren Wirkungsgrad (40% > 5%)
***********

## 2.4.2 Wirkungsgrad eines Benzinmotors

> Über die Benutzung eines Benzinmotors bei einem Auto sind folgende Dinge bekannt:
>
> $E_{chem} = 6000 J$
>
> $E_{kin} = 1800 J$ (_hier sei Rotationsenergie enthalten_)
>
> $E_{therm} = 3900 J$
>
> $E_{el} = 150 J$.

__Aufgabe:__ Berechne den Wirkungsgrad, wenn es das Ziel ist:

- a) mit dem Auto zu fahren

- b) das Auto als Heizung zu verwenden

- c*) die Glühlampe im Auto zum Lesen zu verwenden.

__Lösung überprüfen:__ 

{{1}}
*************
<!-- data-solution-button=off -->
a) $\eta$ = [[ 0,3 ]] 
[[?]] Überlege, welches im Fall a) die zugeführte und welches die genutze Energieform ist. Verwende dann die Formel für $\eta$
[[?]] Die zugeführte Energieform beim Benzinmotor ist chemische Energie. Die genutzte Energieform (wenn man fahren will) ist kinetische Energie.
[[?]] $\eta = \frac{E_{kin}}{E_{chem}}=\frac{1800 J}{6000 J}$
*************

{{2}}
*************
<!-- data-solution-button=off -->
b) $\eta$ = [[ 65 ]] %
[[?]] Hier ist $\eta$ in Prozent gefordert
[[?]] Überlege, welches im Fall a) die zugeführte und welches die genutze Energieform ist. Verwende dann die Formel für $\eta$
[[?]] Die zugeführte Energieform beim Benzinmotor ist chemische Energie. Die genutzte Energieform (wenn man heizen will) ist thermische Energie.
[[?]] $\eta = \frac{E_{therm}}{E_{chem}} \cdot 100\%=\frac{3900 J}{6000 J}\cdot 100\%$
*************

{{3}}
*************
<!-- data-solution-button=off -->
c) $\eta$ = [[ 0,125 ]] %
[[?]] Dies ist eine zweistufige Energieumwandlung
[[?]] Zunächste wird chemische Energie vom Motor in elektrische umgewandelt. Dann wird die elektrische Energie von der Glühlampe in Lichtenergie umgewandelt
[[?]] chem -> el: 6000 J -> 150J. <br> Im Anschluss muss der Wirkungsgrad der Glühlampe berücksichtigt werden (siehe 2.4.1)
[[?]] Mit dem Wirkungsgrad der Glühlampe von 5% ergibt sich, dass die 150J elektrische Energie in $150\cdot0,05=7,5 J$ Lichtenergie umgewandelt werden.
[[?]] Der gesamte Wirkungsgrad beträgt also $\eta = \frac{7,5 J}{6000 J} \cdot 100\% = 0,125 \%$
*************

{{1}}
*************
_Hinweis: Klicke auf die Glühlampen für Lösungshinweise_
*************

## 2.5 Energiebedarf moderner Gesellschaften

{{0-6}}
***********

__siehe LB S. 31__

{{1}} 
***********
Lies die linke Spalte bis zum Diagramm. Beantworte dann die beiden Fragen auf einem Stichpunktzettel.
***********

{{1-3}}
*************
![Energiebedarf](https://diversewolken.ddns.net/nextcloud/index.php/s/siWycf4txMC7qLm/download "Genutzte __primäre__ Energiequellen der Menschheit (Quelle: LB S. 31)") <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->
*************

{{3}}
*************
![Energiebedarf2](https://diversewolken.ddns.net/nextcloud/index.php/s/bxotwGjptqE73fy/download "Genutzte __primäre__ Energiequellen der Menschheit (LB S.31)") <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->
*************


{{1}}
*************
1. Formuliere zwei Aussagen bezüglich der Gesamtenergie und der erneuerbaren Energie, welche man aus dem Diagramm entnehmen kann.

{{2}}
*************
> - die Nutzung @color(primärer Energiequellen,red) ist im Lauf der letzten 50 Jahre gestiegen, sie hat sich mehr als verdoppelt
>
> - die Menge @color(erneuerbarer Energien [Wasser-Sonne-Wind-Biomasse],red) ist ebenfalls gestiegen
*************


2. Ermittle aus dem Diagramm, den Anteil erneuerbarer Energien (in Prozent von der Gesamtenergie) im Jahr 1960 und vergleiche ihn mit dem Anteil im Jahr 2015.

<p class="newspaper">

{{4}}
*************
> - 1960
>
> $$ \dfrac{0,2\,cm}{2\,cm} \cdot 100 \% = 10\% $$

<p class="cb">

{{5}}
*************


> - 2010
>
> $$ \dfrac{1,6\,cm}{5,6\,cm} \cdot 100 \% \ \approx 30\% $$

*************

</p>

*************

</p>

*************

***********

{{6}}
***********

__siehe Diagramm LB S. 31 (unten)__

<p class="newspaper">

@color(_Diagramm skizzenhaft übernehmen_, blue)

![Energiebedarf2](https://diversewolken.ddns.net/nextcloud/index.php/s/bxotwGjptqE73fy/download "Genutzte __primäre__ Energiequellen der Menschheit (LB S.31)")

<p class="cb">

__Nutzung primärer Energiequellen (1960-2015):__

> - die Nutzung @color(primärer Energiequellen,red) ist im Lauf der letzten 50 Jahre gestiegen, sie hat sich mehr als verdoppelt
>
> - die bereitgestellte Menge @color(erneuerbarer Energien [Wasser-Sonne-Wind-Biomasse],red) ist ebenfalls gestiegen

</p>

</p>

__Anteil erneuerbarer Energien (1960-2015):__

<p class="newspaper">

> - 1960
>
> $$ \dfrac{0,2\,cm}{2\,cm} \cdot 100 \% = 10\% $$

<p class="cb">

> - 2010
>
> $$ \dfrac{1,6\,cm}{5,6\,cm} \cdot 100 \% \ \approx 30\% $$

</p>

</p>

***********

## 2.6 Die Bereitstellung elektrischer Energie in modernen Gesellschaften

> @color(Elektrische Energie,red) spielt in modernen westlichen Gesellschaften eine wichtige Rolle. Sie wird durch verschiedene Arten von __Kraftwerken__ bereit gestellt. 
>
> Kraftwerke wandeln primäre Energiequellen (Gas, Kohle, Kernbrennstoff, Windenergie, Wasserenergie) in @color(elektrische Energie,red) um

{{1-6}}
**********
__siehe LB S. 37/38__

__Aufgaben:__ 

<i style="color:blue">

1. übernimm den Merksatz (oben)

---

2. 1. Lies den Text "Die Bedeutung elektrischer Energie" (LB S. 37)

2. 2. Notiere drei Gründe, warum elektrische Energie einen großen praktischen Nutzen hat

{{2}}
*********
![UmwandlungElektrischerEnergie](https://diversewolken.ddns.net/nextcloud/index.php/s/49i35ds3osncYLc/download)
*********

{{3}}
*********
<p style="text-indent:10%; color:black">

> -> elektrische Energie kann aus vielen primären Energieträgern umgewandelt werden
>
> -> elektrische Energie ist leicht transportabel
>
> -> elektrische Energie lässt sich vor Ort in viele andere Energieformen umwandeln

</p>
*********

---

3. 1. Lies den Text "Beretistellung elektrischer Energie durch Kraftwerke (S.38).

3. 2. Notiere bespielhaft für drei Kraftwerkstypen den Wirkungsgrad

3. 3. Betrachte die schematische Dartellung verschiedener Kraftwerksformen (S.38/39 unten)

{{4}}
************
![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download)
************

3. 4. Überprüfe und notiere Elemente, welche in beinahe jedem Kraftwerkstyp zum Einsatz kommen

{{5}}
*********
<p style="text-indent:10%; color:black">

> -> in beinahe jedem Kraftwerkstyp (ausgenommen Solarkraftwerk) kommt ein @color(Generator,red) zum Einsatz
>
> -> Generatoren wandeln mechanische Energie(z.B. Rotationsenergie) in elektrische Energie um

</p>
*********

---

</i>

**********


{{6}}
**********

__Gründe für die Nutzung elektrischer Energie als @color(sekundäre Energiequelle , red):__

> -> elektrische Energie kann aus vielen primären Energieträgern umgewandelt werden
>
> -> elektrische Energie ist leicht transportabel
>
> -> elektrische Energie lässt sich vor Ort in viele andere Energieformen umwandeln

__Generatoren als Energiewandler für elektrische Energie:__

> -> in beinahe jedem Kraftwerkstyp (ausgenommen Solarkraftwerk) kommt ein @color(Generator,red) zum Einsatz
>
> -> Generatoren wandeln mechanische Energie(z.B. Rotationsenergie) in elektrische Energie um
**********

## Wie funktioniert ein Generator?

!?[MausStrom](https://www.youtube.com/watch?v=Je22SgH8TCk)