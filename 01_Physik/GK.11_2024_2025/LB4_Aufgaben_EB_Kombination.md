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

.blue {
    color:blue
}

.green {
    color:darkgreen
}

.red {
    color:darkgreen
}
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@onload
window.LIA.settings.font_size = 2
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


## 3. Übungen zur Kombination aus statischen E- und B-Feld

@color(Löse aus den folgenden Aufgaben die __Grundlagen__ und wähle __eine__ der beiden Aufgaben I oder II., blue)

_Hinweis: Es gibt einige Aufgaben die als **Partnerübung** gekennzeichnet sich. Hier empfiehlt es sichin einer kleinen Gruppe zu arbeiten._ <br>

@color(-> Eine Person stellt die Frage und schaut sich die Lösung an. Die andere Person beantwortet die Frage und wird unterstützt., blue)

### Grundlagen

1. Notiere die Ladung des Elektrons, die Masse eines Protons, die Ladung und Masse eines Alpha-Teilchens

<p style="margin-left:10%">

<details>

<summary> Hinweis zur Lösung </summary>

Nutze die Formelsammlung unter der Rubrik: _Tabellierte Werte_

</details>

---

@rangeQuiz2($q_e$, -1.602e-19 , $C$)

@rangeQuiz2($m_p$, 1.67e-27, $kg$)

@rangeQuiz2($q_\alpha$, 3.204e-19 , $C$)

@rangeQuiz2($m_\alpha$, 6.64e-27, $kg$)

</p>

2. __Partnerübung__ 

2. 1. Definiere den Begriff homogenes Feld.

<details style="margin-left:10%">

<summary> Lösung </summary>

Ein homogenes Feld hat an jedem Ort (d.h. an jeder Stelle im Raum) den gleichen Wert (z.B. Feldstärke).

</details>

2. 2. Definiere den Begriff statisches Feld.

<details style="margin-left:10%">

<summary> Lösung </summary>

Ein statisches Feld ist zeitlich konstant, d.h. es verändert sich mit der Zeit nicht.

</details>

### Übungsaufgabe I

