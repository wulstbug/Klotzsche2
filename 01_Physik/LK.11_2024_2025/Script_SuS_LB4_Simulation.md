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

# LB 4 Modellierung und Simulation


![ModellierungSimulation](https://diversewolken.ddns.net/nextcloud/index.php/s/ETBrpgNNii6A2gE/download)

**Download-Link der Simulationssoftware _Moebius_:**

[Moebius-Lizenz-Sachsen](https://www.primtext.de/moebius/moeb-setup-sachsen.exe)

## 4.1 Einführung

![TB_Simulation_1](https://diversewolken.ddns.net/nextcloud/index.php/s/TcbtzC4iX557WHe/download)

![TB_Simulation_1](https://diversewolken.ddns.net/nextcloud/index.php/s/bRRYfqjs7oKe2d5/download)


## 4.2 Modellierung einer Bewegung mit dem Simulationstool _Moebius_

![TB_Demo_FreierFall_1](https://diversewolken.ddns.net/nextcloud/index.php/s/wXxCppGqtw8A5ag/download)

![Tafelbild_Demo_FreierFall_2](https://diversewolken.ddns.net/nextcloud/index.php/s/sdMRCrsy24LAC9K/download)


### 4.2.1 Experimente Freier Fall

[DateiAblage](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr)

![Experiment](https://diversewolken.ddns.net/nextcloud/index.php/s/XHwzajk8jjrRjkG/download)

![TennisBall](https://diversewolken.ddns.net/nextcloud/index.php/s/72oyGXjfT2i38cw/download)

### 4.2.2 Experiment und Modellierung - Freier Fall mit Luftreibung - Muffinförmchen

__Aufgabenstellung:__ Untersuche den freien Fall eines Muffinförmchens im Experiment und in der Simulation. Ermittle den $c_w$-Wert des Muffin-Förmchens und vergleiche Zeit-Orts-Graphen von Experiment und Simulation.

__Halte deine Ergebnisse in Protokollform fest (jedes Gruppenmitglied).__

__Vorgaben Experiment:__ 

- die Masse des Förmchens beträgt $0,69 g \pm 0,01 g$

- ermittle den Flächeninhalt $A$ des Förmchens

- das Muffinförmchen soll eine Fallstrecke von ca. 80cm aus der Ruhe zurücklegen

- nutze für die Aufnahme der experimentellen Bewegungsdaten die Videoanalyse-Software VIANA2: 

     - um einen hohen Kontrast zu erreichen, sollte das weiße Förmchen vor der dunklen Tafel fallen gelassen werden
     
     - nutze eine Bildwiederholrate von 120 fps, dann betragen die Zeitschritte der Analyse 1/120 s

     - achte darauf, dass das Förmchen im Flug nicht _eiert_
     
     - achte darauf, dass sich das Förmchen __entlang__ einer eingestellten Achse bewegt (x oder y)

- exportiere die Daten der Analyse-Software als CSV-Datei und lege sie auf dem Tablet im _Downloads_-Ordner mit einem geeigneten Namen ab

- um die Daten auf den PC zu transferieren, kannst du diesen Link [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr) benutzen. Erstelle einen Ordner mit deinem Namen, öffne diese Präsentation dann auf dem Laptop und speichere deine CSV-Datei in einem geeigneten Ordner auf dem Laptop

<details style="margin-left:10%">

<summary> Vergleichswerte zum Experiment </summary>

Die Flugzeit nach 0,6 s beträgt etwa 0,8 m

$ A = 0,005 m²$

</details>

---

__Vorgaben Simulation:__

- erstelle eine Simulation, welche den freien Fall des Förmchens unter Berücksichtigung der Luftreibung simulieren kann

- achte bei den Zeitschritten auf das Zeitintervall deiner experimentellen Daten (nutze 5 Kommastellen)

- ergänze in deiner Simulation die experimentell bestimmten Parameter 

- ermittle durch Annähern der simulierten Daten an die experimentellen Daten den $c_w$-Wert des Förmchens

__Auswertung Option 1 (wenig Restzeit):__

- speichere den Orts-Zeit-Graphen deiner Simulation ab

- lade diesen Orts-Zeit-Graphen in deinem Ordner [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr) wieder hoch

- die Lehrkraft wird dir einen Ausdruck deines Zeit-Orts-Diagramms erstellen

- trage in deine Simulation die experimentellen Werte im Abstand von 0,1s per Hand ein

- verbinde diese experimentellen Messwerte mit einer Freihandkurve

__Auswertung Option 2 (ausreichend Restzeit):__

- öffne die experimentelle CSV-Datei auf dem Laptop mit Microsoft-Excel

- wähle in der Simulationsumgebung _Moebius_ die Darstellung als Tabelle, __klicke rechts__ auf die Tabelle und wähle _"mit Excel öffnen"_

- überprüfe, ob die Zeitschritte aus dem Experiment und der Simulation übereinstimmen

- kopiere deine Daten als Tabelle und nutze die Inhalte einfügen Option von Excel <br> ![InhalteEinfügen](/download)

- erstelle eine neue Tabelle mit

<p style="margin-left:10%;margin-right:10%">

| A | B | C |
| $t$ in s | $x_{exp}$ in m | $x_{sim}$ in m |
| .. | .. | .. |

</p>

- erzeuge ein Orts-Zeit-Diagramm wo experimentelle und simulierte Daten verglichen werden

- lade das Diagramm [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr) in deinen Ordner hoch und lass es dir von der Lehrkraft ausdrucken

__Unterschiede zwischen Simulation und Experiment:__

- diskutiere in der Gruppe die Unterschiede zwischen Experiment und Simulation

### 4.2.3. Auswertung Experiment Freier Fall Muffin-Förmchen

Die experimentellen Daten der letzten Unterrichtsstunde können [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr) abgerufen werden.

__Arbeitsaufträge:__

<p style="margin-left:5%">

__Aus Experiment:__

- öffne zunächst die CSV-Datei deiner experimentellen Messwerte mit Excel <br> (_Hinweis: Wenn du keine experimentellen Daten vorliegen hast, kannst du die Demo-Daten in der Datei @color(Demo_Exp.csv, orange) nutzen_)

- überprüfe, welche Koordinate (x oder y) in deinem Versuch entlang der Bewegungsrichtung gesetzt worden ist

- notiere für deinen Versuch die gesamte Flugzeit ($t_{flug}$) und die gesamte Flugstrecke $x_{flug}$ bzw.$y_{flug}$

__Aus Simulation:__

- öffne deine Simulation der letzten Unterrichtsstunde <br>(_Hinweis: Wenn du keine Simulation aus der letzten Stunde vorliegen hast, kannst du die die Datei @color(Demo_Sim.prg, orange) nutzen._)

- der Parameter $c_w$-Wert der Simulation soll nun derart angepasst werden, dass $t_{flug}$ und $x_{flug}$ bzw. $y_{flug}$ übereinstimmen

- nutze die Tabellenansicht @color("Datei -> Druckereinrichtung", blue), um die Werte entsprechend zu vergleichen

- wenn du die Simulation zu deiner Zufriedenheit angepasst hast, speichere sie ab

__Ausdrucken:__

- die simulierten Graphen können direkt in ein PDF gedruckt werden

- wähle dazu im Menu: @color("Datei -> Druckereinrichtung -> PDCCreator", blue)

- wähle anschließend: @color("Name -> PDF-Drucken", blue)

- __deaktiviere die Tabellensicht__

- wähle @color("Datei->Drucken", blue)

- ![Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/3MGSwtD8H5dB6dd/download) achte darauf dass @color(__NUR__, red) die Boxen @color("__Programm  Startwerte und Schaubild__",blue) aktiviert sind

- speichere das PDF unter deinem Namen (z.B. ) und lade es anschließend [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/JSBai3W7eQAHstr) wieder hoch 

- lass es dir von der Lehrkraft ausdrucken

__Vergleich von Simulation und Experiment:__

- trage in deine Simulation die experimentellen Datenpunkte (CSV-Datei oben) in einem zeitlichen Abstand von 0,1s per Hand ein

- verbinde diese experimentellen Messwerte mit einer Freihandkurve

__Unterschiede zwischen Simulation und Experiment:__

- diskutiere in der Gruppe die Unterschiede zwischen Experiment und Simulation

</p>

### 4.2.4 Modelierung Dachdecker-Aufzug

![DDAufzug](https://www.kranzubehoer.com/images/product_images/info_images/Kranmeister_Dachdeckeraufzug.jpg) @color(Es wird ein Demonstationsexperiment zu einem Modell eines Dachdeckeraufzugs gezeigt., blue)

__Aufgabenstellung:__ (1-4) gemeinsam | (5-9) selbsständig

1. Erstelle eine Skizze des Aufbaus und zeichne die auftretenden Kräfte und Messgrößen ein.

2. Untersuche mit einer Handstopuhr Strecke und Zeit an vier Messpunkten.

3. Nutze den CAS und ermittle eine quadratische Funktion (Quadratische Regression), welche die experimentellen Bewegungsdaten möglichst gut wiederspiegelt.

4. Ermittle aus der Regressionsfunktion die Beschleunigung $a_{reg}$.

5. Nutze das Simulationstool _Moebius_ und erstelle einen Programmcode, welcher die Kräfte und die daraus resultierende Bewegung simuliert

6. Ändere den auftretenden Reibungskoeffizienten derart, dass die simulierten Daten mit den experimentellen Messwerten übereinstimmen

7. Ermittle aus den simulierten Daten den Reibungskoeffizient $\mu_R$, die Reibungskraft $F_r$ und die Beschleunigung $a_{sim}$.

8. Vergleiche die ermittelten Beschleunigungen $a_{reg}$ und $a_{sim}$. Diskutiere Gründe für eventuelle Unterschiede.

9. Untersuche für den Messaufbau wesentliche Fehlerquellen.

10. Diagramm (@color(mit Namen,red)) können [hier](https://diversewolken.ddns.net/nextcloud/index.php/s/EsCQXsMK5kwK7ia) hochgeladen und ausgedruckt werden

__Vorbetrachtung:__ Physikalische Grundlagen + Programmcode

<p class="newspaper">


__Formeln:__

Gewichtskraft:

$$ F_g = m_1 \cdot g$$

Reibungskraft:

$$ F_r = m_2 \cdot g \cdot \cos\alpha \cdot \mu_r $$

Hangabtriebskraft:

$$ F_h = m_2 \cdot g \cdot \sin\alpha $$

Beschleunigende Kraft:

$$ F = F_g - F_r - F_h $$

Beschleunigung:

$$ a = \frac{F}{(m_1 + m_2)} $$

Geschwindigkeitsänderung:

$$ \mathrm{d}v = a \cdot \mathrm{d}t $$

Ortsänderung:

$$ \mathrm{d}s = v \cdot \mathrm{d}t $$

<p class="cb">

__Moebius - Programmcode__

<details>

<summary> Moebius - Code </summary>

```

Fg = m1 * g

Fr = m2 * g * cosa * mu

Fh = m2 * g * sina

F = Fg - Fr - Fh

a = F/(m1+m2)

v = v + a*dt

s = s + v*dt

t = t + dt


```

</details>

</p>

</p>

__Versuchsaufbau/Materialien:__

<p class="newspaper">

__Foto:__

![Foto](https://diversewolken.ddns.net/nextcloud/index.php/s/4tkfQFenHKaKmFk/download)

<p class="cb">

__Skizze:__

![VersuchsAufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/zbAYMGQggBjzkN5/download)

</p>

</p>

__Messwerte:__

![Messwerte](https://diversewolken.ddns.net/nextcloud/index.php/s/XCJG3WKTt5mwkos/download)

__Auswertung:__

<p style="margin-left:5%">

_Regression:_

![Regression](https://diversewolken.ddns.net/nextcloud/index.php/s/Ax9rHc78wEPsEBH/download)

_Simulation:_

![Simulation](https://diversewolken.ddns.net/nextcloud/index.php/s/FpZnAFjmqEKpWjo/download)

</p>

__Fehlerbetrachtung:__

__Ergebnis:__


## 4.3 Hinweise zur Erstellung eines Protokolls

<p class="newspaper">

Beim **Auswerten eines Experiments** werden Vergleiche durchgeführt, Diagramme angefertigt und interpretiert, Berechnungen vorgenommen und analysiert.  
Bestandteil der Auswertung vieler Experimente sind Fehlerbetrachtungen zur Abschätzung der Genauigkeit der Messungen.

__Zu jedem Experiment gehört ein Protokoll__

Bestandteile eines solchen Protokolls sind neben Name und Datum:

- **Aufgabe**

- **Vorbereitung** (theoretische Grundlagen, Geräte und Hilfsmittel, experimentierte Ordnung, Messwertetabellen)

- **Durchführung** (Erfassung der Beobachtungen und der Messungen)

- **Auswertung** mit Fehlerbetrachtung und Formulierung eines Ergebnisses mit Bezug auf die Aufgabe

<p class="cb">

<!-- style="width:50%" -->
``` ascii 

o------------------o
|                  |
| Aufgabenstellung |<-o
|                  |  |
o--------o---------o  |
         |            |
         v            |
o------------------o  |
|                  |  |
|   Vorbereitung   |  |
|                  |  |
o--------o---------o  |
         |            |
         v            |
o------------------o  |
|                  |  |
|   Durchführung   |  |
|                  |  |
o--------o---------o  |
         |            |
         v            |
o------------------o  |
|                  |  |
|    Auswertung    o--o
|                  |
o------------------o

```

</p>

</p>