<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp

@style
.lia-effect__circle {
    display: none !important;
}
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 40px;
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
@end

@onload
window.LIA.settings.font_size = 2
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@uhr

<div style="position: fixed; right:50px; top:100px;">

<details>

<summary> Uhrzeit </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=de&size=large&timezone=Europe%2FBerlin" width="100%" height="150" frameborder="0" seamless></iframe> 

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

@timer2

<div style="position: fixed; right:50px; top:300px;">

<details>

<summary> Timer(@0:@1) </summary>

<div style="text-align:left;padding:1em 0;"> 

<iframe width="200" height="90" src="https://webuhr.de/embed/timer/#countdown=00:@0:@1&enabled=0&onzero=0&theme=0&ampm=0&sound=xylophone" frameborder="0" allowfullscreen>

</iframe> 

</div>

</details>

</div>

@end

@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0$\ $=$\ $ 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
    input <= 0.03
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
    input <= 0.2
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

@rangeQuiz0
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:5px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)
    input == 0
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:5px">
@2
</div>
</div>
@end

mode: presentation

-->

# LB 12 Atomvorstellungen

![Atomvorstellungen](https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp)

## 12. 1. Geschichte der Atommodelle


## 12. 2. Entstehung von Spektrallinien




### Übung: Spektrallinien

> 1. In der folgenden Abbildung ist für die _subjektive Methode_ das Linienspektrum einer $He$-Gasentladung dargestellt. Ermitteln Sie für die rote und die orange Spektrallinie die Wellenlänge in der Einheit nm. Ermitteln Sie ebenfalls die Energie der zugehörigen Photonen in der Einheit eV. Notieren Sie Ihre Ergebnisse im Hefter.

<p style='margin-left:10%'>

_Hinweise: Für den folgenden Versuch wurde das Interferenzmuster durch ein Gitter mit 600 vertikalen Spalten pro mm aufgenommen. Der Abstand des Gitters vom Schirm beträgt 39 cm. Der Schirm beginnt im Abstand von 5cm von der Spektrallampe._

![Spektrallinien-He](https://diversewolken.ddns.net/nextcloud/index.php/s/Z4oJjK2DTzYfCbs/download)

</p>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Orange Linie:__

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_o$,573,$\mathrm{nm}$)

@rangeQuiz2($E_{ph-o}$,2.165,$\mathrm{eV}$)

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Rote Linie:__

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_r$,651,$\mathrm{nm}$)

@rangeQuiz2($E_{ph-r}$,1.906,$\mathrm{eV}$)

</p>

</div>

</section>

> 2. Vergleichen Sie die von Ihnen ermittelten Werte mit den in der Formelsammlung angegebenen Spektrallinien für Helium. __Notieren Sie die Tabellenwerte.__

---

> 3. In der folgenden Abbildung ist für die _subjektive Methode_ das Linienspektrum einer $H$-Gasentladung dargestellt. Da sich über die Zeit andere Gase im Glaskörper gesammelt haben, ist hier neben den beiden hauptsächlich sichtbaren Linien (rot, hellblau) ein quasi-kontinuierliches Spektrum sichtbar, welches für diese Auswertung nicht beachtet werden soll. <br> Ermitteln Sie die sichtbaren Spektrallinien von Wasserstoff. Notieren Sie Ihre Ergebnisse im Hefter in Tabellenform. Berechnen Sie die zugehörige Photonenenergie in eV.

<p style='margin-left:10%'>

__Sichtbare Spektrallinien des Wasserstoff__

![Spektrallinien-H](https://diversewolken.ddns.net/nextcloud/index.php/s/9Y6d7636gEFARiH/download)

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Experimentell:__ $\lambda$ in nm

@rangeQuiz2($\lambda_r$,644,$\mathrm{nm}$)

@rangeQuiz2($\lambda_b$,484,$\mathrm{nm}$)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Tabellenwert__ 

@rangeQuiz2($\lambda_r$,656,$\mathrm{nm}$)

@rangeQuiz2($\lambda_b$,486,$\mathrm{nm}$)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Tabellenwert:__ $E_{ph}$ in eV 

@rangeQuiz2($E_{ph-r}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($E_{ph-b}$,2.553,$\mathrm{eV}$)

</div>

</section>


</p>

---


12. 3. Spektrallinien am Wasserstoffatom