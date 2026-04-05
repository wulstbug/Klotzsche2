<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

logo: https://diversewolken.ddns.net/nextcloud/index.php/s/42Da3SQjpKcpDR5/download

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


## Absorptionsspektroskopie


### Aufgabe 1: Quiz Regenbogen

__Quiz Regenbogen: Spektral-Farben__

??[Regenbogen-Spektralfarben](https://learningapps.org/692413)

### Aufgabe 2 - Helligkeit von Leuchtenden Objekten

??[Simulation-Schwarzkörperstrahlung](https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_all.html?locale=de)

@color(Schätze mit Hilfe der Simulation die ungefähre Temperatur der Sterne, blue)

<p class="newspaper">

![Sternfärbung](https://diversewolken.ddns.net/nextcloud/index.php/s/dQKqBZmDJPKxD8G/download)

<p class="cb">

<!-- data-solution-button="3" -->
A: [[ 1000 K | 2000 K | 3000 K | (4000 K) | 5000 K | 6000 K | 7000 K | 8000 K | 9000 K | >10000 K ]]

<!-- data-solution-button="3" -->
B: [[ 1000 K | 2000 K | 3000 K | 4000 K | 5000 K | 6000 K | 7000 K | (8000 K) | (9000 K) | (>10000K) ]]

<!-- data-solution-button="3" --><!-- data-solution-button="3" -->
C: [[ 1000 K | (2000 K) | 3000 K | 4000 K | 5000 K | 6000 K | 7000 K | 8000 K | 9000 K | >10000 K ]]

</p>

</p>

### Aufgabe 3 - Erkenne die Elemente

<p style="color:blue">

Wenn das weiße Licht eines Sterns die Atmosphäre eines Planeten durchläuft, so werden einzelne Teile des Farbenspektrums absorbiert.

Analysiere die Absorptionsspektren und ordne die Elemente zu.

1. ![Na](https://diversewolken.ddns.net/nextcloud/index.php/s/X7NQccm7prTcExG/download)

<!-- data-solution-button="3" -->
[[ Natrium ]]


---

2. ![O2](https://diversewolken.ddns.net/nextcloud/index.php/s/dCmpMGaXMw3ikeL/download)

<!-- data-solution-button="3" -->
[[ Sauerstoff ]]


---

3. ![H2](https://diversewolken.ddns.net/nextcloud/index.php/s/g75rrGPjtNMTMFi/download)

<!-- data-solution-button="3" -->
[[ Wasserstoff ]]


---

4. ![N2](https://diversewolken.ddns.net/nextcloud/index.php/s/7cmpM6Ag5arjF9e/download)

<!-- data-solution-button="3" -->
[[ Stickstoff ]]


---

</p>

### Aufgabe 4: Erkenne die Planeten

<p style="color:blue">

Benenne die vom James Webb Telescope aufgenommenen Planeten.

</p>

1. ![Jupiter](https://diversewolken.ddns.net/nextcloud/index.php/s/JxLJdxT5HNbeNQX/download)

<!-- data-solution-button="3" -->
[[ Jupiter ]]

2. ![Saturn](https://diversewolken.ddns.net/nextcloud/index.php/s/bxHecCkgfqoTX3F/download)

<!-- data-solution-button="3" -->
[[ Saturn ]]

3. ![Neptun](https://diversewolken.ddns.net/nextcloud/index.php/s/9sAXacWqpGgoes2/download)

<!-- data-solution-button="3" -->
[[ Neptun ]]

