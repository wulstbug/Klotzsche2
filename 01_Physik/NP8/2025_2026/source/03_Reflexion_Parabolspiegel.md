<!--

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/2QswjeyfXeqwRtN/download

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

### Konstruktionsanleitung: Reflexion an einem Parabolspiegel

__Erklärung:__ Für einen exakten Brennpunkt ist die perfekte Spiegelform eine Parabel. Wir werden in diesem Abschnitt statt einer kugelförmigen Spiegelfläche eine Parabel verwenden.    


<details>

<summary> __Aufgabenteil 1:__ </summary>

<p style="margin:5%">

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

2. Blende das Koordinatensystem ein und platziere den Ursprung mittig.

     ![Koord](https://diversewolken.ddns.net/nextcloud/index.php/s/pGEcgSo6YKCakip/download)

3. Für eine Parabel benötigen wir eine Gerade und einen Punkt. Die Gerade wird die y-Achse sein. Setze einen Punkt auf die Koordinate (-10,0). Tipp dazu:

<p style="color:red;margin-left:10%">
     P= (-10,0) <br>
</p>

4. Nun erstellen wir die parabelförmige Spiegelfläche (Parabolspiegel). Wähle dazu Parabel, klicke dann auf den Punkt P und anschließend auf die y-Achse.

<p style="color:red;margin-left:10%">

     ![Para-Hs4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/nxc5GnMt3ng9ziT/download)

     ![Para-Hs4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/WQPPsWpQiaHG8mA/download)

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

