<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

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

### Konstruktionsanleitung: Reflexion an einem Parabolspiegel

__Erklärung:__ Für einen exakten Brennpunkt ist die perfekte Spiegelform eine Parabel. Wir werden in diesem Abschnitt statt einer kugelförmigen Spiegelfläche eine Parabel verwenden.    


<details>

<summary> __Aufgabenteil 1: Hauptspiegel__ </summary>

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

     ![Para-Hs4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/nxc5GnMt3ng9ziT/download) <!-- style="max-width:300px" -->
     
     ![Para-Hs4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/WQPPsWpQiaHG8mA/download) <!-- style="max-width:300px" -->

</p>

5. Blende nun den Punkt P aus (-> Objekt anzeigen).

6. Wir müssen nun einen Parallelstrahl zur x-Achse konstruieren. Setze dazu zunächst einen Punkt oberhalb der x-Achse. Wähle anschließend _Parallele Gerade_, klicke dann auf die x-Achse und anschließend auf den eben gesetzten Punkt.

7. Der Lichtstrahl darf nur bis zur Spiegelfläche laufen. Wir müssen also den Schnittpunkt zwischen der parallelen Gerade und dem Spiegel ermitteln. Wähle dazu _Schnittpunkt_ und klicke anschließend zurerst auf die parallele Gerade und anschließend auf den Spiegel.

     ![Para-HS7](https://diversewolken.ddns.net/nextcloud/index.php/s/6kSjHMW3k6mYEkf/download) <!-- style="max-width:300px" -->

8. Wir blenden nun die parallele Gerade aus, da sie keinen physikalischen Strahlengang darstellt. Klicke rechts auf die Gerade und wähle _Objekt anzeigen_. Ist der Haken verschwungen, wird die Gerade ausgeblendet.

9. Wir zeichnen nun einen Lichtstrahl, der am Spiegel endet. Wähle dazu _Strahl_ klicke anschließend __zuerst__ auf den Schnittpunkt am Spiegel und __danach__ auf den zusätzlichen Punkt (hier A). Ändere die Farbe des Strahls auf rot.

     ![Para-HS9](https://diversewolken.ddns.net/nextcloud/index.php/s/TY2QGeR2jcenMnm/download) <!-- style="max-width:300px" -->

10. Um das Lot zu ermitteln müssen wir an der Auftrefstelle des Lichtstrahls zuerst eine Tangente an den Spiegel zeichnen. Wähle dazu _Tangenten_, klicke anschließend auf den Spiegel und danach auf den Schnittpunkt von Spiegel und Strahl (hier B). Ändere die Farbe und die Linienstärke der Tangente.

     ![Sph-HS10.1](https://diversewolken.ddns.net/nextcloud/index.php/s/bJR44Ani5DTkLcY/download) <!-- style="max-width:300px" -->

     ![Sph-HS10.2](https://diversewolken.ddns.net/nextcloud/index.php/s/6Ny9iwHNgcQgfmd/download) <!-- style="max-width:300px" -->

11. Das Lot steht senkrecht auf der Tangente. Dazu wählen wir senkrechte Gerade, klicken auf die Tangente und dann auf den Schnittpunkt.

     ![Sph-HS11](https://diversewolken.ddns.net/nextcloud/index.php/s/tCZmsCm8cRNEbjM/download) <!-- style="max-width:300px" -->

12. Reflektiere (Spiegle) nun den einfallenden Lichtstrahl am Lot.

13. Blende nun den Schnittpunkt, den reflektierten Punkt, sowie die Tangente am Spiegel aus (siehe 8.).

     ![Sph-HS13](https://diversewolken.ddns.net/nextcloud/index.php/s/FJ5P3rLfEDCKaSX/download) <!-- style="max-width:300px" -->


13. Klicke nun rechts auf den reflektierten Lichtstrahl und wähle _Spur anzeigen_. Bewege anschließend den Punkt des einfallenden Lichtstrahls (hier D).

     ![Sph-HS14](https://diversewolken.ddns.net/nextcloud/index.php/s/neeHq5EPtRJW2Qm/download)

> Blende nun den als erstes erstellten Punkt ein. Dieser Punkt wird Brennpunkt der Parabel genannt. Wenn man die Lichtstrahlen verfolgt, erscheint diese Bezeichnung sehr treffen.


</p>

</details>


<details>

<summary> __Aufgabenteil 2: Sekundärspiegel__ </summary>

<p style="margin:5%">

Damit das Hubble-Teleskop eine kompakte Bauweise erhält, besitzt es einen zweiten parabelförmigen Hohlspiegel.

![Sekundärspiegel-Hubble](https://diversewolken.ddns.net/nextcloud/index.php/s/zz2YEtEYfaSoJpy/download)

Ergänze in deiner Zeichnung einen zweiten Hohlspiegel (Sekundärspiegel, welcher das Licht zurückwirft und die Abbildung kompakter machtn.)

1. Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

2. Füge einen zweiten Punkt (links vom ersten Brennpunkt) und eine zweite Gerade parallel zur y-Achse (zwischen erstem Brennpunkt und y-Achse ein).

3. Erstelle nun einen zweiten Spiegel (Sekundärspiegel, der nach außen gewölbt ist). Reflektiere den am Hauptspiegel reflektierten Lichtstrahl am Sekundärspiegel. Zeige seine Spur an. Verändere den Sekundärspiegel (über den Punkt und die Gerade) so, dass ein Brennpunkt erscheint.

![Sekundärspiegel](https://diversewolken.ddns.net/nextcloud/index.php/s/ryz8AxFnbg9DzkT/download)

</p>

</details>