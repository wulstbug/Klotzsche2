<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/4jcdw8fPN5AxSZb/download

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

### Konstruktionsanleitung: Reflexion an einem sphärischen Spiegel


<details>

<summary> __Aufgabenteil 1:__ </summary>

<p style="margin:5%">

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

2. Blende das Koordinatensystem ein und platziere den Ursprung mittig.

     ![Koord](https://diversewolken.ddns.net/nextcloud/index.php/s/pGEcgSo6YKCakip/download)

3. Setze einen Punkt (Mittelpunkt des kreisförmigen Spiegels auf den Koordinatenursprung). Benenne ihn mit M.

     ![Sph-Hs3](https://diversewolken.ddns.net/nextcloud/index.php/s/n3NXmqosdm7qQMK/download)

4. Für den Kreisbogen benötigen wir zwei weitere Punkte. Setze einen Punkt B = (18,-3) und einen Punkt C = (18,3). Trage dazu in die Eingabezeile ein:

<p style="color:red;margin-left:10%">
B= (18,-3) <br>
C= (18,3)


     ![Sph-Hs4](https://diversewolken.ddns.net/nextcloud/index.php/s/NJjo4gXMNagnRzb/download)

</p>

5. Ergänze nun einen Kreisbogen. Klicke dazu auf _Kreisbogen_ und wähle __zuerst den Mittelpunkt__ und dann die Punkte B & C __gegen den Uhrzeigersinn__, d.h. zuerst B, dann C.


     ![Sph-Hs5.1](https://diversewolken.ddns.net/nextcloud/index.php/s/cGNP9jpGg5pCdSn/download) 

     ![Sph-HS5.2](https://diversewolken.ddns.net/nextcloud/index.php/s/Z9LLLeHfwjNpfJZ/download)

6. Wir müssen nun einen Parallelstrahl zur x-Achse konstruieren. Setze dazu zunächst einen Punkt oberhalb der x-Achse. Wähle anschließend _Parallele Gerade_, klicke dann auf die x-Achse und anschließend auf den eben gesetzten Punkt.

     ![Sph-Hs6.1](https://diversewolken.ddns.net/nextcloud/index.php/s/Lzxs4D9FPeBLTQm/download) 

     ![Sph-HS6.2](https://diversewolken.ddns.net/nextcloud/index.php/s/XbEpSmYRf5g7K6K/download)

7. Der Lichtstrahl darf nur bis zur Spiegelfläche laufen. Wir müssen also den Schnittpunkt zwischen der parallelen Gerade und dem Spiegel ermitteln. Wähle dazu _Schnittpunkt_ und klicke anschließend zurerst auf die parallele Gerade und anschließend auf den Spiegel.

     ![Sph-Hs7.1](https://diversewolken.ddns.net/nextcloud/index.php/s/bL36igAPGHK9rtY/download) 

     ![Sph-HS7.2](https://diversewolken.ddns.net/nextcloud/index.php/s/d85HdALQ7GxsgCT/download)

8. Wir blenden nun die parallele Gerade aus, da sie keinen physikalischen Strahlengang darstellt. Klicke rechts auf die Gerade und wähle _Objekt anzeigen_. Ist der Haken verschwungen, wird die Gerade ausgeblendet.

9. Wir zeichnen nun einen Lichtstrahl, der am Spiegel endet. Wähle dazu _Strahl_ klicke anschließend __zuerst__ auf den Schnittpunkt am Spiegel und __danach__ auf den zusätzlichen Punkt (hier D). Ändere die Farbe des Strahls auf rot.

     ![Sph-Hs9.1](https://diversewolken.ddns.net/nextcloud/index.php/s/Rx67pTdFDZy48bo/download) 

     ![Sph-HS9.2](https://diversewolken.ddns.net/nextcloud/index.php/s/i4ZtdFdPWSdFYWF/download)

10. Füge nun das Lot ein. Das Lot ist eine Gerade vom Spiegel (Schnittpunkt) durch den Mittelpunkt des Kreises. Ändere die Strichart auf _gestrichelt_ und die Farbe auf blau.

     ![Sph-HS10](https://diversewolken.ddns.net/nextcloud/index.php/s/J95B3b7bLSAqKjC/download)

11. Spiegel nun den ersten Punkt am Lot (hier D). Füge anschließend eine Strahl vom Schnittpunkt des Spiegels zum gespiegelten Punkt (hier D') ein.

     ![Sph-HS11](https://diversewolken.ddns.net/nextcloud/index.php/s/DESXyz7AiyNJ5a2/download)

12. Blende nun den Schnittpunkt, sowie die Randpunkte des Spiegel aus (siehe 8.).

13. Klicke nun rechts auf den reflektierten Lichtstrahl und wähle _Spur anzeigen_. Bewege anschließend den Punkt des einfallenden Lichtstrahls (hier D).

     ![Sph-HS11](https://diversewolken.ddns.net/nextcloud/index.php/s/4jcdw8fPN5AxSZb/download)

> Was kannst du über den Schnittpunkt aller reflektierten Lichtstrahlen aussagen?


</p>

</details>


---

<details>

<summary> __Aufgabenteil 2:__ </summary>

<p style="margin-left:5%">

Wechsle in einem weiteren Fenster [hier zum Labyrinth](https://www.geogebra.org/classroom/xfwnnpnr) und bearbeite folgende Anleitung. Finde das Tor, in welches Lichtstrahl 1 trifft. Konstruiere den Lichtweg sauber.

<div style="margin:5%">

![VglLab](https://diversewolken.ddns.net/nextcloud/index.php/s/HXzk3JjHMA4oNcf/download)

</div>

</p>

</details>
