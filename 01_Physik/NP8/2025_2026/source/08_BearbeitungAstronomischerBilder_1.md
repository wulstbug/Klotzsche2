<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/s92S5jps7G29Fbz/download

language: de

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


# Bearbeitung Astronomischer Bilder (1)


__Arbeitsablauf:__

1. __Datei besorgen:__ Astronomische Daten werden in einem eigenen Datei-Format, dem __FITS-Format__ gespeichert.

---

2. __Datei in Bearbeitungsprogramm laden:__ FITS-Dateien können nur von speziellen Programmen gelesen werden. Wir nutzen die Seite https://ogy.de/gykl_fits

<details style='margin-left:10%'>

<summary> @color(Details, blue) </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

2. 1. Rufen wir die Seite https://ogy.de/gykl_fits auf, so erhalten wir zunächst einen Willkommensbildschirm der uns in die Nutzung des Programms einführt.

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/K3Hy3i5XWWsRa3m/download)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

2. 2. Wir können uns das Tutorial ansehen (Englisch) oder die Info wegklicken. Wir öffnen heute mindestens ein Archiviertes Bild. Das erste Bild ist eine Aufnahme des Mondes. Klicke auf @color(Archived Images, blue) und öffne die Datei __Moon160919094536__

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/resR9ynmMfxHBm9/download)

</div>

</section>




</details>

---

3. __Graustufen geeignet darstellen:__ Astronomische Bilder enthalten keine Farben sondern Helligkeitsstufen (Graustufen). Bevor man einem Bild Farbe hinzufügt, muss die Darstellung geeignet angepasst werden.

<details style='margin-left:10%'>

<summary> @color(Details, blue) </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

3. 1. Bei einer astronomischen Aufnahme wird das Bild meistens sehr lange beleuchtet. Daher gibt es nicht nur Helligkeitswerte am Objekt selbst, sondern auch im __Hintergrund__. <br> <br> Der Hintergrund des Mondes sollte eigentlich schwarz sein, ist aber grau darstellt.

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/en8HK7mz5y7cqjs/download)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

3. 2. Um einen grau erscheinenden Untergrund zu reduzieren, können wir die __untere Schwelle__, d.h. den Wert für einen schwarzen Bildpunkt anpassen. Diese Schwelle nennt man @color(Low Brightness Limit, red). <br> <br> @color(Bewege den Schieber vorsichtig nach links und rechts.Beobachte die Anpassung des Hintergrundschwarz. Ein geeigneter Wert ist hier 300. Stelle das ein., blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_3.2](https://diversewolken.ddns.net/nextcloud/index.php/s/resR9ynmMfxHBm9/download)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

3. 3. Auch die __Obere Schwelle__ kann hier angepasst werden, sie heißt @color(High Brightness Limit, red). <br> <br> @color(Verändere auch hier den Reiter und beobachte das Bild. Hier ist der voreingestellte Wert von 809 sinnvoll., blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/yGqZA89CnRmrCm5/download)

</div>

</section>

</details>


---

4. __Farbdarstellung bearbeiten:__ Wenn eine geeignete Graustufendarstellung gelungen ist, kann mit der Farbbearbeitung begonnen werden.


<details style='margin-left:10%'>

<summary> @color(Details, blue) </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

4. 1. Wir haben bis zu diesem Punkt nur ein Graustufen-Bild. An dieser Stelle wollen wir dem Bild eine Farbe verpassen. Mit Hilfe des Reiters. Im Menüpunkt _Color_ gibt es verschiedene Farbtabellen/Farbverläufe, welche  dem Bild zugewiesen werden können. <br> <br> @color( Probiere verschiedene Farbverläufe aus. Wähle anschließend eine Einstellung die dir gefällt., blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_4.1](https://diversewolken.ddns.net/nextcloud/index.php/s/i24GN2Zb8mZBm9r/download)

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

---

4. 2. Mit den Schiebereglern _Stretch/Contrast_ lassen sich die Farbwerte verschieben und die Darstellungen anpassen.  <br> <br> @color(Probiere verschiedene Einstellungen aus., blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_4.2](https://diversewolken.ddns.net/nextcloud/index.php/s/DjEZ7nQLx2n4zqq/download)

</div>

</section>

</details>

5. Position des Objektes anpassen


<details style='margin-left:10%'>

<summary> @color(Details, blue) </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

5. 1. Wir können die Position eines dargestellten Objektes innerhalb unseres Bildausschnittes gut anpassen. Dafür benötigen wir das _Tool_: __SHIFT__  <br> <br> @color( Wähle im Menüpunkt _Tools_ __SHIFT__. Verschiebe den Mond innerhalb deines Bildes ein bisschen. ACHTUNG: WILDES Klicken führt zu Verzögerungen. , blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_5.1](https://diversewolken.ddns.net/nextcloud/index.php/s/Mmij7MaLkDZDwA8/download)

</div>

</section>

</details>


---

6. __Daten abspeichern:__ Um ein Bild mit den gegebenen Einstellungen abzuspeichern, nutze den Menüpunkt _Image_ ->Save as FITS. <br> <br> Speichere die FITS-Datei in einem eigenen Order in deinem Laufwerk.

---

7. Ein zweites Bild bearbeiten. Wähle in den __Archived Images__ die Datei __Hubble-Lagoon-502nVisB__.

<details style='margin-left:10%'>

<summary> @color(Details, blue) </summary>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

7. 1. Zunächst siehst du in diesen Daten nichts. Der hier vom HUBBLE-Teleskop aufgenommene Nebel hat eine sehr schwache Intensität. Wir müssen durch eine geeignete Einstellung die schwachen Bildsignale deutlich sichtbar machen. <br> <br> @color(Wähle dazu im Menü _Scale_ die Option _Log_. Nun werden die Helligkeitswerte auf einer Logarithmischen Skala dargestellt., blue)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![FITS_5.1](https://diversewolken.ddns.net/nextcloud/index.php/s/mox49BDKfSJrMCc/download)

</div>

</section>

7. 2. Probiere anschließend eine geeignete Anpassung der Helligkeitswerte und der Farbtabelle.

</details>

---

8. __Bilder überblenden:__ Das Programm hat im Hintergrund beide Bilder geladen. Du kannst nun über den Menüpunkt _Tools_ -> _Blending_ beide Bilder übereinander legen. <br> <br> @color(Probiere es einfach aus., blue)

