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

# LB3: Bewegungsgesetze (Kinematik) - 9a

@uhr

![KinematikUndDynamik](https://www.online-wissensdatenbank.de/wp-content/uploads/2023/12/kinematik-grundlagen-der-bewegungslehre.jpg "Bild-Quelle: https://www.online-wissensdatenbank.de")

## 3.1. Einführung in die Analyse von Bewegungen

## 3. 2. Gleichförmige Bewegungen

[LEIFI-GleichförmigeBewegung_1](https://www.leifiphysik.de/mechanik/gleichfoermige-bewegung/grundwissen/gleichfoermige-bewegung)

{{2}}
***********
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

### Übung zur zusammengesetzt gleichförmigen Bewegung

[Moodle_Übung_Zusammengesetzte_Gleichförmige_Bewegungen](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=562)


## 3. 3. Geschwindigkeit

[Geogebra_Autofahrt](https://www.geogebra.org/m/hdkrad92)

### Übung: Eine realistische Autofahrt

![8](https://diversewolken.ddns.net/nextcloud/index.php/s/7LXaxmwTBorb4cj/download)

Link zum [Arbeitsblatt](https://diversewolken.ddns.net/nextcloud/index.php/s/S4zs3zybdcyf4Fx)

Löse die Aufgaben auf dem Arbeitsblatt. Vergleich deine Lösungen dann mit den Aufgaben bei Moodle.

[Moodle_EineRealistischeAutofahrt_2](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=558)

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

- [Moodle-EineRealistischeAutofahrt-10-bis-13](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=559)
</p>


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
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten den Beschleunigung. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist 9. Klasse. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
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


## 3. 5. Gleichförmige und beschleunigte Bewegung in Diagrammen darstellen

### Übungsaufgaben zur Vorbereitung LK bei Moodle

> Einige Aufgaben sind immer doppelt, bitte abwechselnd lösen

[Übungen zur LK](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=567)


### KI-Aufgabe: Fragen zu den Bewegungsgesetzen

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
    <span class="text-box" id="textToCopy2">Ich werde dir jetzt 5 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10. Frage mich jedes mal, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln möchte.
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

## 3.6. Bewegungsgleichungen s(t) und v(t)

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

$ s = \frac{1}{2} \cdot 3 \frac{m}{s^2} \cdot 10s^2 + 10\frac{m}{s} \cdot 10 s$

</details>

<details>

<summary> Lösung </summary>

$s = 250 m$

</details>

</p>

</p>

</p>



### Übungsaufgaben zu den Bewegungsgleichungen

1. Der neue Golf ID3 beschleunigt von 0 km/h auf 100 km/h in 8,9s. Ermittle die Beschleunigung und die Strecke, die er für diese Beschleunigung benötigt.

<p style ="margin-left:5%">

@rangeQuiz2($a$, 3.12 ,$s$)

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