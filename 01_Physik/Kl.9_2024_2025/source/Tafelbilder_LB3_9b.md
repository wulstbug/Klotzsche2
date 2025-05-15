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

# LB3: Bewegungsgesetze (Kinematik) - 9b

@uhr

![KinematikUndDynamik](https://www.online-wissensdatenbank.de/wp-content/uploads/2023/12/kinematik-grundlagen-der-bewegungslehre.jpg "Bild-Quelle: https://www.online-wissensdatenbank.de")

## 3.1. Einführung in die Analyse von Bewegungen

## 3. 2. Gleichförmige Bewegungen

[LEIFI-GleichförmigeBewegung_1](https://www.leifiphysik.de/mechanik/gleichfoermige-bewegung/grundwissen/gleichfoermige-bewegung)

__Aufgaben:__

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


### Übung zur zusammengesetzt gleichförmigen Bewegung

??[Moodle_Übung_Zusammengesetzte_Gleichförmige_Bewegungen](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=561)

## 3. 3. Geschwindigkeit

[Geogebra_Autofahrt](https://www.geogebra.org/m/hdkrad92)

### Übung: Eine realistische Autofahrt

![8](https://diversewolken.ddns.net/nextcloud/index.php/s/7LXaxmwTBorb4cj/download)

Link zum [Arbeitsblatt](https://diversewolken.ddns.net/nextcloud/index.php/s/S4zs3zybdcyf4Fx)

Löse die Aufgaben auf dem Arbeitsblatt. Vergleich deine Lösungen dann mit den Aufgaben bei Moodle.

[Moodle_EineRealistischeAutofahrt](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=557)


## 3. 4. Beschleunigung

<p class="newspaper">

__Beispiel 1:__ Auf dem Arbeitsblatt der letzten Stunde (Aufgabe 8) wurde gefragt: Um welchen Betrag ändert sich die Geschwindigkeit von Punkt 5->6 pro Sekunde, oder <br> @color(Wie groß ist die Beschleunigung?, red)

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

Lösung: 

<p style="margin-left:5%">

$ a_{5->6} = \dfrac{\Delta v}{\Delta t} = \dfrac{12,56 \frac{m}{s}}{25 s}$

$a_{5->6}=0,5024 \frac{m}{s^2} \approx 0,5 \frac{m}{s^2}$

</p>



<p class="cb">

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

</p>

<br>

</p>

---

<p style="color:blue">
__Aufgaben: __

- übernimm das Tafelbild

- berechne Beispiel 2

- löse bei Moodle die Aufgaben 10-13

- [Moodle-EineRealistischeAutofahrt-10-bis-13](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=557)
</p>

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


#### KI-Aufgaben: Erkläre Begriffe der Bewegungsgesetze

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

---

> __1. Geschwindigkeit-Aufgabe:__<br> Erkläre mit eigenen Worten den Unterschied zwischen der Durchschnittsgeschwindigkeit und der Momentangeschwindigkeit.

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

#### KI-Aufgaben 2: Erkläre Begriffe der Bewegungsgesetze

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

---

> __2. Beschleunigung:__<br> Erkläre mit eigenen Worten den Beschleunigung.

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten den Begriff Beschleunigung. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist 9. Klasse. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
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

### Übungsaufgaben zur Vorbereitung LK bei Moodle

> Einige Aufgaben sind immer doppelt, bitte abwechselnd lösen

[Übungen zur LK](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=564)


#### KI-Aufgabe: Fragen zu den Bewegungsgesetzen

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Fragen.
</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

---

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich werde dir jetzt 5 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10.
    1. Beschreibe den Begriff Bewegung oder anders ausgedrückt, definiere Bewegung.
    2. Beschreibe den Begriff Geschwindigkeit oder anders ausgedrückt, definiere Geschwindigkeit.
    3. Beschreibe, was eine gleichförmige Bewegung charakterisiert.
    4. Beschreibe den Unterschied zwischen Durchschnittsgeschwindigkeit und Momentangeschwindigkeit.
    5. Beschreibe den Begriff Beschleunigung oder anders ausgedrückt, definiere Beschleunigung.
    Alle Fragen sind im Fach Physik im Niveau der 9. Klasse zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.</span>
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


## 3.7. Bewegungsgleichungen s(t) und v(t)

<p class="newspaper3">

@color(__Stillstand__, orange)

<br> <br>

| ![Stillstand_s](https://diversewolken.ddns.net/nextcloud/index.php/s/oZ3XsqSB3GRHsKD/download) | ![Still_v](https://diversewolken.ddns.net/nextcloud/index.php/s/rBGtSm48JYBGL7P/download) |

<br> <br>

$ \boxed{s(t) = s_0}$

$ \boxed{v(t) = 0 } $

mit:

<p style="margin-left:5%">

$s_0$ .. Anfangsweg

$v = 0 $

$ a = 0 $ 

</p>

<p class="cb">

@color(__gleichförmige Bewegung__, blue)

<br> <br>

| ![Stillstand_s](https://diversewolken.ddns.net/nextcloud/index.php/s/jTEtobWNAZmejEb/download) | ![Still_v](https://diversewolken.ddns.net/nextcloud/index.php/s/CXZSMBojQ94ZmH9/download) |

<br> <br>

$ \boxed{s(t) = v_0 \cdot t + s_0}$

$ \boxed{v(t) = v_0} $

mit:

<p style="margin-left:5%">

$s_0$ .. Anfangsweg

$v_0$ .. Anfangsgeschwindigkeit

$ a = 0 $ 

</p>

<p class="cb">

@color(__gleichmäßig beschleunigte Bewegung__, green)

<br> <br>

| ![Beschl_s](https://diversewolken.ddns.net/nextcloud/index.php/s/aWLGbejN8i9Rzgj/download) | ![Beschl_v](https://diversewolken.ddns.net/nextcloud/index.php/s/FfS76JwYLYcJYtR/download) |

<br> <br>

$ \boxed{s(t) = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t + s_0}$

$ \boxed{v(t) = a \cdot t + v_0} $

mit:

<p style="margin-left:5%">

     $s_0$ .. Anfangsweg

     $v_0$ .. Anfangsgeschwindigkeit

     $a$ .. Beschleunigung

</p>

</p>

</p>

</p>

### Beispielaufgaben zu den Bewegungsgleichungen

<p class="newspaper">

__Beispiel 1:__

Ein Fahrzeug beschleunigt mit 5 m/s² für 5 s. Ermittle die Geschwindigkeit und den zurück gelegten Weg.

__geg.:__

<p style="margin-left:5%">

$a =  5 \frac{m}{s^2}$

$t = 5 s$

$ v_0 = 0$

$s_0 = 0$

</p>

__ges.:__

<p style="margin-left:5%">

s, v

</p>

__Lsg.:__

<p style="margin-left:5%">

$ s = \frac{1}{2} \cdot a \cdot t^2$

$ v = a \cdot t$

<details>

<summary> Lösung </summary>

$s = 62,5 m$

$v = 25 \frac{m}{s}$

</details>

</p>

<p class="cb">

__Beispiel 2:__

Ein Fahrzeug fährt auf eine Autobahn. Es fährt auf den Beschleunigungsstreifen mit einer Geschwindigkeit von 36 km/h. Dann beschleunigt es innerhalb von 10s auf 144 km/h. Ermittle die Beschleunigung und den zurück gelegten Weg.

__geg.:__

<p style="margin-left:5%">

$v_{anf} = 36 \frac{km}{h} = 10 \frac{m}{s}$

$v_{end} = 144 \frac{km}{h} = 40 \frac{m}{s}$

$\Delta v = v_{end} - v_{anf} = 30 \frac{m}{s}$

$t = 10 s$

$s_0 = 0$

</p>

__ges.:__

<p style="margin-left:5%">

s, a

</p>

__Lsg.:__

<p style="margin-left:5%">

<details>

<summary> Lösungsweg </summary>

$ a = \frac{\Delta v}{\Delta t} = \frac{30 \frac{m}{s}}{10 s}= 3 \frac{m}{s^2}$

$ s = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t$

$ s = \frac{1}{2} \cdot 3 \frac{m}{s^2} \cdot (10s)^2 + 10\frac{m}{s} \cdot 10 s$

</details>

<details>

<summary> Lösung </summary>

$s = 250 m$

</details>

</p>

</p>

</p>


### KI-Aufgabe Beschleunigte Bewegung

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Fragen.
</p>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

---

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich möchte, dass du dir eine Rechen-Aufgabe für mich ausdenkst, mich dann danach fragst und meine Antwort überprüfst. Die Aufgabe soll im Bereich Physik der 9. Klasse Bewegungsgesetze sein. Erfinde eine zufällige Beschleunigung und frage mich nach der Geschwindigkeit, die der Körper nach einer bestimmten Zeit erreicht hat. Wenn ich die Frage richtig beantwortet habe, stelle mir eine Folgefrage, welche ebenfalls eine Berechnung erfordert und an die vorherige Frage angelehnt ist. Der Schwierigkeitsgrad der Fragen soll steigen. Wenn ich diese Frage beantwortet habe, dann gib mir eine Folge-Aufgabe. Gib mir nicht die Lösungen oder Tipps, wenn ich nicht darum bitte. <br> Wenn ich die Frage nicht richtig beantwortet habe, frage mich, ob ich es nochmal versuchen will oder einen Tipp möchte. Frage mich nach der dritten Frage, ob ich eine Bewertung auf einer Skala von 0 bis 10 meiner gesamten Antworten möchte. Wenn ich einwillige, dann bewerte meine Antworten auf einer Skala von 0 bis 10.</span>
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


### Übungsaufgaben zu den Bewegungsgleichungen

1. Der neue Golf ID3 beschleunigt von 0 km/h auf 100 km/h in 8,9s. Ermittle die Beschleunigung und die Strecke, die er für diese Beschleunigung benötigt.

<p style ="margin-left:5%">

@rangeQuiz2($a$, 3.12 ,$\frac{m}{s^2}$)

@rangeQuiz2($s$, 123.619 ,$m$)

</p>

2. Ein Schlitten fährt einen Hang hinunter. Der Hang ist 50m lang. Der Schlitten hat eine gleichmäßige Beschleunigung von 0,5 m/s². Ermittle die Zeit, die der Schlitten den Hang hinunter braucht und ermittle die Endgeschwindigkeit.

<p style ="margin-left:5%">

@rangeQuiz2($t$, 14.14 ,$s$)

@rangeQuiz2($v$, 7.07 ,$\frac{m}{s}$)

</p>

3. Ein Fahrzeug steht an einer Ampel. Als die Ampel auf grün schaltet fährt es mit einer Beschleunigung von 2 m/s² los. Im Moment des Losfahrens überholt ein zweites Auto auf der zweiten Spur mit einer Geschwindigkeit von 50 km/h. Es bewegt sich gleichförmig. Ermittle den Überhol-Zeitpunkt, die Strecke, an welchem das erste Auto, das zweite Auto überholt und die Überholgeschwindigkeit (in km/h).

<p style ="margin-left:5%">

@rangeQuiz2($t$, 13.89 ,$s$)

@rangeQuiz2($s$, 192.917 ,$m$)

@rangeQuiz2($v$, 100 ,$\frac{km}{h}$)

</p>


## 3.8. Analyse in v(t)-Diagrammen

<p class="newspaper">

{1}{__Beschleunigung a aus dem v(t)-Diagramm ermitteln__}

{{3}}
********
> Die Beschleunigung entspricht in einem v(t)-Diagramm dem @color(Anstieg des Graphen, red).

__Merke:__ Der Anstieg eines Graphen kann mit dem @color(Anstiegsdreieck,red) ermittelt werden.

********

<p class="cb">

{2}{__Zurückgelegten Weg s aus dem v(t)-Diagramm ermitteln__}

{{5}}
********
> Der zurückgelegte Weg entspricht in einem v(t)-Diagramm dem @color(Flächeninhalt unter dem Graphen, red).

__Merke:__ Der Flächeninhalt unter dem Graph kann durch geometrische Berechnung ermittelt werden.
********

</p>

</p>

---

<p class="newspaper">

{{4}}
********
__Anstieg (allgemein):__ $\boxed{m = \dfrac{\Delta y}{\Delta x}}$

![Bild-Diagramm-x-y](https://diversewolken.ddns.net/nextcloud/index.php/s/2aRa2oZLNKQfdAg/download)
********

<p class="cb">

{{6}}
********
__Beispiel 1:__ @color(Gleichförmige Bewegung, blue)

Fläche unter dem Graph ist ein Rechteck.

![Bild-Diagramm-gleichf](https://diversewolken.ddns.net/nextcloud/index.php/s/Fp8yMpQgYN7ep7F/download)
********

</p>

</p>

---

<p class="newspaper">

{{4}}
********
__Anstieg in v(t):__ $\boxed{a = \dfrac{\Delta v}{\Delta t}}$

![Bild-Diagramm-v-t](https://diversewolken.ddns.net/nextcloud/index.php/s/rsEJwBZknbyfGN2/download)
********

<p class="cb">
{{6}}
********
__Beispiel 2:__ @color(Gleichmäßige Beschleunigung, blue)

Fläche unter dem Graph ist ein rechtwinkliges Dreieck.

![Bild-Diagramm-gleichmBeschl](https://diversewolken.ddns.net/nextcloud/index.php/s/95wwXeFTf9omXGb/download)
********

</p>

</p>

---

### Übungsaufgabe 1 (zu v(t)-Diagrammen)

![Übungsaufgabe](https://diversewolken.ddns.net/nextcloud/index.php/s/JEPGoaMHYYzbLyR/download)

(+) Bestimme zu jedem Abschnitt 

- a) die Art der Bewegung

- b) die Beschleunigung

- c) den zurückgelegten Weg


##### Lösungen a) Art der Bewegung

__A-B__

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [(X)] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung
    [( )] gleichmäßig gebremste Bewegung

__B-C__

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [( )] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung
    [(X)] gleichmäßig gebremste Bewegung

__C-D__

    <!-- data-solution-button="off" -->
    [(X)] Stillstand
    [( )] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung
    [( )] gleichmäßig gebremste Bewegung

__D-E__

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [( )] gleichförmige Bewegung
    [(X)] gleichmäßig beschleunigte Bewegung
    [( )] gleichmäßig gebremste Bewegung

__E-F__

    <!-- data-solution-button="off" -->
    [( )] Stillstand
    [(X)] gleichförmige Bewegung
    [( )] gleichmäßig beschleunigte Bewegung
    [( )] gleichmäßig gebremste Bewegung

##### Lösungen b) Beschleunigung

__A-B__

<!-- data-solution-button="off" -->
$a$ = [[ 0 ]] $\frac{m}{s^2}$

<details style="margin-left:5%">

<summary> Lösung </summary>

Anstieg ist Null, d.h. $\Delta v=0$, d.h. a = 0.

</details>

---

__B-C__

<!-- data-solution-button="off" -->
$a$ = [[ -6 ]] $\frac{m}{s^2}$

<details style="margin-left:5%">

<summary> Lösung </summary>

Geschwindigkeit ändert sich von 60 $\frac{m}{s}$ auf 0 $\frac{m}{s}$. D.h. $\Delta v=v_{end}-v_{anf}=0\frac{m}{s}-60\frac{m}{s}=60\frac{m}{s}$. Die benötigte Zeit ist $\Delta t=10s$. Die Beschleunigung ist laut Formel:

$ a=\frac{\Delta v}{\Delta t}=\frac{-60\frac{m}{s}}{10s}=-6 \frac{m}{s^2} $

</details>

---

__C-D__

<!-- data-solution-button="off" -->
$a$ = [[ 0 ]] $\frac{m}{s^2}$

<details style="margin-left:5%">

<summary> Lösung </summary>

Anstieg ist Null, d.h. $\Delta v=0$, d.h. a = 0.

</details>


---

__D-E__

<!-- data-solution-button="off" -->
$a$ = [[ 0,5 ]] $\frac{m}{s^2}$

<details style="margin-left:5%">

<summary> Lösung </summary>

Geschwindigkeit ändert sich von $0 \frac{m}{s}$ auf $10 \frac{m}{s}$. D.h. $\Delta v=v_{end}-v_{anf}=10\frac{m}{s}-0\frac{m}{s}=10\frac{m}{s}$. Die benötigte Zeit ist $\Delta t=20s$. Die Beschleunigung ist laut Formel:

$ a=\frac{\Delta v}{\Delta t}=\frac{10\frac{m}{s}}{20s}=0,5 \frac{m}{s^2} $

</details>

---

__E-F__

<!-- data-solution-button="off" -->
$a$ = [[ 0 ]] $\frac{m}{s^2}$

<details style="margin-left:5%">

<summary> Lösung </summary>

Anstieg ist Null, d.h. $\Delta v=0$, d.h. a = 0.

</details>

##### Lösungen c) Zurückgelegter Weg

__A-B__

<!-- data-solution-button="off" -->
$s$ = [[ 600 ]] $m$

<details style="margin-left:5%">

<summary> Lösung </summary>

Der zurückgelegte Weg ist der Flächeninhalt zwischen dem Graph und der x-Achse. Hier ist es ein Rechteck. Es hat die Seiten $60\frac{m}{s}$ und $10s$. Der Flächeninhalt beträgt 

$s = 60\frac{m}{s} \cdot 10s = 600m$

</details>

---

__B-C__

<!-- data-solution-button="off" -->
$s$ = [[ 300 ]] $m$

<details style="margin-left:5%">

<summary> Lösung </summary>

Der zurückgelegte Weg ist der Flächeninhalt zwischen dem Graph und der x-Achse. Hier ist es ein rechtwinkliges Dreieck. Es hat die Schenkel $60\frac{m}{s}$ und $10s$. Der Flächeninhalt beträgt 

$s = \frac{1}{2} \cdot 60\frac{m}{s} \cdot 10s = 300m$

</details>

---

__C-D__

<!-- data-solution-button="off" -->
$s$ = [[ 0 ]] $m$


<details style="margin-left:5%">

<summary> Lösung </summary>

Der Flächeninhalt zwischen Graph und x-Achse ist Null. Daher legt der Körper keinen Weg zurück.

$s=0m$

</details>

---

__D-E__

<!-- data-solution-button="off" -->
$s$ = [[ 100 ]] $m$


<details style="margin-left:5%">

<summary> Lösung </summary>

Der zurückgelegte Weg ist der Flächeninhalt zwischen dem Graph und der x-Achse. Hier ist es ein rechtwinkliges Dreieck. Es hat die Schenkel $10\frac{m}{s}$ und $20s$. Der Flächeninhalt beträgt 

$s = \frac{1}{2} \cdot 10\frac{m}{s} \cdot 20s = 100m$

</details>

---

__E-F__

<!-- data-solution-button="off" -->
$s$ = [[ 200 ]] $m$

<details style="margin-left:5%">

<summary> Lösung </summary>

Der zurückgelegte Weg ist der Flächeninhalt zwischen dem Graph und der x-Achse. Hier ist es ein Rechteck. Es hat die Seiten $10\frac{m}{s}$ und $20s$. Der Flächeninhalt beträgt 

$s = 10\frac{m}{s} \cdot 20s = 200m$

</details>

### Übungsaufgabe 2: Zu den  Bewegungsgleichungen (3.7)

2. 1. (+) Ein Vater spielt mit seinem Kind _Rennen um die Wette_. Das Ziel ist ein Baum und befindet sich in 30m Entfernung. Das Kind hat, wenn es rennt eine Geschwindigkeit von $2\frac{m}{s}$. Der Vater hat eine Geschwindigkeit von $6 \frac{m}{s}$. Damit das Rennen fair ist, gibt der Vater dem Kind $10s$ Vorsprung. Ermittle, wer das Ziel als erster erreicht. Begründe deine Aussage durch Berechnung.

<details style ="margin-left:5%">

<summary> Lösung </summary>

Beide erreichen das Ziel gleichzeitig.

</details>

<details style ="margin-left:5%">

<summary> Begründung </summary>

Das Kind rennt in den ersten $10s$ seines Vorsprungs genau 20m. Für die restlichen 10m benötigt es weitere 5s. Der Vater rennt nach 10s los und benötigt für die gesamten 30m ebenfalls 5s. Sie erreichen das Ziel gleichzeitig.

</details>

---

2. 2. (+) Ein ICE beschleunigt gleichmäßig mit einer Beschleunigung von $2\frac{m}{s^2}$. Ermittle die Beschleunigungszeit und die Beschleunigungsstrecke, wenn der Zug eine End-Geschwindigkeit von 180 km/h erreichen soll.

<p style ="margin-left:5%">

@rangeQuiz2($t$, 25 ,$s$)

@rangeQuiz2($s$, 625 ,$m$)

</p>


<details style ="margin-left:5%">

<summary> Lösungshinweis: </summary>

Stelle für den ICE die Bewegungsgleichung s(t) und v(t) für eine gleichmäßig beschleunigte Bewegung auf (siehe _3.7 Bewegungsgleichungen_). Um die Beschleunigungszeit zu bestimmen kannst du v(t) nutzen. Achte auf die Umrechnung in $m/s$.

</details>

<details style ="margin-left:5%">

<summary> Lösungsweg </summary>

Die Bewegungsgleichungen für eine gleichmäßig beschleunigte Bewegung lauten (keine Anfangsgeschwindigkeit $v_0$, kein Anfangsweg $s_0$):

> $s(t) = \frac{1}{2} \cdot a \cdot t^2$
>
> $v(t) = a \cdot t$

Da der ICE von 0 auf 180km/h (50m/s) beschleunigt, kann man mit der Gleichung v(t)=50m/s die Beschleunigungszeit ausrechnen

> $50 \frac{m}{s} = 2 \frac{m}{s^2} \cdot t$
>
> => $\underline{t = 25 s}$

Jetzt kann man diese Zeit in die erste Gleichung s(t) einsetzen und erhält als Gesamtstrecke $s= \frac{1}{2} \cdot 2\frac{m}{s^2} \cdot (25s)^2 = 625m$.

> => $s=625 m$

</details>

---

### Übungsaufgabe 3: Zurückgelegter Weg (3.8)

> 3. (++) Zu einer geradlinigen Bewegung gehört das Zeit-Geschwindigkeits-Diagramm der folgenden Abbildung: <br> ![v-t-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/8PB92pbssc5MoMo/download)<!-- style="max-width:80%"-->

> 3. 1. Berechnen Sie die Beschleunigungen in den drei Zeitintervallen.

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

> 3. 2. Berechnen Sie die Teilwege ($s_1,\, s_2,\, s_3$), sowie den Gesamtweg.

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

### Übungsaufgabe 4 zu den Bewegungsgleichungen (3.7)

4. 1. (++) Ein Fahrzeug fährt auf der Autobahn mit einer Geschwindigkeit von 144 km/h. Plötzlich erkennt der Fahrer 200m vor ihm ein stehendes Fahrzeug und er tritt sofort auf die Bremse. Dabei kann das Fahrzeug mit einer Beschleunigung von $-5\frac{m}{s^2}$ gleichmäßg bremsen. Zeige durch Berechnung, ob es zu einem Aufprall kommt oder nicht.

<p style ="margin-left:5%">

<!-- data-solution-button="off" -->
- [( )] Ja
- [(x)] Nein

</p>


<details style ="margin-left:5%">

<summary> Lösungshinweis: </summary>

Stelle für das Fahrzeug die Bewegungsgleichung s(t) und v(t) für eine gleichmäßig beschleunigte Bewegung mit Anfangsgeschwindigkeit $v_0$ auf (siehe _3.7 Bewegungsgleichungen_). Um die Beschleunigungszeit zu bestimmen kannst du v(t) nutzen. Überprüfe anschließend, ob die benötigte Strecke größer oder kleiner als 200m ist. Achte auf die Umrechnung in $m/s$.

</details>

<details style ="margin-left:5%">

<summary> Lösungsweg </summary>

Die Bewegungsgleichungen für eine gleichmäßig beschleunigte Bewegung lauten (mit Anfangsgeschwindigkeit $v_0$, kein Anfangsweg $s_0$):

> $s(t) = \frac{1}{2} \cdot a \cdot t^2 + v_0 \cdot t$
>
> $v(t) = a \cdot t + v_0$

Das Fahrzeug hat eine Anfangsgeschwindigkeit $v_0 = 144 \frac{km}{h} \overset{:3,6}{=} 40 \frac{m}{s}$. Die Endgeschwindigkeit ist Null. Man kann für die zweite Gleichung noch die Beschleunigung nutzen und damit die Bremszeit ausrechnen.

> $0 \frac{m}{s} = -5 \frac{m}{s^2} \cdot t + 40 \frac{m}{s}$
>
> => $\underline{t = 8 s}$

Jetzt kann man diese Zeit in die erste Gleichung s(t) einsetzen und erhält als Gesamtstrecke $s=\frac{1}{2} \cdot -5\frac{m}{s^2} \cdot (8s)^2 + 40 \frac{m}{s} \cdot 8s = 160 m$.

Der Bremsweg genügt, um eine Kollision zu verhindern.

</details>

---

4. 2. (+++) Ein Fahrzeug (A) steht an einer Ampel. Als die Ampel auf grün schaltet fährt es mit einer Beschleunigung von 1,5 m/s² los. Im Moment des Losfahrens überholt ein zweites Auto (B) auf der zweiten Spur mit einer Geschwindigkeit von 80 km/h. Es bewegt sich gleichförmig. Ermittle den Überhol-Zeitpunkt, die Strecke, an welchem das erste Auto, das zweite Auto überholt und die Überholgeschwindigkeit (in km/h).

<p style ="margin-left:5%">

@rangeQuiz2($t$, 29.63 ,$s$)

@rangeQuiz2($s$, 658.3786 ,$m$)

@rangeQuiz2($v_A$, 160 ,$\frac{km}{h}$)

</p>

<details style ="margin-left:5%">

<summary> Lösungshinweis: </summary>

Stelle für beide Fahrzeuge die Bewegungsgleichung $s_A(t)$ (Auto A) und $s_B(t)$ (Auto B) auf (siehe _3.7 Bewegungsgleichungen_). Wenn sich die Fahrzeuge überholen, dann haben sie in diesem Moment die gleiche Strecke zurückgelegt. Das heißt, du kannst die beiden Gleichungen gleich setzen um die Überholzeit zu ermitteln. 

</details>

<details style ="margin-left:5%">

<summary> Lösungsweg </summary>

<p class="newspaper">

Für das erste Auto (A) gilt die Bewegungsgleichung (siehe _3.7 Beschleunigte Bewegung_):

> $ s_A(t) = \frac{1}{2} \cdot a_A \cdot t^2$

-> Hierbei ist $a_A=1,5\frac{m}{s^2}$.

<p class="cb">

Für das zweite Auto (B) gilt die Bewegungsgleichung (siehe _3.7 Gleichförmige Bewegung_):

> $ s_B(t) = v_{0B} \cdot t$

-> Hierbei ist $v_{0B} = \frac{80}{3,6} \frac{m}{s} = 22,22 \frac{m}{s}$.

</p>

</p>

Um den Überholzeitpunkt auszurechnen muss man $s_A(t) = s_B(t)$ setzen.

> $$ \frac{1}{2} \cdot a_A \cdot t^2 = v_{0B} \cdot t $$

Als Lösung ergibt sich zum einen $t=0$ (das ist an der Ampel) und dann 

> $$ t = \frac{2\cdot v_{0B}}{a_A} = \frac{2\cdot 22,22 \frac{m}{s}}{1,5s} $$
>
> $$ \underline{t = 29,63s} $$

Der zurückgelegte Weg kann dann mit $s_A(t)$ oder $s_B(t)$ berechnet werden

> $$ \underline{s_B(t=29.63s) = 658,38 m}$$

Die Geschwindigkeit des Fahrzeugs A berechnet sich mit $v_A = a_A \cdot t$ zu

> $$ \underline{v_A = 1,5\frac{m}{s^2} \cdot 29,63s = 44,44 \frac{m}{s} \overset{\cdot 3,6}{=} 160 \frac{km}{h}} $$

</details>


### Übungsaufgabe 5 Zuordnung Graphen

<p class="newspaper">

(+++) Gegeben sind folgende v(t)-Graphen für 7 verschiedene Fälle.

![Faelle_vt](https://diversewolken.ddns.net/nextcloud/index.php/s/L8Y8XrqrZpBX6Tt/download)

<p class="cb">

Ordne im folgenden Bild die x(t) Fälle den v(t) Fällen zu.

<iframe src="https://learningapps.org/watch?v=pd58g8qzt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

</p>

</p>
