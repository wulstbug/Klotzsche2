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

### 2.4.2 Wirkungsgrad eines Benzinmotors

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

@timer(10,00)

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
> - die Menge @color(erneuerbarer Energien Wasser-Sonne-Wind-Biomasse,red) ist ebenfalls gestiegen
*************


2. Ermittle aus dem Diagramm, den Anteil erneuerbarer Energien (in Prozent von der Gesamtenergie) im Jahr 1960 und vergleiche ihn mit dem Anteil im Jahr 2015.

<p class="newspaper">

{{4}}
*************
> - 1960
>
> $$ \dfrac{0,2\,cm}{2,2\,cm} \cdot 100 \% \approx 10\% $$

<p class="cb">

{{5}}
*************


> - 2015
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
<p class="newspaper">

@color(_Diagramm skizzenhaft übernehmen_, blue)

![Energiebedarf2](https://diversewolken.ddns.net/nextcloud/index.php/s/bxotwGjptqE73fy/download "Genutzte __primäre__ Energiequellen der Menschheit (LB S.31)")

<p class="cb">

@color(__siehe Diagramm LB S. 31__, blue)

__Nutzung primärer Energiequellen (1960-2015):__

> - die Nutzung @color(primärer Energiequellen,red) ist im Lauf der letzten 50 Jahre gestiegen, sie hat sich mehr als verdoppelt
>
> - die bereitgestellte Menge @color(erneuerbarer Energien Wasser-Sonne-Wind-Biomasse,red) ist ebenfalls gestiegen

</p>

</p>

__Anteil erneuerbarer Energien (1960-2015):__

<p class="newspaper">

> - 1960
>
> $$ \dfrac{0,2\,cm}{2,2\,cm} \cdot 100 \% \approx 10\% $$

<p class="cb">

> - 2010
>
> $$ \dfrac{1,6\,cm}{5,6\,cm} \cdot 100 \% \ \approx 30\% $$

</p>

</p>

***********

## 2.6 Die Bereitstellung elektrischer Energie in modernen Gesellschaften

@timer(10,00)

> @color(Elektrische Energie,red) spielt in modernen westlichen Gesellschaften eine wichtige Rolle. Sie wird durch verschiedene Arten von __Kraftwerken__ bereit gestellt. 
>
> Kraftwerke wandeln primäre Energiequellen (Gas, Kohle, Kernbrennstoff, Windenergie, Wasserenergie) in @color(elektrische Energie,red) um

{{1-6}}
**********
__siehe LB S. 37/38__

__Aufgaben:__ 

<i style="color:blue">

1. Übernimm den Merksatz (oben)

---

2. 1. Lies den Text "Die Bedeutung elektrischer Energie" (LB S. 37)

2. 2. Notiere drei Gründe, warum elektrische Energie für moderne Gesellschaften einen große Bedeutung hat

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
![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/Xbf7QmBSmwzN4GK/download)
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

## Generator selber bauen

__Aufgabenstellung:__ Nutze in einer Gruppe von zwei Leuten den Bausatz und baue den Generator auf. Am Lehrertisch gibt es ein Demogerät. Experimentiere mit dem Generator anhand folgender Aufgaben

{{1}}
*******
<p class="newspaper">

__Der Generator:__

1. Schließe an den Generator das Cassy-Messgerät zur Spannungsmessung an. (nur @color(roten,red) und @color(blauen, blue) Pol verwenden.)

2. Stelle das Cassy-Messgerät bei der Spannungseinstellung (__Messbereich__) auf -0,3 bis 0,3 V.

3. Drehe an der Welle und überprüfe die angezeigte Spannung. <br> @color(-> Der Spannungsmesser sollte ausschlagen.,orange)

4. Drehe die Welle in die andere Richtung und überprüfe die angezeigte Spannung. Was stellst du fest?

    @color(Spannung wechselt das Vorzeichen, orange)


<p class="cb">

{{3}}
***********
__Der Elektro-Motor:__
***********

{{2}}
****************
5. Besorge dir am Lehrertisch eine Spannungsquelle. Schließe die Spannungsquelle statt dem Cassy-Messgerät an den Generator an. Erhöhe langsam die Spannung.

     <bdi style="color:red">$\boxed{\textbf{ACHTUNG: SPANNUNG}}$</bdi>

     <bdi style="color:red">$\boxed{\textbf{NICHT ÜBER 2V ERHÖHEN}}$</bdi>

6. Welche andere Funktion kann ein Generator übernehmen?

7. Vertausche die Pole der Spannungsquelle und beobachte das Verhalten deines Experimentes.
****************
</p>

</p>
*******

## 2.7 Die Funktionsweise eines Generators

Ein einfacher __Generator__ besteht typischer Weise aus einem @color(Magneten, orange) und einer @color(Spule,orange), welche sich im Magnetfeld drehen kann.

{{1}}
**************
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
**************

{{2}}
**************
__Video: Wie funktioniert ein Generator?__

!?[EVN-Wie-Funktioniert-Ein-Generator](https://www.youtube.com/watch?v=qJCWKwpt1lg)
**************

## 2.8 Grundlage Generator: Das Induktionsgesetz

- @color(Lies LB. S. 53, blue)

- @color(Notiere das Induktionsgesetz [erster Merksatz], blue)

- @color(Ermittle die Einflussfaktoren auf die erzeugte [d.h. induzierte] Spannung, blue)

{{1}}
***********
> __Das Induktionsgesetz:__ Zwischen den Enden einer Spule wird eine Spannung @color(induziert, red), wenn sich das von ihr umfasste Magnetfeld ändert. 
***********

{{2}}
***********
> __Die Induktionsspannung:__ Die Induktionsspannung ab hängt vom 
> 
> 1. Bau der Spule (__Windungszahl__, __Querschnittsfläche__) 
>
> 2. wie schnell und wie stark sich das __Magnetfeld__ in der Spule ändert.
***********

{{3}}
***********
> __Nutzen der Induktion:__ Da bei der Induktion die Bewegung des Rotors in elektrische Spannung "umgesetzt" wird, war es mit der Entdeckung der Induktion (1831) erstmals möglich 
>
>> @color(__mechanische Energie__, blue) in @color(__elektrische Energie__, red) umzuwandeln.
***********

### Fragen zum Generator 2

@timer(08,00)

@color(Beantwortet die Fragen 1 und 2 auf dem Arbeitsblatt __allein__. Überprüft anschließend mit dem Nachbarn/der Nachbarin gegenseitig die Fragen 3.-8., blue)

1. Bei einem Generator wird das Induktionsgesetz genutzt. Notiere es.

    {1}{<bdi style="color:orange">In einer Spule wird eine Spannung induziert, solange sich das von der Spule umfasste Magnetfeld ändert.</bdi>}

<p class="newspaper">

2. Beschreibe anhand der Skizze den Aufbau eines Wechselstromgenerators. 

    {2}{<bdi style="color:orange"> Ein Wechselstromgenerator besteht aus einem rotierenden Magneten (Rotor) und fest stehenden Induktionsspulen (Stator). </bdi>}

<p  class="cb">

![AB_Generator](https://diversewolken.ddns.net/nextcloud/index.php/s/5m3cZF62Y7DoNms/download)

</p>

</p>

{{3}}
**********
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
**********

## 2.9 Die Generator-Spannung

## Simulation 1

??[PHET_Generator](https://phet.colorado.edu/sims/html/generator/latest/generator_all.html?locale=de)

## Simulation 2

??[Fendt_Generator](https://www.walter-fendt.de/html5/phde/generator_de.htm)

## Simulation 3

[LEIFI-Generator](https://www.leifiphysik.de/elektrizitaetslehre/wechselstromtechnik/versuche/erzeugung-sinusfoermiger-wechselspannung)


## 2.9 Die induzierte Spannung am Generator

> Ein Generator in seiner einfachsten Bauform mit Magnet und Spule erzeugt eine Spannung, die mit der Zeit ihren __Wert__ und ihr __Vorzeichen__ (d.h. $\oplus$ und $\ominus$ ) ändert.
>
> Eine solche Spannung nennt man @color(__Wechselspannung__ $U$~,red).


{{1-5}}
**********
__Beispiel einer Wechselspannung:__

![Wechselspannung](https://diversewolken.ddns.net/nextcloud/index.php/s/yqQtJBq5kcN3p2r/download "Quelle: https://www.sanier.de/elektroinstallation/spannungsarten-und-stroeme" )<!-- style="max-width:500px" -->
**********

{{5}}
**********
![Wechselspannung](https://diversewolken.ddns.net/nextcloud/index.php/s/9kfekzHmQteXnca/download "Quelle: https://www.sanier.de/elektroinstallation/spannungsarten-und-stroeme" )<!-- style="max-width:500px" -->
**********

{{2}}
**********
__Eigenschaften einer Wechselspannung:__

| | | |
| {3}{__Amplitude $\hat{U}$__} | {4}{__Periodendauer $T$__} |  {6}{__Frequenz $f=\frac{1}{T}$__} |
| {3}{Die Amplitude gibt den @color(Maximalwert der Spannung,orange) an.} | {4}{@color(Zeit, orange) zwischen zwei Maxima.} | {6}{Die Frequenz gibt an, wie oft die Spannung ihren @color(Maximalwert pro Sekunde, orange) erreicht.} |
| {3}{Einheit [V]} | {4}{Einheit [s]} | {6}{Einheit __1 Hertz__  [ 1Hz = $\frac{1}{s}$]} |
**********

## 2.10 Wechselspannung und Dioden

Eine Diode wird (mit einem Schutzwiderstand) an eine Wechselspannung angeschlossen. 

@color(_Was kann man beobachten?_, blue) <br> <br>

<p class="newspaper">

{1}{![DiodeWechselSpannung](https://diversewolken.ddns.net/nextcloud/index.php/s/AYWgzemZr89zamr/download)}

<p class="cb">

{{2}}
*******
!?[Diode50Hz](https://youtu.be/qXN1QMhcvEU)
*******

</p>

</p>

{{3}}
********
__Beobachtung:__ Da die Spannung ständig die Pole ändert, wird die Diode regelmäßig in __Durchlass-__ und __Sperrrichtung__ geschaltet.

-> Die Diode geht an und aus.
********

## Aufgaben zur Wechselspannung 1

Bestimme für die Netzspannung einer Haushaltssteckdose Amplitude, Periodendauer und Frequenz (_Achte auf die Einheiten_).

![Netzspannung](https://diversewolken.ddns.net/nextcloud/index.php/s/jmBedzyFa2xBTLF/download "Quelle: https://www.sonnentaler.net/dokumentation/wiss/elektrizitaet/grundlagen/elektrik-im-haus/")<!-- style="min-width:60%"-->

@color(_Hinweis: 1000 ms = 1 s_, red)

__Lösungen:__

1. Amplitude 

@rangeQuiz2($\hspace{1cm}$ $\hat{U}$, 325, $V$)

2. Periodendauer 

@rangeQuiz2($\hspace{1cm}$$T$, 0.02, $s$)

3. Frequenz

@rangeQuiz2($\hspace{1cm}$$f$, 50, $\dfrac{1}{s}$)

## 2.11 Die Netzspannung im Haushalt

> Die Spannung an einer herkömmlichen Steckdose hat eine Amplitude von $\hat{U} = 325 V$. 
>
> Im Alltag wird aber ein Mittelwert angegeben, er beträgt $\bar{U} = 230 V$.
>
> Die Frequenz beträgt $f = 50 Hz= 50 \frac{1}{s}$.

![Netzspannung](https://diversewolken.ddns.net/nextcloud/index.php/s/jmBedzyFa2xBTLF/download)

@color(_Notiere folgende Übersicht im Hefter._,blue)


## Aufgaben zur Wechselspannung 2

<iframe src="https://learningapps.org/watch?v=p23wxsi7224" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

## Aufgaben zur Wechselspannung 3

[QuizZumGenerator](https://www.leifiphysik.de/elektrizitaetslehre/induktion-und-transformator/aufgabe/quiz-zum-generator)

## Aufgabe zur Wechselspannung 4

Eine Glühlampe wird (mit einem Schutzwiderstand) an eine Wechselspannung angeschlossen. 

@color(_Was kann man beobachten?_, blue) <br> <br>

<p class="newspaper">

{1}{![GlühlampeWechselSpannung](https://diversewolken.ddns.net/nextcloud/index.php/s/3C3Bgw3RmCExGNy/download)}

<p class="cb">

{{2}}
*******
@color(Notiere deine Vermutung, blue)

__Bring dein Tablet zurück in den Tabletschrank!__
*******

</p>

</p>



## 2.14 E = mc² - Was bedeutet das?

![Emc2](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjvaU4S7ZdTFeYPO_Y35x5BTvwXeKgnYSXqzDKfg6mvkyEp-o0wNR4lt8PhZTomPbP-kXhcNNWJYegNFO3k_4ZO_x2uyv_7h7HRSPie0xc9XxNsuHz_IrMJQOtPQeLtLmZoc1DubOQ5xWQ/s1600/energy+mass+equivalence+albert+einstein+history+science+physics.jpg)

### Quiz Kernspaltung und Kernfusion

__Teil A:__

1. Die Explosion einer Atombombe wird durch eine unkontrollierte Kettenreaktion verursacht.

     [(x)] wahr
     [( )] falsch

2. Es ist möglich, Quecksilber mithilfe von Kernspaltung in Gold zu verwandeln.

     [(x)] wahr
     [( )] falsch

3. Die meisten Kernkraftwerke verwenden Lithium als Brennstoff.

     [( )] wahr
     [(x)] falsch

4. Kernfusionsreaktoren beziehen ihre Energie durch kontrollierte Kettenreaktionen.

     [(x)] wahr
     [( )] falsch


__Teil B:__

1. Was ist eine Kettenreaktion?

     [( )] Eine Reihe von chemischen Reaktionen, von denen jede das Produkt einer vorangegangenen Reaktion als eine ihrer Reaktionsmittel verwendet.
     [( )] Eine Reihe von Reaktionen auf verschiedene Reize von außen.
     [(x)] Eine Reihe von Kernspaltungsreaktionen, von denen jede mit einem Neutron begann, das während einer vorhergegangenen Kernspaltungsreaktion freigesetzt wurde.
     [( )] Eine Reihe von Kernfusionsreaktionen, von denen jede die Bindung eines Atomkerns beinhaltet, welcher in einer vorhergegangenen Kernfusionsreaktion erzeugt wurde.

2. Was sind Quellen von Kernenergie?

     [[ ]] Zellteilung
     [[x]] Kernspaltung
     [[ ]] Freisetzung von Elektronen
     [[x]] Kernfusion

3. Was ist die Wärme- und Lichtquelle eines Sterns?

     [( )] Verbrennung von fossilen Brennstoffen
     [( )] Kernspaltung
     [(X)] Kernfusion 
     [( )] Potentielle Energie

4. Wie nennen wir den Vorgang, in dem zwei kleine Atomkerne zu einem größeren Kern verschmelzen?

     [( )] Kernspaltung
     [( )] Redundanz
     [(x)] Kernfusion
     [( )] Alchemie


__Teil C__

1. Wie nennt man den Vorgang, in dem ein schwerer Atomkern sich in zwei oder mehrere kleinere Kerne spaltet und dabei Neutronen und Energie freigegeben werden?

     [[Kernspaltung]]

2. Welche der folgenden Optionen sind Schritte in der Elektrizitätserzeugung durch eine Kernspaltungsreaktion mit Uran?

     [[x]] Der Dampf treibt eine Turbine an, die einen Generator mit Energie versorgt.
     [[ ]] Zwei Uran-Atomkerne verschmelzen miteinander und bilden einen schwereren Kern. Dieser Vorgang setzt einige freie Neutronen und eine große Menge an Energie frei.
     [[x]] Der Uran-Atomkern wird von einem Neutron getroffen. Er spaltet sich und gibt zwei leichtere Kerne sowie einige freie Neutronen frei.
     [[x]] Die kinetische Energie der neuen Atomkerne und der freien Neutronen wird in Wärme umgewandelt.
     [[x]] Die Wärme wird zum Wasserkochen verwendet, wodurch Dampf entsteht.
     [[ ]] Die freien Neutronen prallen gegen eine Turbine, wodurch die Turbine sich dreht und einen Generator mit Energie versorgt.

3. Aluminium weist die Ordnungszahl 13 auf, Eisen die Ordnungszahl 26 und Tellur die Ordnungszahl 52. Welche der folgenden Reaktionen können thypothetisch Eisen produzieren?

     [[x]] Kernspaltung von Tellur.
     [[ ]] Kernspaltung von Aluminium.
     [[ ]] Kernfusion von Tellur.
     [[x]] Kernfusion von Aluminium.

4. Wie nennt man den Vorgang, in dem zwei leichte Atomkerne zu einem schwereren Kern verschmelzen und dabei große Energiemengen freigegeben werden?

     [[Kernfusion]]

5. Welche dieser Optionen stellen Produkte aus der Kernfusion von Wasserstoff in der Sonne dar?

     [[ ]] Gold
     [[x]] Energie in Form von Wärme und Strahlung
     [[x]] Helium
     [[ ]] Uran
     
6. Welche der folgenden Optionen können mit einem Atom geschehen, nachdem es ein Neutron absorbiert hat?

     [[x]] Es kann eventuell instabil werden und sich in zwei oder mehrere kleinere Atomkerne spalten.
     [[x]] Es kann eventuell Neutronen freisetzen.
     [[ ]] Es kann eventuell all seine Elektronen freisetzen.
     [[x]] Es kann eventuell Energie freisetzen.

## 2.14 E = mc² - oder - Woher kommt die Energie bei Kernspaltung und Kernfusion

Die berühmte Formel

> $$ \boxed{E=m \cdot c^2} $$

bedeutet in Worten, dass {1}{@color(Energie und Masse identisch sind, red)}. {2}{Anders ausgedrückt, steckt in der Masse eines Körpers seine Energie.}

{{3}}
***********
[LEIFI-Massendefekt](https://www.leifiphysik.de/kern-teilchenphysik/kernreaktionen/grundwissen/masse-energie-beziehung)

__Beispiel: [Kernspaltung-U-235](https://www.leifiphysik.de/kern-teilchenphysik/kernspaltung-und-kernfusion/grundwissen/kernspaltung)__

| __Ausgangskerne__ | | __Reaktionsprodukte__ |
| $$ ^{235}_{92}\mathrm{U} + ^{1}_{0}n $$ | $\rightarrow$ | $$ ^{144}_{56}\mathrm{Ba} + ^{89}_{36}{\mathrm{Kr}}  + 3 \cdot ^{1}_0n + \mathrm{Energie} $$ |
| {5}{235,044u<br>+1,009u<br>---------} | {5}{$\rightarrow$}| {8}{143,923u<br>+88,918u<br>+3∙1,009u<br>---------}|
| {6}{<bdi style="color:blue">236,053u</bdi>} | {10}{__>__} | {9}{<bdi style="color:red">235,868u</bdi>} | 
***********

<p class="newspaper">

{{4}}
************
_Masse eines U-235 Atoms:_

> $m_{\mathrm{U-235}} = 235,044 u$
>
> _Hinweis: Die Einheit u heißt @color(atomare Masseneinheit,blue)_:
>
> $1u = 1,6605 \cdot 10^{-27} kg$

_Masse eines Neutrons:_

> $m_{\mathrm{n}} = 1,009 u$
************


<p class="cb">

{{7}}
************
_Masse eines Ba-144 Atoms_

> $m_{\mathrm{Ba-144}} = 143,923 u$

_Masse eines Kr-89 Atoms_

> $m_{\mathrm{Kr-89}} = 88,918 u$
************

</p>

</p>


{{10}}
********
> __Bei der Kernspaltung ging eine Masse von__
>
> $\Delta m$ = <bdi style="color:blue">236.053u</bdi> - <bdi style="color:red">235,868u</bdi> = __0,185 u__
>
> __verloren. Nach E=mc² ist Masse gleich Energie. Die verlorene Masse $\Delta m$ nennt man @color(Massendefekt ,red) und wird in Form von Energie freigesetzt.__
********

{{11}}
********

> $ E = \Delta m \cdot c^2 $
>
> $ E = 0,185 \cdot 1,6605 \cdot 10^{-27} kg \cdot (3 \cdot 10^8 \frac{m}{s})^2 $$
>
> $ E = 2,764\cdot 10^{-11} J$

Für jedes U-235 Atom, dass gespaltet wird, wird die Energie $2,764\cdot 10^{-11} J$ frei.
********

<p class="newspaper">

{{12}}
********
1kg angereichertes Uran (5% U-235) enthält ca. $1,28 \cdot 10^{23}$ Atome. <br> D.h. 1kg Uran-235 enthält potentiell die freisetzbare Energie von
********

{{13}}
********
> $ E = 2,764\cdot 10^{-11} J \cdot 1,38 \cdot 10^{23}$
>
> $ E = 3,81 \cdot 10^{12} J \approx 3`800`000 MJ$
********

<p class="cb">

{{14}}
********
Zum Vergleich: 

1kg TNT Sprengstoff enthällt eine Energie von ca.

> $ E = 4,18 \cdot 10^6 J$
>
> $ E = 4,18 MJ$
********

</p>

</p>

### Aufgaben zu 2.14

In [dieser Formelsammlung](https://www.iqb.hu-berlin.de/abitur/abitur/dokumente/naturwissenschaften/N_Mathematischna.pdf) findest du ab Seite 65 die Atommassen ausgewählter Nuklide.

Ziel ist es, den Massendefekt folgender Reaktion zu ermitteln.

$$ ^{239}_{94}\mathrm{Pu} + ^{1}_{0}n \rightarrow ^{144}_{56}\mathrm{Ba} + ^{94}_{38}{\mathrm{Sr}}  + 2 \cdot ^{1}_0n + \mathrm{Energie} $$ 


1. Ermittle die Atommasse der folgenden Nuklide.

1. 1. Pu-239: 

@rangeQuiz2($\hspace{1cm}$ $m_{\mathrm{Pu-239}}$, 239.052 , $u$)

1. 2. Neutron

@rangeQuiz2($\hspace{1cm}$ $m_{\mathrm{n}}$, 1.009 , $u$)

1. 3. Ba-144

@rangeQuiz2($\hspace{1cm}$ $m_{\mathrm{Ba-144}}$, 143.923, $u$)

1. 4. Sr-94

@rangeQuiz2($\hspace{1cm}$ $m_{\mathrm{Sr-94}}$, 93.915, $u$)

2. 1. Addiere nun die Massen der linken und der rechten Seite zusammen.

<p style="margin-left:10%">

<p class="newspaper">

__Ausgangskerne__ 

$$ ^{239}_{94}\mathrm{Pu} + ^{1}_{0}n $$

@rangeQuiz2($m_{\mathrm{ausg}}$, 240.061, $u$)

<p class="cb">

__Reaktionsprodukte__ 

$$ ^{144}_{56}\mathrm{Ba} + ^{94}_{38}{\mathrm{Sr}}  + 2 \cdot ^{1}_0n $$

@rangeQuiz2($m_{\mathrm{reakt}}$, 239.856, $u$)

</p>

</p>

</P>

2. 2. Ermittle den Massendefekt $\Delta m$ (Massenverlust)

@rangeQuiz2($\hspace{1cm}$ $\Delta m$ ,0.205 ,$u$)

2. 3. Ermittle aus dem Massendefekt die Energie

<p style = "margin-left:10%">

$ E = \Delta m \cdot c^2 $

$ c = 3 \cdot 10^8 \frac{m}{s} $

$ u = 1,66 \cdot 10^{-27} kg$

@rangeQuiz2($E$ , 3.0627e-11 ,$J$)

</p>
