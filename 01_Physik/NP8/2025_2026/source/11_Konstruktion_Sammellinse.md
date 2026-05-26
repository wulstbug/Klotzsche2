<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/twWpgsoaTm7Fcwd/download

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

# Konstruktionsanleitung - Abbildung an einer Sammellinse

<details>

<summary> __Aufgabenteil 1:__ </summary>

<p style="margin:5%">

__Aufgabe 1:__ Wechsle in einem weiteren Fenster [hier zu Geogebra](https://www.geogebra.org/classroom/dmvmdyvu) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

1. Zeichne zunächst die optische als Gerade auf der x-Achse.

---

2. Zeichne anschließend die Linsenebene als Strecke (Bereich [-5 bis 5]) auf der y-Achse.

---

3. Definiere anschließend die Variablen $g=5$, $G=2$ und $f=3$. Tippe dazu

@color(g=5, red) <br>

@color(G=2, red) <br>

@color(f=3, red) <br>

![Vlg1](https://diversewolken.ddns.net/nextcloud/s/W5FnSssDngTdHmi/download)

---

4. Erstelle nun den Gegenstand. Dazu musst du zwei Punkte definieren (den unteren (G0) und den oberen Punkt (G1)) und ihn anschließend als Vektor (G0->G1) definieren. <br> Achte auf __Groß/Kleinschreibung__

<p style="color:red; margin-left:5%">

G0 = (-g, 0)

G1 = (-g, G)

</p>

<p style="margin-left:5%">

Wähle anschließend den Menupunkt _Vektor_ und verbinde G0 und G1.

</p>

![Vlg2](https://diversewolken.ddns.net/nextcloud/s/n8sMNy2ttrCKgZF/download)

---

5. Definiere nun die beiden Brennpunkte (F1, F2) mit der Variable f.

<p style="color:red; margin-left:5%">

F1 = (f, 0)

F2 = (-f, G)

</p>

![Vlg3](https://diversewolken.ddns.net/nextcloud/s/FECLbtZt8nt6WZs/download)

---

5. Konstruiere nun ausgehend von der Spitze des Gegenstandes Parallelstrahl, Brennpunktstrahl und Mittelpunktstrahl. 



---

6. Zeichne Sie das Lot durch den Punkt D. Wähle dazu _Senkrechte Gerade_, klicke dann auf den Spiegel und anschließend auf den Schnittpunkt von Lichtstrahl und Spiegel.

<p style="margin:5%">

| ![Vgl6](https://diversewolken.ddns.net/nextcloud/index.php/s/GMgcYbeWrzJkCLC/download) | ![Vgl6b](https://diversewolken.ddns.net/nextcloud/index.php/s/KDDDXw6ArwEJaDj/download)<!-- style="margin:10px"--> |

</p>

---

7. Ändere die Linienform auf gestrichelt, die Dicke auf 1 und die Farbe auf blau. 

![Vgl7](https://diversewolken.ddns.net/nextcloud/index.php/s/mp7ZZNmgHqZkM6t/download)

---

8. Zeichne den Einfallswinkel. Setze dazu zuerst einen Punkt (E) auf das Lot, wähle dann Winkel und klicke die Punkte CDE in dieser Reihenfolge. Wähle bei den Einstellungen den Reiter _Darstellung_ und ändere die Größe des Winkels auf 100. Beschrifte auch das Lot.

<p style="margin:5%">

| ![Vgl8a](https://diversewolken.ddns.net/nextcloud/index.php/s/GdG6MFxTJX75cJK/download) | ![Vgl8b](https://diversewolken.ddns.net/nextcloud/index.php/s/gGBjBj6FdLypQe2/download)<!-- style="margin:10px"--> |

</p>

---

9. Für die Reflexion des Lichtstrahls verwenden wir den Befehl _Spiegle an Gerade_. Wähle dazu zuerst den Punkt C und dann das Lot. Du erhälst einen Punkt C, der am Lot gespiegelt wurde. 

| ![Vgl9a](https://diversewolken.ddns.net/nextcloud/index.php/s/zGKeSrHiXQMkbtk/download) | ![Vgl9b](https://diversewolken.ddns.net/nextcloud/index.php/s/664JKd34YMtkjBT/download)<!-- style="margin:10px"--> |

---

10. Zeichne einen Strahl von Punkt D durch C'. Ergänze die Farbe des Lichtstrahls zu rot, beschrifte den Lichtstrahl mit reflektierter Lichtstrahl. Ergänze den Reflexionswinkel.

![Vgl10](https://diversewolken.ddns.net/nextcloud/index.php/s/yiSTSgpFNJRoP7f/download)<!-- style="margin:10px"-->

---

11. Beschrifte nun noch den neuen Winkel (er heißt $\beta$) mit $\alpha'$. Kopiere dazu das $\alpha$ aus der Beschriftung des ersten Winkels und setze es im zweiten Winkel mit einem __'__ ein.

![Vgl11](https://diversewolken.ddns.net/nextcloud/index.php/s/ysHAQjxma8A5AZ7/download)<!-- style="margin:10px"-->

---

12. Blende nun die überflüssigen Punkte E und C' aus. Klicke dazu rechts auf die Punkte und wähle _Objekt anzeigen_.

---

13. Überprüfe deine Konstruktion.

![Vgl12](https://diversewolken.ddns.net/nextcloud/index.php/s/fqt36pkWXAkc7tY/download)<!-- style="margin:10px"-->

---

</p>

</details>

---

<details>

<summary> __Aufgabenteil 2:__ </summary>

<p style="margin:5%">

14. Konstruiere nun einen zweite Spiegel, an dem der reflektierte Lichtstrahl ebenfalls reflektiert wird.

![Vgl13](https://diversewolken.ddns.net/nextcloud/index.php/s/twWpgsoaTm7Fcwd/download)<!-- style="margin:10px"-->



15. @color(Achtung:, red) Der reflektierte Lichtstrahl geht nicht durch den zweiten Spiegel hindurch. Konstruiere zuerst den Schnittpunkt (H) zwischen reflektiertem Lichtstrahl und Spiegel 2. Klicke nun rechts auf den reflektierten Lichtstrahl und blende ihn aus (Objekt anzeigen). Es wird nun nur noch der Schnittpunkt H angezeigt, der reflektierte Lichtstrahl bleibt versteckt.

<div style="margin:5%">

<details>

<summary> Hinweise (zum Aufklappen) </summary>

| ![Vergleich15a](https://diversewolken.ddns.net/nextcloud/index.php/s/TowjQPbxWEnnkBq/download) | ![Vergleich15](https://diversewolken.ddns.net/nextcloud/index.php/s/NPdKMyTibFnGXtc/download) |

</details>

</div>

16. Zeichne nun eine Strecke vom Spiegel1 zum Spiegel2. Für den Spiegel2 ist dieser Strahl nun der einfallende Lichtstrahl.


<div style="margin:5%">

<details>

<summary> Hinweise (zum Aufklappen) </summary>

![Vergleich16a](https://diversewolken.ddns.net/nextcloud/index.php/s/N8neeeEg897odSE/download)

</details>

</div>

17. Wiederhole nun die Prozedur zum reflektieren des Lichtstrahls an Spiegel2. Benenne die Winkel mit $\alpha_2$ und $\alpha_2'$

<div style="margin:5%">

<details>

<summary> Hinweise (zum Aufklappen) </summary>

![Vergleich17](https://diversewolken.ddns.net/nextcloud/index.php/s/pLezfiAept7gAFW/download)

</details>

</div>

</p>

</details>

---

<details>

<summary> __Aufgabenteil 3:__ </summary>

<p style="margin-left:5%">

Wechsle in einem weiteren Fenster [hier zum Labyrinth](https://www.geogebra.org/classroom/xfwnnpnr) und bearbeite folgende Anleitung. Finde das Tor, in welches Lichtstrahl 1 trifft. Konstruiere den Lichtweg sauber.

<div style="margin:5%">

![VglLab](https://diversewolken.ddns.net/nextcloud/index.php/s/HXzk3JjHMA4oNcf/download)

</div>

</p>

</details>
