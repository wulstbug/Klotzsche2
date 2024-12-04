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

- um die Daten auf den PC zu transferieren, kannst du diesen Link benutzen. Erstelle einen Ordner mit deinem Namen, öffne diese Präsentation dann auf dem Laptop und speichere deine CSV-Datei in einem geeigneten Ordner auf dem Laptop

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