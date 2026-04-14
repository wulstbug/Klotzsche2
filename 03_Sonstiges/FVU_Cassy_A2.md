<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://www.sciencedaily.com/images/1920/Quantum-Clock.webp

@style
.lia-effect__circle {
    display: none !important;
} 
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 20px;
}
.flex-child,
.flex-child-1 { flex: 1; }
.flex-child-2 { flex: 2; }
.flex-child-3 { flex: 3; }
.flex-child-4 { flex: 4; }
.flex-child-5 { flex: 5; }
.flex-child-6 { flex: 6; }
.flex-child-7 { flex: 7; }
.flex-child-8 { flex: 8; }

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

@media (max-width: 500px) {
    .flex-child,
    .flex-child-1,
    .flex-child-2,
    .flex-child-3,
    .flex-child-4,
    .flex-child-5,
    .flex-child-6,
    .flex-child-7,
    .flex-child-8 {
        flex: 100%; /* Makes the child divs take up the full width on slim devices */
        margin-right: 0; /* Removes the right margin */
    }
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
    display: block;
}

@end

@onload
window.LIA.settings.font_size = 2


const canvas = document.querySelector('.lia-canvas')
if (canvas) {
  canvas.classList.remove('lia-navigation--visible')
  canvas.classList.add('lia-navigation--hidden')
}

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

@timer2

<div style="position: fixed; right:50px; top:300px;">

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
<div style="float:left;margin-right:5px">
@0$\ $=$\ $ 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-(@1))/Math.abs(@1)
    input <= 0.03
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:10px">
@2
</div>
</div>
@end

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:10px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-(@1))/Math.abs(@1)
    input <= 0.2
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

@rangeQuiz0
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-(@1))
    input == 0
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

mode: presentation

-->


# Quiz - Festigung Cassy Messgerät

__Frage 1 – Single Choice__

Warum ist die digitale Messwerterfassung in der Technik wichtig?

- [( )] Damit Physiklehrer weniger korrigieren müssen
- [(X)] Zur Überwachung und Steuerung komplexer technischer Anwendungen
- [( )] Um analoge Messgeräte teurer erscheinen zu lassen
- [( )] Weil digitale Geräte besser aussehen

__Frage 2 – Multiple Choice__

Welche physikalischen Größen wurden im Unterricht mit dem Cassy gemessen?

- [[X]] Temperatur
- [[X]] Spannung
- [[X]] Stromstärke
- [[ ]] Schallgeschwindigkeit
- [[ ]] Luftfeuchtigkeit

__Frage 3 – Single Choice__

Wie wird der Temperatursensor beim ersten Experiment getestet?

- [( )] Man hält ihn unter fließendes Wasser
- [( )] Man legt ihn auf die Heizung
- [(X)] Man klemmt ihn zwischen die Finger
- [( )] Man pustet ihn an

__Frage 4 – Single Choice__

Welcher Graph soll in Experiment 1 auf dem Cassy angezeigt werden?

- [( )] $U(t)$ – Spannung-Zeit-Graph
- [( )] $I(t)$ – Stromstärke-Zeit-Graph
- [(X)] $\vartheta(t)$ – Temperatur-Zeit-Graph
- [( )] $s(t)$ – Weg-Zeit-Graph

__Frage 5 – Zuordnung (Lückentext)__

Geben Sie den Kanal an, mit welchem die folgende Größe gemessen wird.

Die **Spannung** $U$ wird über [[Kanal A]] gemessen (Stecker: rot + schwarz).
Die **Stromstärke** $I$ wird über [[Kanal B]] gemessen (Stecker: schwarz + blau).

__Frage 6 – Single Choice__

Was versteht man beim Cassy unter einem **Trigger**?

- [( )] Den Knopf zum Ausschalten des Geräts
- [( )] Den Anschluss für den Sensor
- [(X)] Ein Startsignal, das die automatische Messung auslöst
- [( )] Die Batterieanzeige

__Frage 7 – Single Choice__

Welcher Trigger wurde in Experiment 2 für die Spannungsmessung verwendet?

- [( )] $I > 1\,\mathrm{A}$
- [(X)] $U > 0,5\,\mathrm{V}$
- [( )] $\vartheta > 30\,°\mathrm{C}$
- [( )] $t > 10\,\mathrm{s}$

__Frage 8 – Single Choice__

Welche Messzeit wurde für die Spannungsmessung beim Einschalten der Glühlampe eingestellt?

- [( )] $5\,\mathrm{s}$
- [( )] $1\,\mathrm{min}$
- [(X)] $1\,\mathrm{s}$
- [( )] $10\,\mathrm{s}$

__Frage 9 – Multiple Choice__

Welche Einstellungen müssen vor einer automatisierten Messung am Cassy vorgenommen werden?

- [[X]] Trigger festlegen
- [[X]] Messzeit einstellen
- [[X]] Messintervall definieren
- [[ ]] Bildschirmhelligkeit anpassen
- [[ ]] WLAN-Passwort eingeben

__Frage 10 – Single Choice__

Was beschreibt das **Messintervall**?

- [( )] Die Gesamtdauer der Messung
- [( )] Die Anzahl der Sensoren
- [(X)] Den Zeitabstand zwischen zwei aufeinanderfolgenden Messwerten
- [( )] Die Pause zwischen zwei Experimenten

__Frage 11 – Single Choice__

Wie wird das Cassy-Messgerät im Experiment gesteuert?

- [( )] Ausschließlich über Tasten am Gerät
- [( )] Per Fernbedienung
- [(X)] Über ein iPad mit der Cassy-App
- [( )] Per Sprachsteuerung

Frage 12 – Single Choice

Wie wird das Cassy zur Spannungsmessung an der Glühlampe angeschlossen?

- [(X)] Parallel zur Glühlampe
- [( )] In Reihe zur Glühlampe
- [( )] Parallel zur Spannungsquelle und in Reihe zur Glühlampe gleichzeitig
- [( )] Es wird gar nicht an den Schaltkreis angeschlossen

Frage 13 – Ja/Nein (Single Choice)

Viele physikalische Größen benötigen einen eigenen Sensor, um mit dem Cassy gemessen zu werden.

- [(X)] Richtig
- [( )] Falsch

