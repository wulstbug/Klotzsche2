<!--
author: Christian Golnik

language: de

logo: https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg

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

### IQB-Aufgabe Milikan-Versuch

1. __Aufgabenstellung:__  [Milikan-Aufgabenstellung](https://diversewolken.ddns.net/nextcloud/index.php/s/EzY4gat6pjTXD7b/download)

2. __Hilfestellung:__ [Milikan-Hilfestellung](https://diversewolken.ddns.net/nextcloud/index.php/s/cizYee289ftPDQi/download)

3. __Zusätzliches Material:__ [Milikan-Material](https://diversewolken.ddns.net/nextcloud/index.php/s/dAa869L72S2dLzo/download)

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


## 7. 2. Geschwindigkeitsfilter für geladene Teilchen - E-B-Kombination

### Übungsaufgabe Querfeldablenkung - E-B-Kombination

![Nr262_ElektronenbahnImElektrischenFeld.png](https://diversewolken.ddns.net/nextcloud/index.php/s/MMoMF6oKAeALQHs/download) Aus einer Elektronenquelle treten die Elektronen mit einer Geschwindigkeit $v_0$ senkrecht in das homogene elektrische Feld eines
Plattenkondensators der Breite 8,0 cm und der
Länge 10,0 cm ein. An den Plattenkondensator wird eine Spannung
von 12 kV angelegt.

2. 1. __Partnerübung*:__ Nennen Sie die Art der Flugbahn der Elektronen. Leiten Sie eine Gleichung für die Elektronenbahn im Feld her.

<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösungfindung__ </summary>

Auf die Elektronen wirkt die elektrische Kraft immer senkrecht zur den Kondensatorplatten, hier senkrecht nach oben. Das elektrische Feld ist homogen, demzufolge ist die elektrische Kraft konstant.

Dieser Effekt ist ähnlich dem horizontalen Wurf eines Körpers (nur nach oben statt nach unten). 

</details>

<details style="margin-left:10%">

<summary> __Hinweise zur Bahnform__ </summary>

In horizontaler Richtung (x-Richtung) wirkt keine Kraft auf das Elektron. Nach dem 1. Newton'schen Gesetz ist die Bewegung in x-Richtung daher __gleichförmig__.

In vertikaler Richtung (y-Richtung) wirkt auf das Elektron die konstante elektrische Kraft. Daher führt es in dieser Richtung nach dem zweiten Newton'schen Gesetz eine __gleichmäßig beschleunigte Bewegung__ aus.

</details>

<details style="margin-left:10%">

<summary> __Hinweise zu Bewegungsgleichungen__ </summary>

In horizontaler Richtung (x-Richtung): 

$x(t) = v_0 \cdot t$

In vertikaler Richtung (y-Richtung): 

$y(t) = \frac{1}{2} \cdot a \cdot t^2 $ wobei $a=\frac{F_{el}}{m}$

Ermitteln Sie nun die Wurfparabel $y(x)$. Stellen Sie dazu $x(t)$ nach der Größe $t$ um und setzen Sie diese in die Gleichung $y(t)$ ein.

</details>

<details style="margin-left:10%">

<summary> __Lösungsweg__ </summary>

Bewegungsgleichungen:

$x(t) = v_0 \cdot t$

$y(t) = \frac{1}{2} \cdot \frac{F_{el}}{m_e} \cdot t^2 $

Stelle $x(t)$ nach $t$ um: 

$t = \frac{x}{v_0}$

Setze $t$ in $y(t)$ ein, es ergibt sich die Wurfparabel y(x):

$ y(x) = \frac{1}{2} \cdot \frac{F_{el}}{m_e} \cdot \frac{x^2}{v_0^2}$

Die elektrische Kraft $F_{el}= \frac{U}{b} \cdot q_e$, wobei b der Plattenabstand des Kondensators ist. Setzt man das noch in y(x) ein, so ergibt sich

$ y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e} \cdot \frac{x^2}{v_0^2}$

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$ \boxed{y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot v_0^2} \cdot x^2}$

Dies ist die Gleichung für eine Parabel. Die Größen im Bruch sind alle gegeben, es gilt y~x2.

</details>

</p>

---

2. 2. Ermitteln Sie die Eintrittsgeschwindigkeit $v_0$, bei welcher die Elektronen genau den hinteren Rand der Platte erreichen. 


<p style="margin-left:10%">

@rangeQuiz2($v_0$, 5.74e7 , $\frac{m}{s}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösungfindung__ </summary>

Nutzen Sie die Lösung aus 2.1. Verwenden Sie die Bahnform. Legen Sie ein _geeignetes_ Koordinatensystem fest und überprüfen Sie, welche Korrdinaten die obere rechte Ecke des Kondensators hat.

</details>

<details style="margin-left:10%">

<summary> __Hinweise zum Koordinatensystem__ </summary>

Ein geeignetes Koordinatensystem wäre mit dem Ursprung am Eintrittsort des Elektrons in den Plattenkondensator (in der Abbildung der rote Punkt).

Die rechte obere Ecke des Kondensators wäre dann bei x=10cm und y=4cm.

</details>

<details style="margin-left:10%">

<summary> __Lösungsweg: Hinweise zur Nutzung der Gleichung y(x) __ </summary>

Die obere rechte Ecke des Kondensators besitzt die Koordinate (0,1 m | 0,04 m). Für die Bahngleichung (Wurfparabel) des Elektrons gilt:

$y(x) = \frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot v_0^2} \cdot x^2$

Mit $y=0,04m$ und $x=0,1m$. Stellt man die Gleichung nach $v_0$ um, so ergibt sich:

$v_0 = \sqrt{\frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot y}}\cdot x$

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

geg.: 

<p style="margin-left:10%">

$x=0,1m$

$y=0,04m$

$U=12\cdot10^3 V$

$|q_e|=1,602\cdot10^{-19}C$

$m_e=9,11\cdot10^{-31}kg$

$b=0,08 m$

</p>

ges.: $v_0$

Lsg.: _(Herleitung siehe Lösungsweg)_

$ v_0 = \sqrt{\frac{1}{2} \cdot \frac{U\cdot q_e}{b\cdot m_e \cdot y}}\cdot x$

$v_0 = 5,74 \cdot 10^7 \frac{m}{s}$

</details>

</p>


---

2. 3. __Partnerübung:__ Beschreiben Sie die Bewegung der Elektronen, wenn die Geschwindigkeit $v_0$ größer als der in 2.2. ermittelte Wert ist.


<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Ist $v_0$ größer, fliegen sie über die Kondensatorplatten hinweg. Durch die größere Geschwindigkeit ist weniger Zeit, sie zu der Platte _hin zu lenken_. Stellt man die Bahnkurve nach x um, ist x~v2. Eine größere Geschwindigkeit bedeutet bei gleichem y, also Plattenabstand, ein größeres x.

</details>

---

Zwischen den Kondensatorplatten soll dem elektrischen Feld ein homogenes Magnetfeld so überlagert werden, dass die Elektronen der Geschwindigkeit $1,8\cdot 10^7 \frac{m}{s}$ die Anordnung unabgelenkt durchfliegen.

2. 4. __Partnerübung:__ Ermitteln Sie die Orientierung des Magnetfeldes. Begründen Sie Ihre Aussage.

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Überprüfen Sie die Richtung der elektrischen Kraft. Die Lorentzkraft muss der elektrischen Kraft entgegen gerichtet sein.

Überlegen Sie, welche Hand man für die Bestimmung der Lorentzkraft auf Elektronen nutzen muss.

Nutzen Sie die Drei-Finger-Regel um die Richtung des magnetischen Feldes zu bestimmen.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Die elektrische Kraft auf die Elektronen wirkt nach oben. Demzufolge muss die Lorentzkraft nach unten wirken. Nutzt man die Drei-Finger-Regel mit der linken Hand (Daumen=Elektronenbewegung; Zeigefinger=Magnetfeld; Mittelfinger=Kraftrichtung [nach unten]) so ergibt sich, dass das Magnetfeld in die Tafelebene hinein zeigen muss.

</details>

---

2. 5. __Partnerübung:__ Zeigen Sie, dass der Betrag der magnetischen Flussdichte 8,3 mT sein muss.

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Stellen Sie die Gleichung für die elektrische Kraft und die Lorentzkraft auf. Setzen Sie beide Kräfte gleich. Stellen Sie die Gleichung nach der magnetischen Flussdichte $B$ um.

</details>

<details style="margin-left:10%">

<summary> __Kräftegleichungen__ </summary>

Für die elektrische Kraft gilt:

<p style="margin-left:10%">

$F_{el} = E_{el} \cdot q_e$

Die elektrische Feldstärke $E_{el}$ in einem Plattenkondensator errechnet man mit 

$E_{el} = \frac{U}{d}$ mit d .. Plattenabstand.

Daher ist

$F_{el} = \frac{U}{d} \cdot q_e$

</p>

Für die Lorentzkraft $F_L$ gilt:

<p style="margin-left:10%">

$F_L = q_e \cdot v \cdot B$

</p>

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Setzt man die elektrische Kraft gleich der Lorentzkraft so ergibt sich

$F_{el} = F_L$

$ \frac{U}{d} \cdot q_e = q_e \cdot v \cdot B$

Diese Gleichung muss noch nach B umgestellt werden.

$\boxed{B= \frac{U}{v\cdot d}}$

Setzt man die gegebenen Wert $U=12\cdot10^3 V$, $v=1,8\cdot10^7\frac{m}{s}$ und $d=0,08m$ ein, so ergibt sich

$B = 0,0083 T$

</details>

---


2. 6. Erklären Sie, in welche Richtung Elektronen mit einer kleineren Geschwindigkeit unmittelbar nach dem Einschuss in den Feldbereich abgelenkt werden.

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

Wenn die Elektronen langsamer fliegen, ändert sich die elektrische Kraft nicht. Die magnetische Kraft (_Lorentzkraft_) wird jedoch geringer, so dass die Elektronen nach oben abgelenkt werden.

</details>

---

Nun wird die Ablenkspannung ausgeschaltet, so dass nur noch das magnetische Feld vorhanden ist.

2. 7. *Ermitteln Sie die minimale Eintrittsgeschwindigkeit der Elektronen in das magnetische Feld, damit Sie den Feldbereich wieder verlassen, ohne auf eine Kondensatorplatte zu treffen.<br>_Hinweis: Hier müssen zur Vollständigkeit zwei Fälle betrachtet werden._

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![262_Lsg_f](https://diversewolken.ddns.net/nextcloud/index.php/s/qNeT5R6rQDm5DQ7/download)

</details>


## 7.3. Bewegung geladener Teilchen im homogenen Magnetfeld

### Übungsaufgaben - Geladene Teilchen im homogenen Magnetfeld

1. Aufgabe 2 a+b+c aus: [Abituraufgabe-2-abc](https://virtuelle-experimente.de/b-feld/uebungen/aufgaben.php)

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


### KI-Aufgabe: Bewegung eines Elektrons im B-Feld


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert.
</p>

---

__Ladung im B-Feld-Aufgabe:__<br> 

<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">
Ich habe folgende 4 Aufgaben bekommen: <br> 1. Erkläre, warum sich ein geladenes Teilchen in einem homogenen Magnetfeld auf einer Kreisbahn bewegt.<br> 2. Gib begründet qualitativ an, wie sich der Kreisbahnradius mit zunehmender Geschwindigkeit verändert.<br> 3. Wiederhole Aufgabe. mit veränderter magnetischer Flussdichte.<br> 4. Hat man Ionen identischer Geschwindigkeit und Ladung, kann man mit Hilfe eines homogenen Magnetfeldes einen Massenspektrograph, d.h. eine Trennung der Teilchen nach ihrer Masse erreichen. Erkläre, wie das funktionieren könnte. <br>
Stelle mir nacheinander die 4 Aufgaben. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungskurs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln. Schätze meine Ergebnisse zusammenfassend ein.</span>
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


## 7.4. e/m-Versuch mit Helmhotz-Spulen

### Fehlerrechnung am e/m-Versuch

## 7.5. Anwendung - Geladene Teilchen in elektrischen und magnetischen Feldern

> __Aufgabe:__ Erstelle in einer kleinen Gruppe innerhalb der nächsten 45 Minuten eine kurze Präsentation zu einem dieser Themen. Jede Präsentation sollte nicht mehr als 5 min dauern.

<p class="newspaper">

__Mögliche Themen:__

- Linearbeschleuniger

- Zyklotron

- Synchrotron

- Massenspektrometer

- magnetische Flaschen (Plasmaphysik)

- Elektronenmikroskopie

- Ionenantriebe (Raumfahrt)

<p class="cb">

__Inhalt:__

- kurze Einführung -> _Worum handelt es sich?_

- Anwendungsbereiche / Anwendungsbeispiele

- Erklärung der grundlegenden Physik: Teilchenbewegung in Feldern

- interessante Details / aktuelle Informationen

</p>

</p>