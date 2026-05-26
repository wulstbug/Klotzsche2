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

![Vlg4](https://diversewolken.ddns.net/nextcloud/s/3bybBERcDcmpd4N/download)

---

6. Anschließend den Ort den Schnittpunkt der Strahlen und damit das Bild des Gegenstandes.

![Vlg5](https://diversewolken.ddns.net/nextcloud/s/Nx9ZyS5yoi8HttH/download)

</p>

</details>

---

<details>

<summary> __Aufgabenteil 2:__ </summary>

<p style="margin:5%">

1. Konstruiere das Bild an einer Zerstreungslinse. Gleiche Werte (g=5, G=2, f=3).

</p>

</details>

---

<details>

<summary> __Aufgabenteil 3:__ </summary>

<p style="margin-left:5%">


</p>

</details>
