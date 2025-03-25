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

</p>

2. Wechsle zu den _Übungen_ (oberes Menü) und bearbeite:

2. 1. Übung Fachbegriffe

2. 2. _Optional:_ Übung Anschluss

2. 3. Mulitple Choice kurze Version

2. 4. Abituraufgaben

      - Aufgabe 2

      - Aufgabe 5 (a, b, d)

</p>

