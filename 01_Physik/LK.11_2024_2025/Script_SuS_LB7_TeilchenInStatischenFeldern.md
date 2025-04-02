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
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
}

.red {
    color: red;
}

.blue {
    color: blue;
}

.darkgreen {
    color: darkgreen;
}

.orange {
    color: orange;
}

.purple {
    color: purple;
}

@end

@color
<bdi style="color:@1">@0</bdi>
@end


@rangeQuiz2

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

@onload
window.LIA.settings.font_size = 2
@end

-->


# LB 7 - Geladene Teilchen in statischen elektrischen und magnetischen Feldern

{{1}}
**********
> Die Bewegung elektrisch geladener Teilchen beschreiben wir mit den Methoden der __Kinematik__ [@color(__LB 3__, red)] auf Basis der wirkenden Kräfte (__elektrische Kraft__ $F_{el}$ [@color(__LB 5__,red)] und __Lorentzkraft__ $F_L$ [@color(__LB 6__,red)]). Dabei betrachten wir die Teilchen als __Punktmassen__, welche den __Newton'schen Gesetzen__ [@color(__LB 2__, red)] folgen. __Energie__betrachtungen, z.B. zur kinetischen Energie, [@color(__LB 1__, red)] sind gültig. 
**********

![ProtonCollisionCern](https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg)

## 7.1. Geladene Teilchen im elektrischen Feld

<p class="newspaper">

__Bewegung im Längsfeld__

> Elektrische Kraft auf Teilchen (hier @color(Elektronen, darkgreen) ) wirkt __entlang der Bewegungsrichtung__

<p class="cb">

__Bewegung im Querfeld__

> Elektrische Kraft auf Teilchen (hier @color(Elektronen, darkgreen) ) wirkt __senkrecht zur Bewegungsrichtung__

</p>

</p>

---

<p class="newspaper">

__Elektronenkanone__

![Elektronenkanone](https://diversewolken.ddns.net/nextcloud/index.php/s/cC5JWAYmimFKmrC/download)

<p class="cb">

__Ablenkröhre__

![Ablenkröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/HaNg8rpJnyZj7F5/download)

</p>

</p>

### 7.1.1. Beschleunigung im Längsfeld - Elektronenkanone

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

3. 3. (_Optional_) Löse das Quiz.

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


### 7.1.2. Ablenkung Querfeld - Ablenkröhre

@timer(35, 00)

__Aufbau einer Elektronen-Ablenkröhre__

??[VirtuelleExperiment_ElektronenAblenkrhre](https://virtuelle-experimente.de/e-feld/hypothesen/versuchsaufbau.php "Quelle: Stefan Richtberg, https://virtuelle-experimente.de CC BY-NC-SA 3.0 DE")

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
>
> Die parabelförmige Bewegung ist eine __Superposition__ (Überlagerung) aus einer gleichförmigen Bewegung (in x-Richtung) und einer gleichmäßig beschleunigten Bewegung in (y-Richtung). Es gelten die __Bewegungsgleichungen__:

<p class="newspaper">

> $x(t) = v_{0x} \cdot t$ 
>
> $v_x(t) = v_{0x} $
>
> $a_x(t) = 0 $

<p class="cb">

> $y(t) = \frac{1}{2} \cdot a_y \cdot t^2$
>
> $v_y(t) =  a_y \cdot t$
> 
> $a_y(t) \overset{\mathrm{2.NG}}{=} \frac{F_{el}}{m} = \frac{E_{el}\cdot q}{m} = \frac{U_p \cdot q}{d \cdot m} $

</p>

</p>

</p>

2. Wechsle zu den _Übungen_ (oberes Menü) und bearbeite:

2. 1. Übung Fachbegriffe

2. 2. _Optional:_ Übung Anschluss

2. 3. Mulitple Choice kurze Version

2. 4. Abituraufgaben

      - Aufgabe 2

      - Aufgabe 5 (b, d)

</p>

#### KI-Aufgabe: Erkläre die Bewegung einer elektrischen Ladung im Längs- und im Querfeld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes: <br> 1. Wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld) <br> 2. Wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen.

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten die Bewegung einer elektrischen Ladung im Einfluss eines homogenen elektrischen Feldes: <br> 1. Wenn die Feldlinien in Bewegungsrichtung verlaufen (Längsfeld) <br> 2. Wenn die Feldlinien senkrecht zur Bewegungsrichtung verlaufen. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungskurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
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


## 7.1.3. Der Millikan-Versuch

_Tafelbildvideo zum Millikan-Versuch:_

!?[Millikan-Experiment](https://www.youtube.com/watch?v=XMfYHag7Liw)

<details>

<summary> __Fertiges Tafelbild zum Nachschlagen__ </summary>

![TB_Millikan](https://diversewolken.ddns.net/nextcloud/index.php/s/ocNCHdfqgfNNt44/download)

</details>

---

__Erklärung:__

Robert Millikan führte einen berühmten Versuch durch, um die Elementarladung $q_e$ zu bestimmen. Dabei wurden geladene Öltröpfchen in einem homogenen elektrischen Feld zwischen zwei Platten zum Schweben gebracht, indem sich die elektrische Kraft und die Gewichtskraft gegenseitig kompensieren. 

### IQB-Aufgabe Milikan-Versuch

1. __Aufgabenstellung:__  [Milikan-Aufgabenstellung](https://diversewolken.ddns.net/nextcloud/index.php/s/EzY4gat6pjTXD7b)

2. __Hilfestellung:__ [Milikan-Hilfestellung](https://diversewolken.ddns.net/nextcloud/index.php/s/cizYee289ftPDQi)

3. __Zusätzliches Material:__ [Milikan-Material](https://diversewolken.ddns.net/nextcloud/index.php/s/dAa869L72S2dLzo)

#### KI-Aufgabe: Erkläre den Milikan-Versuch


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung-EFeld-Aufgabe:__<br> Erkläre mit eigenen Worten den Milikan-Versuch <br> 1. Erkläre das Ziel, mit welchem der Versuch durchgeführt wurde. <br> 2. Erkläre den Versuchsaufbau <br> 3. Beschreibe, was bei den Messungen als Ergebnisse heraus gekommen sind. <br> 4. Erkläre, wie man die Ergebnisse interpretieren konnte.

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkläre mit eigenen Worten den Milikan-Versuch <br> 1. Erkläre das Ziel, mit welchem der Versuch durchgeführt wurde. <br> 2. Erkläre den Versuchsaufbau <br> 3. Beschreibe, was bei den Messungen als Ergebnisse heraus gekommen sind. <br> 4. Erkläre, wie man die Ergebnisse interpretieren konnte. <br> Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungskurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
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
