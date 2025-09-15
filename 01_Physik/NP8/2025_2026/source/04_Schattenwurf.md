<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/WeRWZQKdzRbJetX/download

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


## Schattenwurf 3D mit Geogebra

Erstelle mit Hilfe von Geogebra deinen eigenen Schattenwurf in __3D__.

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

---

2. Starte die Ansicht (3D-Projektion). Nutze dazu das Menu (drei Balken oben links), wähle __Ansicht__, deaktiviere __Grafik__ und aktiviere __3DGrafik__.

![2_3DAnsicht](https://diversewolken.ddns.net/nextcloud/index.php/s/amxsBz28ag4e3Gf/download)

---

3. Beobachte das __Drehen__ und __Zoomen__ in der 3D-Ansicht. <br> Klickst du mit einer Maustaste in das Koordinatensystem und hälst die Taste gedrückt, so kannst du die Ansicht __drehen__. Das Koordinatensystem reagiert recht empfindlich. <br> Rollst du mit dem mittleren Mausrad in der Ansicht, so kannst du hinein und hinaus zoomen. Achte darauf, dass der Zeiger über dem Koordinatenursprung liegt, wenn du zoomst. <br> <br> Zum __Drehen__ und __Verschieben__ kann man auch die Menupunkte nutzen.

![3_DrehenVerschieben](https://diversewolken.ddns.net/nextcloud/index.php/s/aNRGdZCZggYEd8L/download)

4. __Ursprüngliche Ansicht wiederherstellen:__ Ansicht komplett verdreht? Nutze die _Home_-Ansicht um zur Ausgangsdarstellung zurückzukehren.

![4_Home](https://diversewolken.ddns.net/nextcloud/index.php/s/eRctztKRZgB4wtj/download)

5. Füge zunächst einen Punkt hinzu, der die Sonne darstellen soll. Tipp dazu in der Eingabe: __Sonne = (-5,0,5)__

![5_Sonne](https://diversewolken.ddns.net/nextcloud/index.php/s/9XT6oQed8Q2XDwk/download)

6. Ändere die Farbe der Sonne auf Gelb/Orange. Bewege die Ansicht, in dem du die linke Maustaste gedrückt hältst und die Maus bewegst. Du kannst den Ort der Sonne nun einsehen.

![6_Sonnenansicht](https://diversewolken.ddns.net/nextcloud/index.php/s/5A7jC2paaWnqczs/download)

7. Nun muss das erste schattenwerfende Objekt konstruiert werden. Wir wählen ein einfaches Quadrat, welches aufrecht steht. Definiere dazu die 4 Eckpunke:

- E1 = (0,2,0)
- E2 = (0,4,0)
- E3 = (0,2,2)
- E4 = (0,4,2)

![7_Eckpunkt](https://diversewolken.ddns.net/nextcloud/index.php/s/DCZbNNzCXwii9c5/download)

8. Ergänze nun die Eckpunkte zu einem Quadrat. Wähle dazu oben im Menü Vieleck und klicke anschließend die Eckpunkte im Uhrzeigersinn an.

![8_Vieleck1](https://diversewolken.ddns.net/nextcloud/index.php/s/9GBY6cJK3Yzz7db/download)

![8_Vieleck2](https://diversewolken.ddns.net/nextcloud/index.php/s/zor6eAFRdBXA2di/download)

9. Konstruiere nun die Randstrahlen von der Sonne zu den oberen Ecken des Quadrates.

![9_Randstrahlen](https://diversewolken.ddns.net/nextcloud/index.php/s/gDGBc7xG7ZaEGrJ/download)

10. Um den Schatten zu konstruieren, benötigen wir die Schnittpunkte  mit der Bodenfläche. Wähle Schnittpunkt, dann den Randstrahl und dann die graue Ebene.

![10_Schnittpunkt1](https://diversewolken.ddns.net/nextcloud/index.php/s/9GBY6cJK3Yzz7db/download)

![8_Schnittpunkt2](https://diversewolken.ddns.net/nextcloud/index.php/s/NFQqEKK6R3378XG/download)

11. Wiederhole den Vorgang mit dem zweiten Randstrahl. Ergänze anschließend ein Vieleck aus den unteren Ecken des Quadrates (E1, E2) sowie den Schnittpunkten (hier A und B).

![11_Schattenwurf](https://diversewolken.ddns.net/nextcloud/index.php/s/pDP8ESe5gRYQcWe/download)

12. Erganze nun geeignete Farben für das Quadrat (z.B. dunkelgrau) und den Schatten (schwarz). Achte darauf, dass du in den Einstellungen den Wert für Deckkraft (siehe Bild) auf 100 setzt.

![12_Farben1](https://diversewolken.ddns.net/nextcloud/index.php/s/L5oedM8T6RWY36s/download)

![12_Farben2](https://diversewolken.ddns.net/nextcloud/index.php/s/kEYqLePfe5bnaEm/download)

13. Blende nun noch die Rangstrahlen aus und ändere den Hintergrund der Konstruktion auf Schwarz.

![13_FinaleAnpassung](https://diversewolken.ddns.net/nextcloud/index.php/s/QiaRdKFWf65qWkH/download)

> Nun kannst du die Sonne anklicken und verschieben und die Schattenkonstruktion beobachten. Drehe die Ansicht um die Konstruktion von mehreren Seite zu beobachten.

----

14. Ergänze nun ein zweites Objekt im Bereich der negativen y-Achse z.B. ein Rechteck oder ein Dreieck.

__Beispiele:__

![14_NeueObjekte](https://diversewolken.ddns.net/nextcloud/index.php/s/WeRWZQKdzRbJetX/download)

