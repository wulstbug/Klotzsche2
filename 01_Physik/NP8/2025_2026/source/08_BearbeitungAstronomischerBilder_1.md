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


### Erstellung eines astronomischen RGB-Bildes

1. Laden Sie zunächst den Datensatz aus FITS-Dateien für die Antenna-Galaxy auf Ihren PC herunter: [Antennengalaxie.zip](https://diversewolken.ddns.net/nextcloud/index.php/s/TR68AnTQMttWxpN/download)

2. Entpacken Sie die Dateien in das gleiche Verzeichnis (rechtsklick -> hier entpacken)

3. Wechsel Sie im Browser zum FITS-Bildbearbeitung: [OberservingWithNASA](https://waps.cfa.harvard.edu/eduportal/js9/software.php)

4. Zunächst wird das Bild des Lagoon-Nebels geladen. Klicken Sie im <br> Menu auf _Image_ -> _Close Image_

5. Laden Sie zunächst die FITS-Datei für die roten Bilddaten. <br> Menu: _Image_ -> _Open_ -> Antennengalaxy_Rot.fits.

6. Zunächst öffnet sich ein sehr dunkles Bild. Ändern Sie die Darstellung der Helligkeitsskala zu logarithmisch. <br> Menu: _Scale_ -> _log_. Sie sollten nun die Antennengalaxy als Graustufenbild erkennen können.

<p style='margin-left:10%'>

![https://diversewolken.ddns.net/nextcloud/index.php/s/9tp4AbWfw4TPitH/download](https://diversewolken.ddns.net/nextcloud/index.php/s/9tp4AbWfw4TPitH/download)

</p>

7. Passen Sie zunächst die Werte für _Low Brightness Limit_, _High Brightness Limit_, _Strech/Contrast_ und _Shift/Bias_ einzeln an.

<details style='margin-left:10%'>

<summary> Vorschläge </summary>

Low Brightness Limit: 10

High Brightness Limit: Voreinstellung

Strech/Contrast: 1,3

Shift/Bias: 0,48

</details>

8. Ändern Sie anschließend die Farbskala zu Rot. <br> Menu: _Scale_ -> _Red_

<p style='margin-left:10%'>

![https://diversewolken.ddns.net/nextcloud/index.php/s/DsPrPQfmS2LxNgt/download](https://diversewolken.ddns.net/nextcloud/index.php/s/DsPrPQfmS2LxNgt/download)

</p>

9. Wiederholen Sie den Vorgang für die Dateien Grün und Blau.

<p style="margin-left:10%">

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

@color(__ROT:__, red)

![https://diversewolken.ddns.net/nextcloud/index.php/s/DsPrPQfmS2LxNgt/download](https://diversewolken.ddns.net/nextcloud/index.php/s/DsPrPQfmS2LxNgt/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

@color(__GRÜN:__, green)

![https://diversewolken.ddns.net/nextcloud/index.php/s/tBpGrqkyfEkMxLF/download](https://diversewolken.ddns.net/nextcloud/index.php/s/tBpGrqkyfEkMxLF/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

@color(__BLAU__, blue)

![https://diversewolken.ddns.net/nextcloud/index.php/s/jNZ32KRtqKfrRaC/download](https://diversewolken.ddns.net/nextcloud/index.php/s/jNZ32KRtqKfrRaC/download)

</div>

</section>

</p>

10. Nutzen Sie nun das Tool _Blending_ um die Bilder übereinander zu legen. <br> Menu: _Tools_ -> _Blending_

11. Sobald Sie das Häkchen bei _Image Blending_ gesetzt haben, werden die Bilder übereinander gelegt. Wenn Sie das Häckchen wieder heraus nehmen, können Sie sich durch anklicken der einzelnen Bilder jedes einzelne nochmals anschauen.

