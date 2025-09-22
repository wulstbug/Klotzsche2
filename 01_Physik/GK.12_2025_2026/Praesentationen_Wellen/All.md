<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://cmscollege.ac.in/wp-content/uploads/2024/01/physics_image.webp

import: https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/settings.md

@style
.lia-slide__footer {
      display: none !important;
}
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
    display: block;
}

@end

mode: presentation

-->

### 6. 3. Darstellung der Wellenausbreitung mit Wellenfront und Wellennormale

Zur Darstellung der Ausbreitung von Wellen nutzen man __Wellenfronten__ und @color(__Wellennormale__,red)

<p class="newspaper">

{{1}}
************
![WellenfrontWellenNormale](https://diversewolken.ddns.net/nextcloud/index.php/s/sPE2gzAdfqJqdjk/download "Links: Kreisförmige Wellenfront (z.B. Steinwurf in Wasser) | Rechts: Ebene Welle (z.B. Licht)")
************

<p class="cb">

{{4}}
*****************
__Die Wellenfronten__ sind Stellen maximaler Auslenkung (Wellenberge). Ihr Abstand voneinander ist gleich der Wellenlänge $\lambda$.

@color(Die Wellennormale, red) steht immer senkrecht auf der Wellenfront und gibt die Ausbreitungsrichtung der Welle an.
*****************

</p>

</p>

---

<p class="newspaper">

{{2}}
************
Kreisförmige Wellenfront (z.B. Steinwurf ins Wasser)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+4+668+0.00390625%0As+2+257+265+0+0.233333+0+10+100+1+0%0A)
************

<p class="cb">

{{3}}
************

Ebene Welle (z.B. Lichtausbreitung)

??[Fallstad-Kugelwelle](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+0+569+0.048828125%0AS+2+0+1+511+1+0+0.466666+0+10+100+1+0%0A)
************

</p>

</p>

### 6. 4. Huygens'sche Prinzip

> Jeder Punkt einer Wellenfront ist seinerseits wieder Ausgangspunkt für @color(kreis- bzw. kugelförmige Elementarwellen, red)

{{1}}
*************
![Huygernssches-Prinzip](https://diversewolken.ddns.net/nextcloud/index.php/s/zE2kb4mDwinM5M2/download)


-> [Simulation-Ausbreitung-Kreiswelle-EbeneWelle](https://www.leifiphysik.de/mechanik/mechanische-wellen/ausblick/huygenssches-prinzip-zur-beschreibung-von-mechanischen-wellen)
*************

### 6. 5. Reflexion

__Definition:__ Trifft eine Welle auf eine ebene Oberfläche, dann wird sie __reflektiert__. Es gilt das __Reflexionsgesetz__:

{{1}}
**********
<p class="newspaper">

> 1. Bei der Reflexion von Wellen sind der Einfallswinkel $\alpha$ und der @color(Reflexionswinkel $\alpha'$, red) gleich groß. 
>
> 2. Die Wellennormalen der einfallenden und reflektierten Wellen liegen in einer Ebene.

<p class="cb">

![Reflexion_Welle](https://diversewolken.ddns.net/nextcloud/index.php/s/bkBpwMGem3rXEx6/download)

</p>

</p>
**********

{{2}}
**********
??[Fendt-Reflexion](https://www.walter-fendt.de/html5/phde/refractionhuygens_de.htm)
**********


### 6. 6. Brechung


__Definition:__ Trifft eine Welle unter einem Einfallswinkel $\alpha\neq 0$ auf eine @color(__ebene Grenzfläche__, darkgreen) zweier Stoffe, in denen sie sich mit unterschiedlicher @color(Geschwindigkeit, red) ausbreitet, dann ändert sie ihre Ausbreitungsrichtung. Sie wird @color(gebrochen, red). Es gilt das __Brechungsgesetz__:

---

{{1}}
**********
<p class="newspaper">

Beim Übergang von einem Stoff (1) in einen anderen Stoff (2) gilt das __Brechungsgesetz__.

$$\boxed{\dfrac{\sin\alpha}{\sin\beta} = \dfrac{v_1}{v_2}}$$

wobei

<p style="margin-left:5%">

     $\alpha$ .. Einfallswinkel

     $\beta$ .. Brechungswinkel

     $v_1,\,v_2$ .. Ausbreitungsgeschwindigkeiten

</p>

<p class="cb">

![Brechung_Welle](https://diversewolken.ddns.net/nextcloud/index.php/s/3awXew9HRi54nyd/download)

</p>

</p>
**********

{{2}}
**********
??[Fendt-Reflexion](https://www.walter-fendt.de/html5/phde/refractionhuygens_de.htm)
**********

### 6. 7. Beugung

Definition: Trifft eine Welle auf einen Spalt oder eine Kante, so sind die betreffenden Stellen nach _Huygens Prinzip_ Ausgangspunkt von Elementarwellen. Damit breitet sich eine Welle auch in den __Schattenraum__ aus.

---

<p class="newspaper3">

{{1}}
********
![Welle-Beugung](https://diversewolken.ddns.net/nextcloud/index.php/s/M9eEFxFCjRATLt2/download)
********

<p class="cb">

{{2}}
********
__Kante:__

??[Simulation-Kante](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+489+1.5625e-8%0Aw+0+252+131+507+131%0AS+2+0+1+511+1+0+1.399998+0+10+100+1+0%0A)
********

<p class="cb">

{{3}}
********
__Spalt:__

??[Simulation-Spalt](https://www.falstad.com/ripple/Ripple.html?rol=$+3+512+64+0+1+578+1.5625e-8%0AS+2+0+1+511+1+0+2.2166635+0+10+100+1+0%0A203+0+-57+145+577+145+1+20+10%0A)
********

</p>

</p>

</p>

### 6. 8. Interferenz