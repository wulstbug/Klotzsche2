<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/4pAPR6JNCBBnynD/download

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

<div style="position: fixed; right:50px; top:20px;">

<details>

<summary> Uhrzeit </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=de&size=small&timezone=Europe%2FBerlin" width="100%" height="90" frameborder="0" seamless></iframe> 

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

mode: presentation

-->


# Sonnensystem in 2D

Erstelle mit Hilfe von Geogebra dein eigenes Sonnensystem.

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

2. Blende das Koordinatensystem ein und platziere den Ursprung mittig.

![Koord](https://diversewolken.ddns.net/nextcloud/index.php/s/pGEcgSo6YKCakip/download)

3. Erstelle die Sonne als zentralen Punkt im Koordinatenursprung. Setze die Farbe auf ein kräftiges gelb und gib dem Punkt den Namen __Sonne__.

![Sonne](https://diversewolken.ddns.net/nextcloud/index.php/s/ZkKEG8A5F8rZGSE/download)

4. Erstelle nun die erste Planetenbahn. Zur Vereinfachung nehmen wir an, dass es sich um eine Kreisbahn handelt. Den Radius geben wir in Millionen-Kilometern an. Auf der nächsten Seite findest du die Angaben zum Merkur. Wähle dazu __Kreis mit MP und Radius__.

<details style="color:blue; margin-left:10%">

<summary> Planetenbahnen: Radien und mittlere Geschwindigkeiten</summary>

Sonnenradius: 696.000 km

<!-- data-type="bar" data-show
-->
| Planet   |Sonnenabstand (Mio. km) |
|----------|------------------------|
| Merkur   |57.9                    |
| Venus    |108.2                   |
| Erde     |149.6                   |
| Mars     |227.9                   |
| Jupiter  |778.3                   |
| Saturn   |1427.0                 |
| Uranus   |2871.0                 |
| Neptun   |4498.0                |

<!-- data-type="bar" data-show -->
| Planet   | Geschwindigkeit (Mio km/h) |
|----------|------------------------|
| Merkur   | 0.172                |
| Venus    | 0.126                |
| Erde     | 0.107                |
| Mars     | 0.087                 |
| Jupiter  | 0.047                 |
| Saturn   | 0.035                 |
| Uranus   | 0.025                 |
| Neptun   | 0.020                 |

</details>

![Merkurbahn](https://diversewolken.ddns.net/nextcloud/index.php/s/wSMfk2kXKK6T67i/download)

5. Klicke zunächte auf die @color(Sonne, orange) und trage für den Radius den Wert aus dem Diagramm ein, hier 57,9 (Mio-km). Es empfielt sich nun etwas heraus zu Zoomen um den Kreis zu sehen. Ändere die Farbe der Kreisbahn so, dass es zum Merkur passt.

![Merkurbahn2](https://diversewolken.ddns.net/nextcloud/index.php/s/746Y27XgfrgWxFe/download)

6. Nun muss der Merkur als Punkt auf der Kreisbahn gesetzt werden. Wähle dazu Punkt setzen und klicke auf die Kreisbahn. Ändere die Farbe und den Namen des Punktes entsprechend.

![Merkurbahn2](https://diversewolken.ddns.net/nextcloud/index.php/s/WdFZ2KMMpZ9JScH/download)

7. Nun ergänzen wir einen Schieberegler _Beschleunigung_, mit welchem wir die Animationsgeschwindigkeit erhöhen können. Erstelle dazu eine Variable mit dem Namen __Beschleunigung__. 

![Beschleunigung1](https://diversewolken.ddns.net/nextcloud/index.php/s/oEqe2iZzQH7gLPT/download)

8. Erstelle aus der Variable einen Schieberegler und passe die Grenzen an: __Min: 0,5 Max: 20 Schrittweite: 0,5__ (auswählbar im Einstellungsmenu oder in der Algebra-Ansicht.) Blende den Regler anschließend ein.

![Beschleunigung2](https://diversewolken.ddns.net/nextcloud/index.php/s/6CjQnzoFMoCG3fZ/download)

8. Um die Bewegung des Mekur zu animieren wird als nächstes die _Bewegungsgeschwindigkeit_ eingestellt. Nutze dazu in den Einstellungen des Merkur-Punktes den Reiter _Algebra_. Die Beschleunigung des Merkur ergibt sich aus der Bewegungsgeschwindigkeit (Angabe auf der nächsten Seite). Hier müssen wir die Geschwindigkeit in Millionen-Km-Pro-Stunde angeben. <br> In der Tabelle steht der Wert $\approx$ 172000 km/h, dass sind 0,172332 Mio km/h. <br> <br> Trage bei Geschwindigkeit folgendes ein: <br> <br> @color(0.172*Beschleunigung ,red).

![Beschleunigung3](https://diversewolken.ddns.net/nextcloud/index.php/s/bcEy9jWS4S7kXF3/download)

9. Wechsle nun zum Reiter _Grundeinstellungen_ und klicke: _Animation ein_ Der Punkt sollte sich zu bewegen beginnen.

10. Ergänze nun die Planeten Venus, Erde und Mars, indem du die Punkte 4-9 wiederholst.

11. Ändere die Hintergrundfarbe zu schwarz. Klicke dazu auf den Hintergrund, wähle Einstellungen und suche im unteren Bereich der Grundeinstellungen die _Hintergrundfarbe_.
