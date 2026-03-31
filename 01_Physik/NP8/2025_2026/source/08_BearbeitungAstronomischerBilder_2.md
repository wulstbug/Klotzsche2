<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/JPT7NmcBYP7wX7z/download

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



### Erstellung eines astronomischen RGB-Bildes (2)

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

12. Passen Sie die Farbzusammensetzung für die einzelnen Bilder an. Sie können auch andere Farbskalen als die Rot-Grün-Blau-Skala wählen.

------


__Eigenes Bild erstellen__


1. Galaxie oder Nebel

<p style="margin-left:10%">

Nutzen Sie eines der folgenden Archive, um ein eigenes Bild zu kreieren.

![Protoplanetarer Nebel](https://diversewolken.ddns.net/nextcloud/index.php/s/PqgERr2xt8i7Med/download "[__Download: Protoplanetarer Nebel Roberts22__](https://diversewolken.ddns.net/nextcloud/index.php/s/z8aNGd9ZH5RReCA/download)") ![Messier17](https://diversewolken.ddns.net/nextcloud/index.php/s/qbFaWHTfAeWd6mT/download "[Download: __Messier17__](https://diversewolken.ddns.net/nextcloud/index.php/s/jEkJ3dx7ksBxFSG/download)")![Download __Andromeda__](https://diversewolken.ddns.net/nextcloud/index.php/s/6g6T2Hx7a6wbtZs/download "[Download __Andromeda__](https://diversewolken.ddns.net/nextcloud/index.php/s/6EAJGojPg2bbJx4/download)") ![Sternenhaufen](https://diversewolken.ddns.net/nextcloud/index.php/s/mc5HffHedeGa2H7/download "[Download __Sternenhaufen M35__](https://diversewolken.ddns.net/nextcloud/index.php/s/SNH69qqnJ97KYf8/download)") ![Sternengeburtsort](https://diversewolken.ddns.net/nextcloud/index.php/s/DgbMbws45onKZwq/download "[Download __Sternengeburtsnebel N11B__](https://diversewolken.ddns.net/nextcloud/index.php/s/GXWMXnSBMGE8yCE/download)") ![Antennengalaxie](https://diversewolken.ddns.net/nextcloud/index.php/s/9tp4AbWfw4TPitH/download "[Download __Antennengalaxy__](https://diversewolken.ddns.net/nextcloud/index.php/s/TR68AnTQMttWxpN/download)") ![BoxNebula_NGC6309](https://diversewolken.ddns.net/nextcloud/index.php/s/YpCrG9HRYtJL8pM/download "[Download __BoxNebula NGC6309__](https://diversewolken.ddns.net/nextcloud/index.php/s/ffmNCi5wgeRfkms/download)")![SäulenDerSchöpfung](https://diversewolken.ddns.net/nextcloud/index.php/s/9TNKpkfnG6GNZqN/download "[Download __Säulen der Schöpfung__](https://diversewolken.ddns.net/nextcloud/index.php/s/dSPGZjLAk4TbiRa/download)")![ZwergGalaxy](https://diversewolken.ddns.net/nextcloud/index.php/s/jSQqnEd3pyfMksG/download "[Download __Zwerggalaxie__](https://diversewolken.ddns.net/nextcloud/index.php/s/3NNmPRS7FyK2QGi/download)")![Käfernebel](https://diversewolken.ddns.net/nextcloud/index.php/s/zNgFznYprCJQSgX/download "[Download __Käfernebel__](https://diversewolken.ddns.net/nextcloud/index.php/s/AWcdYQYLAcywJiA/download)")

_Hinweis:_ Für die Andromeda-Galaxy sollte das Tool _Zoom out_ zwei mal verwendet werden.

</p>

2. Planet oder Mond

<p style="margin-left:10%">

Fügen Sie einen Planeten oder Mond mit einer geeigneten Farbwahl hinzu.

![Mars](https://diversewolken.ddns.net/nextcloud/index.php/s/xRPy7zWi55j7PDa/download "[__Download: Mars__](https://diversewolken.ddns.net/nextcloud/index.php/s/4z8w6TT8dQ4cgRg/download)") ![Jupiter](https://diversewolken.ddns.net/nextcloud/index.php/s/ojfyyjxKo92aHsQ/download "[__Download: Jupiter__](https://diversewolken.ddns.net/nextcloud/index.php/s/x9rFSDGNzYsXdEe/download)") ![Saturn](https://diversewolken.ddns.net/nextcloud/index.php/s/8BTDmYf5LX4Go4k/download "[__Download: Saturn__](https://diversewolken.ddns.net/nextcloud/index.php/s/F2maPSXLwQaGdpG/download)") ![Mond](https://diversewolken.ddns.net/nextcloud/index.php/s/Nb3MZDLPdwA7LAJ/download "[__Download: Mond__](https://diversewolken.ddns.net/nextcloud/index.php/s/zwAMeE72nLgr6pf/download)")

</p>

3. Speichern Sie ihr Bild (Image -> Save as PNG) auf ihrem PC ab und laden Sie es 

??[hier hoch](https://diversewolken.ddns.net/nextcloud/s/WmRB7yT4BsAM4b2).