1. ![Geschwindigkeitsfilter](https://diversewolken.ddns.net/nextcloud/index.php/s/PfptPJcdpDkjDNX/download) (85) Elektronen treten aus einer Glühkathode K aus und werden durch ein Feld zwischen ihr und der Anode A (Spannung zwischen K und A beträgt U = 500,0 V) zu letzterer hin beschleunigt. Durch die Öffnung C in der Anode treten Elektronen in den Raum ein, in dem zwei Felder wirken:

- ein elektrisches Feld mit der elektrischen Feldstärke E = konst. > 0, dessen Feldlinien parallel zur Zeichenebene verlaufen (in der Skizze weggelassen), und 

- ein magnetisches Feld mit der magnetischen Flussdichte B = 0,012 T, dessen Feldlinien senkrecht aus der Zeichenebene heraus verlaufen (in der Skizze punktförmig dargestellt).

1. 1. Ermittle die Geschwindigkeit $v_1$ derjenigen Elektronen, die an der Oberfläche der Kathode keine kinetische Energie hatten, wenn Sie an der Öffnung C ankommen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($v_1$, 13.3e6 ,$\frac{m}{s}$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Hier kann man die kinetische Energie, die die Elektronen dazu gewinnen gleich der potentiellen Energie der Ladung im elektrischen Feld gleichsetzen.

<details style="margin-left:10%">

<summary> __Hinweis zu Formeln__ </summary>

Die kinetische Energie findet sich in der Formelsammlung. Die potentielle elektrische Energie wurde in Lernbereich II (elektrisches Feld) hergeleitet.

<details style="margin-left:10%">

<summary> _pot. elektr. Energie_ </summary>

$E_{pot.,el.} = E_{el} \cdot q \cdot d \overset{E_{el}=\frac{U}{d}}{=} U \cdot q$

</details>

</details>

</details>

<details>

<summary> __Lösung__ </summary>

![85_Lsg_a](https://diversewolken.ddns.net/nextcloud/index.php/s/r9LweMS7dLMSWPk/download)

</details>

</p>

---

1. 2. Ermittle die Geschwindigkeit $v_2$ solcher Elektronen an der Öffnung C, welche die Katodenoberfläche in Richtung C mit der kinetischen Energie $E_{kin} = 3,2 \cdot 10^{-17} Ws$ verlassen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($v_2$, 15.7e6 ,$\frac{m}{s}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Ähnlich zu a) muss hier zur potentiellen elektrischen Energie der Ladung noch die kinetische Energie der Anfangsgeschwindigkeit addiert werden. Dann wieder Energien gleichsetzen und auflösen.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![85_Lsg_b](https://diversewolken.ddns.net/nextcloud/index.php/s/SGpjarRsK859zkA/download)

</details>

</p> 

---

1. 3. __Partnerübung:__ Die Elektronen treten nach der Öffnung C in den Bereich elektrisches/magnetisches Feld ein. Begründen Sie, dass die Kräfte, die auf ein bewegtes Elektron unter dem Einfluss beider Felder wirken, unterschiedliche Richtungen haben.

<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Auf die Elektronen wirken sowohl die elektrische Kraft, als auch die magnetische Kraft (_Lorentzkraft_). Überprüfen Sie für beide Kräfte die Kraftrichtung.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

- die Kraft des elektrischen Feldes wirkt aufgrund der negativen Ladung des Elektrons und der Polung des Kondensators nach unten. 
- das magnetische Feld wirkt senkrecht zur Geschwindigkeit des Elektrons (_Lorentzkraft_), die Richtung wird mit der
linken-Hand-Regel bestimmt und zeigt nach oben.

</details>

</p>

---

1. 4. Stellen Sie eine Gleichung zur Berechnung des Betrages (des Wertes) der Gesamtkraft auf, wenn bekannt ist, dass sich die Einzelkräfte in der Richtung unterscheiden. (Die Gewichtskraft wird vernachlässigt).


<p style="margin-left:10%">

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Ermitteln Sie mit Hilfe der Formelsammlung die Formel für die elektrische Kraft innerhalb eines Plattenkondensators und Formel für die Lorentzkraft.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$F_{ges} = F_{el} - F_L $

$F_{ges} = E_{el} \cdot q - q \cdot v \cdot B $

</details>

</p>

---

1. 5. Berechnen Sie die notwendige elektrische Feldstärke, damit die Elektronen, die an der Oberfläche der Kathode keine kinetische Energie hatten, die Anordnung geradlinig durchfliegen.

<p style="margin-left:10%">

__Lösungsüberprüfung:__

@rangeQuiz2($E_{el}$, 159.1e3 ,$\frac{V}{m}$)

<details style="margin-left:10%">

<summary> __Hinweise zur Lösung__ </summary>

Überlegen Sie, unter welcher Bedingung die Elektronen keine Ablenkung erfahren (d.h. geradlinig weiter fliegen).

<details style="margin-left:10%">

<summary> __Hinweise zu Kräften__ </summary>

Keine Ablenkung erfolgt, wenn die Gesamtkraft (siehe 1.4.) gleich Null ist. Setzen Sie diese Gleichung gleich Null und ermitteln Sie daraus den Wert für $E_{el}$.

</details>

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$0 = F_{el} - F_L $

$ E_{el} \cdot q = q \cdot v \cdot B \Big| :q$

$ E_{el} = v \cdot B $

$ E_{el} = 13,3\cdot10^{6} \frac{m}{s} \cdot 0,012 T \hspace{0.5cm} \Big[ \frac{m\cdot V\cdot s}{s\cdot m^2} \Big]$

$ E_{el} = 159,1 \cdot 10^{3} \frac{V}{m} $

Alle Elektronen mit der oben berechneten Geschwindigkeit fliegen geradlinig durch die gekreuzten Felder hindurch. Alle anderen werden nach oben oder unten abgelenkt.

Damit wirkt eine solche Anordnung als Geschwindigkeitsfilter für geladene Teilchen und wird z.B. beim Massenspektrographen 
eingesetzt. Die Masse der Teilchen spielt dabei keine Rolle.

</details>

</p>

### Übungsaufgabe II

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

2. 2. Ermitteln Sie die Eintrittsgeschwindigkeit $v_0$, bei welcher die Elektronen genau die hinteren Rand der Platte erreichen. 


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

2. 7. *Ermitteln Sie minimale Eintrittsgeschwindigkeit der Elektronen in das magnetische Feld, damit Sie den Feldbereich wieder verlassen, ohne auf eine Kondensatorplatte zu treffen.<br>_Hinweis: Hier müssen zur Vollständigkeit zwei Fälle betrachtet werden._

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![262_Lsg_f](https://diversewolken.ddns.net/nextcloud/index.php/s/qNeT5R6rQDm5DQ7/download)

</details>