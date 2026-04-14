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

# Motivation 1

[Artemis2](https://www.tagesschau.de/video/video-1571622.html)

# Digitale Messwerterfassung mit Cassy

__Zur Überwachung und Steuerung komplexer technischer Anwendungen müssen verschiende physikalische Größen digital und automatisch gemessen werden. Diese Größen können sein:__




## Teil 1 - Einführung

<section class="flex-container">

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> __Experiment 1: Temperaturmessung__ </summary>

<div style="margin-left:5%">

> __Ziel:__ Temperatur-Zeit-Graph $\vartheta(t)$ auf Cassy anzeigen

</div>


<details style="margin-left:5%">

<summary> __Durchführung:__  </summary>

1. Verbinde den Temperatursensor mit deinem Cassy-Messgerät.

2. Überprüfe ob sich die Temperaturanzeige verändert, wenn du den Temperatursensor zwischen deine Finger klemmst.

3. Stelle einen sinnvollen Messbereich ein(Min-Max-Temperatur)

4. Starte eine automatische Messwertaufnahme und nimm die Temperaturkurve vom Greifen und Loslassen des Temperatursensors auf.

</details>

<details style="margin-left:5%">

<summary> __Hefternotizien:__  </summary>

![Hefternotizen_1](https://diversewolken.ddns.net/nextcloud/s/XWHCzdmocYS6JgH/download)

</details>

</details>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details>

<summary> __Cassy-Ziele__ </summary>

__Bedienung am Cassy-Messgerät:__

> - [ ] Sensor anschließen
> - [ ] korrekte Messwerterfassung kontrollieren
> - [ ] Maximaler u. minimaler Messwert (d.h. Messbereich einstellen)
> - [ ] Messwerte im Diagramm (als Graph) darstellen

![CassyDisplay](https://diversewolken.ddns.net/nextcloud/s/Cqtdwwc2L92e8gb/download)

</details>

</div>

</section>

### Motivation Teil 2

??[ÜberwachungImFahrzeug](https://www.youtube.com/watch?v=f2o9kfwBRks)

## Teil 2 - Automatisierte Messwertaufname von Spannung und Stromstärke


<section class="flex-container">

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> __Experiment 2: Spannung und Stromstärke__ </summary>

<div style="margin-left:5%">

> __Ziel:__ $U(t)$ und $I(t)$-Graph für das Einschalten einer Glühlampe ermitteln. 

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{0-1}}
**************
![Schaltkreis_Spannung](https://diversewolken.ddns.net/nextcloud/s/w8NBCSBjzbaqBDT/download)

**************

{{1-2}}
**************
![Schaltkreis_Spannung](https://diversewolken.ddns.net/nextcloud/s/TF3HcxiFQWZW9Hy/download)

**************

{{2}}
**************
![Schaltkreis_Spannung](https://diversewolken.ddns.net/nextcloud/s/ynzGtcbHrqiyi6n/download)
**************


</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

{{0-1}}
**************
![Schaltkreisfoto_Spannung](https://diversewolken.ddns.net/nextcloud/s/aomMwxBJD7KMGBz/download)

**************

{{1-2}}
**************
![Schaltkreisfoto_Stromstärke](https://diversewolken.ddns.net/nextcloud/s/JBAQppwWkcopQyk/download)

**************

{{2}}
**************
![Schaltkreisfoto_Spannung](https://diversewolken.ddns.net/nextcloud/s/CtconMErCS4gkiS/download)
**************

</div>

</section>


</div>

<details style="margin-left:5%">

<summary> __Durchführung:__  </summary>

1. Verbinde dein Glühlampe und einem Taster mit der Spannungsquelle.  Überprüfe durch Schließen des Schalters, ob die Glühlampe funktioniert.

2. Ergänze parallel zur Glühlampe das Cassy als Spannungsquelle -> Spannung $U$ aktivieren

3. Stelle das Cassy-Messgerät auf Spannungsmessung ein. Betätige den Schalter und überprüfe, ob das Cassy die Spannung anzeigt.

4. Erstelle die Startbedingung für die Messung (Trigger: $U>1\,\mathrm{V}$, Messzeit: $0,5\,\mathrm{s}$)

5. Wiederhole die Messung für die Stromstärke. Versuche selbstständig Trigger und Messzeit zu ermitteln.

</details>

</details>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details>

<summary> __Cassy-Ziele__ </summary>

__Bedienung am Cassy-Messgerät:__

> - [ ] [Cassy mit dem IPad verbinden](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/GK11_Cassy_Kondensator.md#14)
> - [ ] Spannungsmessung $U$ mit Cassy
> - [ ] Stromstärkemessung $I$ mit Cassy
> - [ ] Cassy-Steuerung mit IPad (App)
> - [ ] Zeitgesteuerte (automatisierte) Erfassung von $U(t)$ und $I(t)$
> - [ ] Messwerte als Diagramm darstellen und ausdrucken

</details>

<details>

<summary> __Cassy-Einstellungen__ </summary>

![Einstellungen_Cassy_1](https://diversewolken.ddns.net/nextcloud/s/bqpEdZ7gRZ8pJ85/download)

</details>

</div>

</section>

## _Hefternotiz:_ Automatisierte Messwertaufname von Spannung und Stromstärke

[qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/FVU_Cassy_A1.md)@color(Löse diesen Merksatz und notiere ihn anschließend in deinem Hefter!, blue)

<!-- 
    data-randomize 
    data-solution-button=false 
    data-max-trials="5"
-->
> Mit dem Cassy Messgerät können sehr viele [[ (__physikalische Größen__) | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]]  gemessen werden. Viele Größen benötigen einen eigenen [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | (__Sensor__) | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> <br> Für die __Spannung__ $U$ nutzen wir: [[ __physikalische Größen__ | (__Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ ) | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> Für die __Stromstärke__ $I$ nutzen wir [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | ( __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ ) | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> <br> Damit eine Messung automatisiert startet benötigt sie ein __Startsignal__, man nennt das [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | (__Trigger__) | __Messzeit__ | __Messintervall__ ]] . Dieses Startsignal kann z.B. das Überschreiten der Spannung $U>0,5\,\mathrm{V}$ sein. <br> <br> Bevor die Messung gestartet werden kann, muss die Gesamtzeit für die Messung eingestellt werden: die [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | (__Messzeit__) | __Messintervall__ ]] . <br> Außerdem muss  der Zeitabstand zwischen den Messwerten definiert werden, das heißt [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | (__Messintervall__) ]] .

# Teil 3 - Automatisierte Aufname: Heißleiter

<iframe src="https://diversewolken.ddns.net/pdfjs/web/viewer.html?file=https://diversewolken.ddns.net/nextcloud/s/9FZ5pTMLpDWPayt/download"
        width="100%" 
        height="600px">
</iframe>

## Video - Auto als Spion?

!?[NANO-DatenerfassungAnFahrzeugen](https://www.youtube.com/watch?v=1M3k1SQ5u6c)

## Diskussion - Automatische Messwerterfassung am Fahrzeug

Nutze folgenden QR-Code und lass dich zum Thema automatische Messwerterfassung am Fahrzeug interviewen.

[qr-code](http://10.102.1.3:3001/?q=F%C3%BChre%20mit%20mir%20ein%20Interview%20%C3%BCber%20die%20automatische%20Erhebung%20von%20Sensordaten%20in%20Fahrzeugen.%20Frage%20mich%20nach%20meiner%20Meinung%20zur%20Erhebung%20von%20personenbezogenen%20Daten%20(z.B.%20Gewicht,%20Fahrverhalten,%20h%C3%A4ufige%20Routen,%20Personenanzahl,%20Alter%20etc.)%20und%20das%20Recht%20auf%20diese%20Daten.%20Frage%20mich%20nach%20Vorteilen%20(z.B.%20erh%C3%B6hte%20Sicherheit,%20Komfort)%20aber%20auch%20Risiken%20(z.B.%20ungewollte%20Informationsfreigabe,%20Schutz%20der%20Pers%C3%B6nlichkeitsrechte).%20Stelle%20mir%20die%20Fragen%20eine%20nach%20der%20anderen%20und%20diskutiere%20mit%20mir%20anschlie%C3%9Fend%20meine%20Position.)