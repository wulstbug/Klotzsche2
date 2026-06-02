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


## Aufgaben LK1 - Nawi 8

@color(Löse die beiden folgenden Aufgaben. Nutze als Name deinen Vornamen und den Anfangsbuchstaben des Nachnamen., blue)

---

1. [Aufgabe-1-Reflexion-Ebener-Spiegel](https://www.geogebra.org/classroom/fcghsuwb)

<p style="margin:5%">

> [![Aufgabe-1-Reflexion-Ebener-Spiegel](https://diversewolken.ddns.net/nextcloud/index.php/s/n8m7YAd9rcxgBB9/download)](https://www.geogebra.org/classroom/fcghsuwb)

</p>

---

2. [Aufgabe-2-Hubble-Hohlspiegel](https://www.geogebra.org/classroom/nkdkja9k)

<p style="margin:5%">

> [![Aufgabe-Konstruktion-2](https://diversewolken.ddns.net/nextcloud/index.php/s/n8m7YAd9rcxgBB9/download)](https://www.geogebra.org/classroom/nkdkja9k)

</p>
