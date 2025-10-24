<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/5i8Bj7T9RFPsfcR/download

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


# Sonnensystem in 3D

Erstelle mit Hilfe von Geogebra dein eigenes Sonnensystem in __3D__.

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

---

2. Starte die Ansicht (3D-Projektion). Nutze dazu das Menu (drei Balken oben links), wähle __Ansicht__, deaktiviere __Grafik__ und aktiviere __3DGrafik__.

![2_3DAnsicht](https://diversewolken.ddns.net/nextcloud/index.php/s/amxsBz28ag4e3Gf/download)

---

3. Beobachte das __Drehen__ und __Zoomen__ in der 3D-Ansicht. <br> Klickst du mit einer Maustaste in das Koordinatensystem und hälst die Taste gedrückt, so kannst du die Ansicht __drehen__. Das Koordinatensystem reagiert recht empfindlich. <br> Rollst du mit dem mittleren Mausrad in der Ansicht, so kannst du hinein und hinaus zoomen. Achte darauf, dass der Zeiger über dem Koordinatenursprung liegt, wenn du zoomst. <br> <br> Zum __Drehen__ und __Verschieben__ kann man auch die Menupunkte nutzen.

![3_DrehenVerschieben](https://diversewolken.ddns.net/nextcloud/index.php/s/aNRGdZCZggYEd8L/download)

4. __Ursprüngliche Ansicht wiederherstellen:__ Ansicht komplett verdreht? Nutze die _Home_-Ansicht um zur Ausgangsdarstellung zurückzukehren.

![4_Home](https://diversewolken.ddns.net/nextcloud/index.php/s/eRctztKRZgB4wtj/download)

5. __Ansicht an Größe anpassen:__ Um alle Planetenbahnen darstellen zu können, empfiehlt es sich, die Darstellungsgrenzen anzupassen. Der Radius von Mars beträgt, 227.9 Mio km. Ändere daher die Grenzen von x-Achse und y-Achse zu ($\pm 250$). Wähle Einstellungen->Grundeinstellungen und dann:

| | |
| x Min | -250 |
| x Max | 250 |
| y Min | -250 |
| y Max | 250 |

![5_MinMax](https://diversewolken.ddns.net/nextcloud/index.php/s/3DBNAmtag8HyPfT/download)

6. Ergänze nun die Sonne im Ursprung des Koordinatensystems. Wähle dazu Punkt hinzugfügen, ändere die Farbe auf Gelb und benenne den Punkt als Sonne.

![6_Sonne](https://diversewolken.ddns.net/nextcloud/index.php/s/QsbqdeGLpSd5dcT/download)

6. 1. __Beschleunigung:__ Nun ergänzen wir einen Schieberegler _Beschleunigung_, mit welchem wir die Animationsgeschwindigkeit erhöhen können. Erstelle dazu eine Variable mit dem Namen __Beschleunigung=1__. 

![Beschleunigung1](https://diversewolken.ddns.net/nextcloud/index.php/s/oEqe2iZzQH7gLPT/download)

6. 2. Erstelle aus der Variable einen Schieberegler und passe die Grenzen an: __Min: 0,5 Max: 20 Schrittweite: 0,5__ (auswählbar im Einstellungsmenu oder in der Algebra-Ansicht). @color(_Hinweis: In der 3D-Ansicht lassen sich Schieberegler nicht einblenden._, orange)

![Beschleunigung2](https://diversewolken.ddns.net/nextcloud/index.php/s/6CjQnzoFMoCG3fZ/download)

7. Ergänze nun den ersten __Bahnradius__, wir beginnen mit der __Erde__. In der 3D-Ansicht, muss man zusätzlich zum __Mittelpunkt__ und __Radius__ noch eine Achse angeben. <br> <br> Wähle zunächst __Kreis mit Mittelpunkt, Radius und Richtung.__

![7_MenuKreis](https://diversewolken.ddns.net/nextcloud/index.php/s/RRkGjNtAHfxmQWK/download)

8. Klicke anschließend auf die __Sonne__, __die z-Achse (oben)__ und gib dann den __Bahnradius 149,6__ ein. Ändere nun Farbe und Linienstärke nach deinen Wünschen.

![8_BahnradiusErde](https://diversewolken.ddns.net/nextcloud/index.php/s/SjbKfNwMbMwbbG8/download)

9. Ergänze nun die Erde als Punkt auf der Erdbahn.

![9_Erde](https://diversewolken.ddns.net/nextcloud/index.php/s/B8badF4gkbbsoCc/download)

10. Die Bewegungsgeschwindigkeit und die Bahnradien der Erde kannst du aus dieser Tabelle ablesen.

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

11. Klicke nun die Erde an, gehe zu __Einstellungen->Allgebra__ und ergänze die Geschwindigkeit anhand obiger Tabelle.<br> Tippe dazu: @color(0.107*Beschleunigung,red). <br> Wechsle anschließend zu den Grundeinstellungen und wähle __Animation ein__. Alternativ kannst du auch das _Play_ Symbol neben der Erde nutzen.

![11_AnimationErde](https://diversewolken.ddns.net/nextcloud/index.php/s/aWdc85PB4TFRR6L/download)

12. Ergänze nun weitere Planeten (Merkur, Venus, Mars). 

13. Ändere anschließend die Hintergrundfarbe auf __Schwarz__ und blende das Koordinatensystem aus.

![13_Sonnensystem](https://diversewolken.ddns.net/nextcloud/index.php/s/jMpgRP8H3fxtyHa/download)