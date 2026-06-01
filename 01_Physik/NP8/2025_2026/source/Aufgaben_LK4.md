<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://www.che.de/wp-content/uploads/board-361516_1920.jpg

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


## Aufgaben LK2 - Nawi 8

@color(Von den folgenden zwei Aufgaben ist __genau eine__ Aufgabe zu lösen., blue)

---

<H4> Konstruktion eines Mikroskops mit Geogebra </H4>

In der folgenden Aufgabe soll die Abbildung an einem Mikroskop konstruiert werden. Ein Mikroskop besteht aus zwei Linsen 1. dem Okular (durch das man mit dem Auge blickt) und dem Objektiv (welches sich nahe des Gegenstandes befindet). 

Nähere Informationen erhältst du dann in der Aufgabe selbst.

[![Moodle](https://upload.wikimedia.org/wikipedia/commons/c/c6/Moodle-logo.svg)<!-- style="margin-left:10%;max-width:300px"-->](https://diversewolken.ddns.net/moodle/mod/quiz/view.php?id=634)

---

<H4> 2. Erstellung eines astronomischen Bildes </H4>

- erstelle ein mehrfarbiges astronomisches Bild aus einem Datensatz für Galaxien und Nebel (siehe unten)

[![Webseite-Bilderstellung](https://diversewolken.ddns.net/nextcloud/index.php/s/9btLqZpm9bpw6PH/download)<!-- style="margin-left:10%;max-width:300px"-->](https://ogy.de/gykl_fits)

     []()

- lege dafür mehrere Farbschichten übereinander

- füge anschließend eine weitere Galaxie, einen Nebel, einen  Planeten oder einen Mond aus der Liste der Planeten/Monde hinzu

- dokumentiere den Entstehungsprozess

- nutze für die Dokumentation entweder Canva, Powerpoint oder ein anderes Programm (z.B. Word)

     | | |
     | [![Powerpoint-Datei](https://upload.wikimedia.org/wikipedia/de/thumb/c/c1/Canva_Logo_2021.svg/250px-Canva_Logo_2021.svg.png)<!-- style="margin-left:10%;max-width=300px"-->](https://www.canva.com/classwork/assignments/DAG-8eSp0xs/activity) | [Powerpoint-Datei](https://diversewolken.ddns.net/nextcloud/index.php/s/rY4Sbg4mNqDd5Cd/download) |

> __Galaxien und Nebel:__

<p style="margin-left:10%">

![Protoplanetarer Nebel](https://diversewolken.ddns.net/nextcloud/index.php/s/PqgERr2xt8i7Med/download "[__Download: Protoplanetarer Nebel Roberts22__](https://diversewolken.ddns.net/nextcloud/index.php/s/z8aNGd9ZH5RReCA/download)") ![Messier17](https://diversewolken.ddns.net/nextcloud/index.php/s/qbFaWHTfAeWd6mT/download "[Download: __Messier17__](https://diversewolken.ddns.net/nextcloud/index.php/s/jEkJ3dx7ksBxFSG/download)")![Download __Andromeda__](https://diversewolken.ddns.net/nextcloud/index.php/s/6g6T2Hx7a6wbtZs/download "[Download __Andromeda__](https://diversewolken.ddns.net/nextcloud/index.php/s/6EAJGojPg2bbJx4/download)") ![Sternenhaufen](https://diversewolken.ddns.net/nextcloud/index.php/s/mc5HffHedeGa2H7/download "[Download __Sternenhaufen M35__](https://diversewolken.ddns.net/nextcloud/index.php/s/SNH69qqnJ97KYf8/download)") ![Sternengeburtsort](https://diversewolken.ddns.net/nextcloud/index.php/s/DgbMbws45onKZwq/download "[Download __Sternengeburtsnebel N11B__](https://diversewolken.ddns.net/nextcloud/index.php/s/GXWMXnSBMGE8yCE/download)") ![Antennengalaxie](https://diversewolken.ddns.net/nextcloud/index.php/s/9tp4AbWfw4TPitH/download "[Download __Antennengalaxy__](https://diversewolken.ddns.net/nextcloud/index.php/s/TR68AnTQMttWxpN/download)") ![BoxNebula_NGC6309](https://diversewolken.ddns.net/nextcloud/index.php/s/YpCrG9HRYtJL8pM/download "[Download __BoxNebula NGC6309__](https://diversewolken.ddns.net/nextcloud/index.php/s/ffmNCi5wgeRfkms/download)")![SäulenDerSchöpfung](https://diversewolken.ddns.net/nextcloud/index.php/s/9TNKpkfnG6GNZqN/download "[Download __Säulen der Schöpfung__](https://diversewolken.ddns.net/nextcloud/index.php/s/dSPGZjLAk4TbiRa/download)")![ZwergGalaxy](https://diversewolken.ddns.net/nextcloud/index.php/s/jSQqnEd3pyfMksG/download "[Download __Zwerggalaxie__](https://diversewolken.ddns.net/nextcloud/index.php/s/3NNmPRS7FyK2QGi/download)")![Käfernebel](https://diversewolken.ddns.net/nextcloud/index.php/s/zNgFznYprCJQSgX/download "[Download __Käfernebel__](https://diversewolken.ddns.net/nextcloud/index.php/s/AWcdYQYLAcywJiA/download)")![Lagoonnebel](https://diversewolken.ddns.net/nextcloud/index.php/s/7ZHPZJ5pDE3EyCM/download "[Download __Lagoon-Nebel__](https://diversewolken.ddns.net/nextcloud/index.php/s/J7BmZgAP2Qn4dQK/download)")

</p>

- Klicke auf Download -> Datei auf den PC herunterladen

- wenn die Datei auf den PC herunter geladen ist, rechtsklick auf die Datei -> Alle Extrahieren -> die FITS Dateien werden auf die Festplatte entpackt

- __achte auf die Hinweisdateien__

---

> Planeten und Monde:

<p style="margin-left:10%">

![Mars](https://diversewolken.ddns.net/nextcloud/index.php/s/xRPy7zWi55j7PDa/download "[__Download: Mars__](https://diversewolken.ddns.net/nextcloud/index.php/s/4z8w6TT8dQ4cgRg/download)") ![Jupiter](https://diversewolken.ddns.net/nextcloud/index.php/s/ojfyyjxKo92aHsQ/download "[__Download: Jupiter__](https://diversewolken.ddns.net/nextcloud/index.php/s/x9rFSDGNzYsXdEe/download)") ![Saturn](https://diversewolken.ddns.net/nextcloud/index.php/s/8BTDmYf5LX4Go4k/download "[__Download: Saturn__](https://diversewolken.ddns.net/nextcloud/index.php/s/F2maPSXLwQaGdpG/download)") ![Mond](https://diversewolken.ddns.net/nextcloud/index.php/s/Nb3MZDLPdwA7LAJ/download "[__Download: Mond__](https://diversewolken.ddns.net/nextcloud/index.php/s/zwAMeE72nLgr6pf/download)")


</p>

> -> [Hier Abgeben Hochladen](https://diversewolken.ddns.net/nextcloud/index.php/s/w2AHSy2oxJGn5NC)