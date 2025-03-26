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
    .newspaper3 {
        column-count: 3;
        column-gap: 20px;
        column-rule: 1px solid lightblue;
    }    
    .newspaper4 {
        column-count: 4;
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

# LB3: Bewegungsgesetze (Kinematik)

@uhr

![KinematikUndDynamik](https://www.online-wissensdatenbank.de/wp-content/uploads/2023/12/kinematik-grundlagen-der-bewegungslehre.jpg "Bild-Quelle: https://www.online-wissensdatenbank.de")

<details style="margin-left:10%">

<summary> Tablets 9a </summary>

![Tablets9a](https://diversewolken.ddns.net/nextcloud/index.php/s/K46eDTyd9EkFMSr/download)

</details>

<details style="margin-left:10%">

<summary> Tablets 9b </summary>

![Tablets9b](https://diversewolken.ddns.net/nextcloud/index.php/s/MiN3PTGWnDJRKWe/download)

</details>

<details style="margin-left:10%">

<summary> Tablets 9c </summary>

![Tablets9c](https://diversewolken.ddns.net/nextcloud/index.php/s/f9mzGsqKXPNzkFa/download)

</details>

## 3.1. Einführung in die Analyse von Bewegungen

Die __Kinematik__ (altgriechisch κίνημα kinema, deutsch ‚Bewegung‘) ist das Gebiet der Mechanik, in dem die Bewegung von Körpern rein geometrisch mit den Größen <bdi style="color:red">Ort, Zeit, Geschwindigkeit und Beschleunigung</bdi> beschrieben wird.

> Jeder Körper wird als eine @color(Punktmasse,red) betrachtet.

{{1}}
*******
__Formelzeichen..[Einheit]:__

<div style="text-indent:10%">

> $t$ .. Zeit $\Big[ s \Big]$
>
> $s, x$ .. Ort/Position/Koordinate des Körpers $\Big[ m \Big]$
>
> $v$ .. Geschwindigkeit des Körpers $\Big[ \dfrac{m}{s} \Big]$
> 
> $a$ ..Beschleunigung $\Big[ \dfrac{m}{s^2} \Big]$

</div>
*******

{{2}}
*******
__Abhängigkeiten:__ Um zu beschreiben, zu welcher Zeit sich ein Körper an welchem Ort aufhält, notiert man die Beziehung verschiedener kinematischer Größen folgender Art

_Beispiele:_

<div style="text-indent:10%">

> $s(t)$ ..  @color(_gesprochen: s von t_,blue) bedeutet: Der Körper befindet sich zum Zeitpunkt $t$ am Ort $s$
>
> $v(t)$ .. Der Körper besitzt zum Zeitpunkt $t$ die Geschwindigkeit $v$

</div>
*******

## 3. 2. Gleichförmige Bewegungen

[LEIFI-GleichförmigeBewegung_1](https://www.leifiphysik.de/mechanik/gleichfoermige-bewegung/grundwissen/gleichfoermige-bewegung)

{{1}}
***********
> __Definition__: Eine @color(gleichförmige Bewegung, red) liegt vor, wenn sich die Geschwindigkeit des Körpers nicht ändert.
>
> Beispiele: Förderbänder, Rolltreppen
***********

{{2}}
***********
__Aufgaben  (ca. 35 min):__

1. Erstelle eine Tabelle mit vier Spalten und zehn Zeilen.

2. Die erste Zeile lautet

| | | | |
| $t$ in s | <p style="color:purple">$s_1$ in m</p> | <p style="color:darkgreen">$s_2$ in m</p> | <p style="color:blue">$s_3$ in m</p> |

3. Übernimm die Messwerte aus der Simulation in deine Tabelle.

     [LEIFI-Link-Simulation-GleichförmigeBewegung](https://www.leifiphysik.de/mechanik/gleichfoermige-bewegung/grundwissen/geschwindigkeit-bei-gleichfoermiger-bewegung)


4. Zeichne ein @color(Zeit-Weg-Diagramm, orange) (mind. 5cm x 5 cm), mit der __Zeit t in s__ auf der x-Achse und der __Strecke s in m__ auf der y-Achse. Ergänze die Datenpunkte und verbinde sie als einen farbigen Graph.

5. Löse im Anschluss das Quiz zur gleichförmigen Bewegung auf dieser Seite.

     [Link-Quiz-GleichförmigeBewegung](https://www.leifiphysik.de/mechanik/gleichfoermige-bewegung/aufgabe/quiz-zum-zeit-weg-gesetz-der-gleichfoermigen-bewegung)

6. Schau dir die nächste Seite zur Darstellung von zusammen gesetzten Bewegungen an. Probiere die Lösungen.
***********

## Darstellung in Diagrammform

Häufig ist es __anschaulich__ die Bewegung eines Körpers in @color(Diagrammform, red) darzustellen.

<bdi style="color:red">
Vereinbahrung: In der Kinematik wird die Zeit __immer__ auf der x-Achse dargestellt.
</bdi>

Beispiel: s(t) Diagramm

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

## 3. 2. Gleichförmige Bewegungen


> __Definition__: Eine @color(gleichförmige Bewegung, red) liegt vor, wenn sich die Geschwindigkeit des Körpers nicht ändert.
>
> Beispiele: Förderbänder, Rolltreppen

![ErgebnisGleichförmigeBewegungen](https://diversewolken.ddns.net/nextcloud/index.php/s/WTeKrtEccdTL7C5/download)

{{1}}
***********
> Der Zeit-Weg-Graph ( $s(t)$-Graph) einer gleichförmigen Bewegung ist eine @color(Gerade, red).
>
> Je @color(steiler, red) die Gerade ansteigt, desto @color(größer, red) ist die Geschwindigkeit.
***********

## Bewegungsanalyse - Video

Bis 12:00

!?[Telekolleg_bis_13:40](https://diversewolken.ddns.net/nextcloud/index.php/s/QycTfGXXTDPn2aa/download)

### Übung zur zusammengesetzt gleichförmigen Bewegung

??[Geogebra_Autofahrt](https://www.geogebra.org/m/hdkrad92)

---

{{1}}
*************
??[Moodle_Übung_Zusammengesetzte_Gleichförmige_Bewegungen](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=562)
*************


## 3. 3. Geschwindigkeit
{{1}}
**********
> Definition: Wir definieren __Bewegung__ als Änderung des Ortes in einer bestimmten Zeit. Die __Geschwindigkeit__ gibt an, wie groß die Ortsänderung pro Zeiteinheit ist.
>
> Formelzeichen: $v$
>
> Einheit: $\hspace{1cm} \large{\Big[ \dfrac{m}{s} \Big] \hspace{1cm}\overset{\cdot 3,6}{\underset{:3,6}\rightleftarrows}  \hspace{1cm}\Big[ \dfrac{km}{h} \Big]}$
>
> Formel: $\hspace{1cm} \boxed{\large{v = \dfrac{\Delta s}{\Delta t}}}$
**********

---

{{2}}
**********
<p class="newspaper">
__Durchschnittsgeschwindigkeit $\bar{v}$__
<p class="cb">
__Momentangeschwindigkeit $v(t)$__
</p>
</p>
**********

{{3}}
**********
<p class="newspaper">
Die Durchschnittsgeschwindigkeit gibt einen @color(Mittelwert,red) der Geschwindigkeit über den betrachteten Zeitraum an.

{{5}}
******
> Die Durchschnittsgeschwindigkeit wird mit der Formel $v = \frac{\Delta s}{\Delta t}$ für beliebiges Zeitintervall $\Delta t$ (z.B. für die gesamte Fahrt) berechnet.
******
<p class="cb">
Momentangeschwindigkeit gibt die @color(__aktuelle__,red) Geschwindigkeit zu einem bestimmten Zeitpunkt t an.

{{6}}
******
> Die Momentangeschwindigkeit wird mit der Formel $v = \frac{\Delta s}{\Delta t}$ für ein sehr kleines Zeitintervall $\Delta t$ berechnet.
******
</p>
</p>
**********

{{4-5}}
**********
Ab: 11:00

!?[Telekolleg_bis_13:40](https://diversewolken.ddns.net/nextcloud/index.php/s/QycTfGXXTDPn2aa/download)
**********

### Übung: Eine realistische Autofahrt

{0-1}{![0](https://diversewolken.ddns.net/nextcloud/index.php/s/E3qZoZqZrAteJ8P/download)}

{1-2}{![1](https://diversewolken.ddns.net/nextcloud/index.php/s/kXtSMWDKiAJ2RQt/download)}

{2-3}{![2](https://diversewolken.ddns.net/nextcloud/index.php/s/NdBgcyXZfJnsxaz/download)}

{3-4}{![3](https://diversewolken.ddns.net/nextcloud/index.php/s/Py3SJjkc6sSTgkY/download)}

{4-5}{![4](https://diversewolken.ddns.net/nextcloud/index.php/s/XpMWtHsK2H8B7nR/download)}

{5-6}{![5](https://diversewolken.ddns.net/nextcloud/index.php/s/76zKEaeqPrMgA6K/download)}

{6-7}{![6](https://diversewolken.ddns.net/nextcloud/index.php/s/fc7mWYL4CXTqNAd/download)}

{7-8}{![7](https://diversewolken.ddns.net/nextcloud/index.php/s/tkMAS53nT4WDjKT/download)}

{8}{![8](https://diversewolken.ddns.net/nextcloud/index.php/s/7LXaxmwTBorb4cj/download)}

{{9}}
********
Link zum [Arbeitsblatt](https://diversewolken.ddns.net/nextcloud/index.php/s/S4zs3zybdcyf4Fx)

Löse die Aufgaben auf dem Arbeitsblatt. Vergleich deine Lösungen dann mit Moodle.

??[Moodle_EineRealistischeAutofahrt](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=557)

********

### Tägliche Übung zur Beschleunigung

[TÜ-Beschleunigung-PDF](https://diversewolken.ddns.net/nextcloud/index.php/s/aeGt4Bz9ZqT3kef/download)

oder

[PPT-Beschleunigung](https://gykl-my.sharepoint.com/:p:/g/personal/golnik_ch_gykl_onmicrosoft_com/EYV_CNu29v1Es0v6hxd5YLwBtw9lSEZsJ9Nh9pIE6mDl7A?e=RDmj0F)

## 3. 4. Beschleunigung
{{1}}
**********
> Definition: Die __Beschleunigung__ definieren wir als Änderung der Geschwindigkeit in einer bestimmten Zeit. <br> Die __Beschleunigung__ gibt an, um welchen Wert sich die Geschwindigkeit pro Sekunde ändert.
{{2}}
************
> Formelzeichen:   $\hspace{1cm}a$
> <br> <br>
> Einheit: $\hspace{1cm} \large{\Big[ \frac{\frac{m}{s}}{s} =\frac{m}{s^2} \Big]}$
> <br> <br>
>
> Formel: $\hspace{1cm} \boxed{\large{a = \dfrac{\Delta v}{\Delta t}}}$
************

**********

---

{{3}}
**********
<p class="newspaper">

__Beispiel 1:__ Auf dem Arbeitsblatt der letzten Stunde (Aufgabe 8) wurde gefragt: Um welchen Betrag ändert sich die Geschwindigkeit von Punkt 5->6 pro Sekunde, oder <br> @color(Wie groß ist die Beschleunigung?, red)

{{4}}
**********

__Lösung:__ Die Geschwindigkeit ändert sich in $25s$ von  $0\frac{m}{s} $ auf $12,56 \frac{m}{s}$. <br> Das heißt:

geg.:

<p style="margin-left:5%">

$\Delta t = 25 s$

$\Delta v = 12,56 \frac{m}{s}$

</p>

ges.: 

<p style="margin-left:5%">

$a_{5->6}$

</p>

**********


{{5}}
**********
Lösung: 

<p style="margin-left:5%">

$ a_{5->6} = \dfrac{\Delta v}{\Delta t} = \dfrac{12,56 \frac{m}{s}}{25 s}$

$a_{5->6}=0,5024 \frac{m}{s^2} \approx 0,5 \frac{m}{s^2}$

</p>

**********

<p class="cb">
{{3-6}}
*************
![8](https://diversewolken.ddns.net/nextcloud/index.php/s/7LXaxmwTBorb4cj/download)
*************

{{6}}
*************
__Beispiel 2__: Ermittle die Beschleunigung nach der ersten Ampel.

geg.:

<p style="margin-left:5%">

$\Delta t = ... s$

$\Delta v = ... \frac{m}{s}$

</p>

ges.: 

<p style="margin-left:5%">

$a_{1->2}$

</p>

<details>

<summary> Lsg.: </summary>

<p style="margin-left:5%">

$a_{1->2} = \dfrac{\Delta v}{\Delta t}$

Die Geschwindigkeit ändert sich von $0\frac{m}{s}$ auf $8,6\frac{m}{s}$. Die benötigte Zeit ist $5s$.

$a_{1->2} = \dfrac{8,6\frac{m}{s}}{5 s}$

$a_{1->2}\approx 1,72 \frac{m}{s^2}$

</p>

</details>
*************
</p>

</p>

**********

{{7}}
**********
---
<p style="color:blue">
__Aufgaben: __

- übernimm das Tafelbild

- berechne Beispiel 2

- löse bei Moodle die Aufgaben 10-13

[Moodle-EineRealistischeAutofahrt-10-bis-13](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=557)
</p>
**********

### Video: Alles immer schneller

Telekolleg_AllesImmerSchneller_Bis5:50

!?[Telekolleg_AllesImmerSchneller](https://diversewolken.ddns.net/nextcloud/index.php/s/2QFxN89dLeXtMdT/download)

#### KI: Unterschied zwischen Durchschnittsgeschwindigkeit und Momentangeschwindigkeit


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Generator-Aufgabe:__<br> Erkläre mit eigenen Worten den Unterschied zwischen der Durchschnittsgeschwindigkeit und der Momentangeschwindigkeit.

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten den Unterschied zwischen der Durchschnittsgeschwindigkeit und der Momentangeschwindigkeit. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist 9. Klasse. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
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


### Videoanalyse mit VIANA2

__Arbeitsablauf__

1. Besorge dir in deiner Gruppe ein Stahlkugel und ein großes Lineal.

2. Positioniere das Tablet auf dem Tisch so, dass das Lineal zu sehen ist und die Kugel entlange des Lineals rollen kann.

3. Öffne das Video-Analyse-Tool VIANA2 auf dem Tablet.

4. Wähle: Neues Projekt. Nimm mit dem Tablet die gleichförmige Bewegung der Kugel entlang des Lineals auf.

5. Ergänze in deiner Analyse den Maßstab und das Koordinatensystem

6. Lass dir das s(t)-Diagramm und das v(t)-Diagramm darstellen.

7. Zeige dein Ergebnis kurz dem Fachlehrer

8. Lass dir zwei Holzblocks geben und stelle diese unter deinen Tisch.

9. Wiederhole die Analyse mit einem neuen Projekt und einer __beschleunigten Bewegung__ der Kugel auf dem schrägen Tisch.

