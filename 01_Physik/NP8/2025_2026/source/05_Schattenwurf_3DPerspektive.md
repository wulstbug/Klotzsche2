<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/yL6PWBAP7A5cZ3z/download

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


## Schattenwurf 3D-Perspektive

Erstelle mit Hilfe von Geogebra deinen eigenen Schattenwurf in __3D__.

Wechsle in einem weiteren Fenster [Klicke hier: Geogebra: 3D-Perspektive -> Schatten zeichnen](https://www.geogebra.org/classroom/yufw2qaq) und bearbeite folgende Anleitung. Gehe zu @color(Weiter ohne Anmeldung, orange) und nutze deinen Vornamen oder deine Initialien.

---



1. Zeichne eine senkrechte Hilfslinie zum Horizont durch die Sonne. 

2. Markiere den Schnittpunkt mit dem Horizont. Nenne diesen Punkt N.

3. Zeichne nun einen Strahl (s) von der Sonne durch die linke obere Ecke deines Objektes.

4. Zeichne nun einen Strahl (a) von N ausgehend, durch den unterhalb der Ecke aus 3. liegenden Punkt.

5. Konstruiere den Schnittpunkt (O)zwischen s und a.
    -> Dieser Punkt ist eine Ecke deines Schattens.

6. Vergleiche deine Konstruktion.

<div style="text-indent:10%">

<details>

<summary> Zwischenbild </summary>

![Vergleiche6](https://diversewolken.ddns.net/nextcloud/index.php/s/TfwxTdXPFkRr5nZ/download)<!-- style="max-height:400px" -->

</details>

</div>

     
7. Wiederhole diesen Vorgang für zwei weitere Ecken (hinten links, vorne rechts).

8. Vergleiche deine Konstruktion.

<div style="text-indent:10%">

<details>

<summary> Zwischenbild </summary>

![Vergleiche8](https://diversewolken.ddns.net/nextcloud/index.php/s/PgxTpAJNA6enGbR/download)<!-- style="max-height:400px" -->

</details>

</div>

9. Wähle Vieleck und verbinde die Eckpunkte zu einem sinnvollen Schatten.

<div style="text-indent:10%">

<details>

<summary> Menupunkt </summary>

![Vieleck](https://diversewolken.ddns.net/nextcloud/index.php/s/qXcdz4gpdZLjdxH/download)<!-- style="max-height:400px" -->

</details>

</div>

10. Vergleiche deine Konstruktion.


<div style="text-indent:10%">

<details>

<summary> Zwischenbild </summary>

![Vergleiche10](https://diversewolken.ddns.net/nextcloud/index.php/s/3FLELHRHbb2ixpw/download)<!-- style="max-height:400px" -->

</details>

</div>

11. Blende nun den zweiten Quader ein. Klicke dazu oben links auf Quader2 und wiederhole die Schattenkonstruktion.


<div style="text-indent:10%">

<details>

<summary> Zwischenbild </summary>

![Vergleiche11_1](https://diversewolken.ddns.net/nextcloud/index.php/s/YqBxWJCRrH78eP7/download)<!-- style="max-height:400px" -->

</details>

<details>

<summary> Lösung </summary>

![Vergleiche11_2](https://diversewolken.ddns.net/nextcloud/index.php/s/FWTP7kckBYEwcGy/download)<!-- style="max-height:400px" -->

</details>

</div>

12. Probiere nun einen Schattenlauf mit bewegter Sonne

     [Klicke hier: Geogebra: 3D-Schatten zeichnen mit Sonnenlauf](https://www.geogebra.org/classroom/trc9cuu8)

