<!--
author: Christian Golnik

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


@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0$\ =\ $
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
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
<div style="float:left">
@2
</div>
</div>
@end

mode: presentation

-->

## 2.5 Energiebedarf moderner Gesellschaften

@timer(10,00)

{{0-6}}
***********

__siehe LB S. 31__

{{1}} 
***********
@color(Lies die linke Spalte bis zum Diagramm. Beantworte dann die beiden Fragen auf einem Stichpunktzettel., blue)
***********

{{1-3}}
*************
![Energiebedarf](https://diversewolken.ddns.net/nextcloud/index.php/s/siWycf4txMC7qLm/download "Genutzte __primäre__ Energiequellen der Menschheit (Quelle: LB S. 31)") <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->
*************

{{3}}
*************
![Energiebedarf2](https://diversewolken.ddns.net/nextcloud/index.php/s/bxotwGjptqE73fy/download "Genutzte __primäre__ Energiequellen der Menschheit (LB S.31)") <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->
*************


{{1}}
*************
1. Formuliere zwei Aussagen bezüglich der Gesamtenergie und der erneuerbaren Energie, welche man aus dem Diagramm entnehmen kann.

{{2}}
*************
> - die Nutzung @color(primärer Energiequellen,red) ist im Lauf der letzten 50 Jahre gestiegen, sie hat sich mehr als verdoppelt
>
> - die Menge @color(erneuerbarer Energien [Wasser-Sonne-Wind-Biomasse],red) ist ebenfalls gestiegen
*************


2. Ermittle aus dem Diagramm, den Anteil erneuerbarer Energien (in Prozent von der Gesamtenergie) im Jahr 1960 und vergleiche ihn mit dem Anteil im Jahr 2015.

<p class="newspaper">

{{4}}
*************
> - 1960
>
> $$ \dfrac{0,2\,cm}{2,2\,cm} \cdot 100 \% \approx 10\% $$

<p class="cb">

{{5}}
*************


> - 2010
>
> $$ \dfrac{1,6\,cm}{5,6\,cm} \cdot 100 \% \ \approx 30\% $$

*************

</p>

*************

</p>

*************

***********

{{6}}
***********
<p class="newspaper">

@color(_Diagramm skizzenhaft übernehmen_, blue)

![Energiebedarf2](https://diversewolken.ddns.net/nextcloud/index.php/s/bxotwGjptqE73fy/download "Genutzte __primäre__ Energiequellen der Menschheit (LB S.31)")

<p class="cb">

@color(__siehe Diagramm LB S. 31__, blue)

__Nutzung primärer Energiequellen (1960-2015):__

> - die Nutzung @color(primärer Energiequellen,red) ist im Lauf der letzten 50 Jahre gestiegen, sie hat sich mehr als verdoppelt
>
> - die bereitgestellte Menge @color(erneuerbarer Energien [Wasser-Sonne-Wind-Biomasse],red) ist ebenfalls gestiegen

</p>

</p>

__Anteil erneuerbarer Energien (1960-2015):__

<p class="newspaper">

> - 1960
>
> $$ \dfrac{0,2\,cm}{2,2\,cm} \cdot 100 \% \approx 10\% $$

<p class="cb">

> - 2015
>
> $$ \dfrac{1,6\,cm}{5,6\,cm} \cdot 100 \% \ \approx 30\% $$

</p>

</p>

***********

## 2.6 Die Bereitstellung elektrischer Energie in modernen Gesellschaften

@timer(10,00)

> @color(Elektrische Energie,red) spielt in modernen westlichen Gesellschaften eine wichtige Rolle. Sie wird durch verschiedene Arten von __Kraftwerken__ bereit gestellt. 
>
> Kraftwerke wandeln primäre Energiequellen (Gas, Kohle, Kernbrennstoff, Windenergie, Wasserenergie) in @color(elektrische Energie,red) um

{{1-6}}
**********
__siehe LB S. 37/38__

__Aufgaben:__ 

<i style="color:blue">

1. Übernimm den Merksatz (oben)

---

2. 1. Lies den Text "Die Bedeutung elektrischer Energie" (LB S. 37)

2. 2. Notiere drei Gründe, warum elektrische Energie für moderne Gesellschaften einen große Bedeutung hat

{{2}}
*********
![UmwandlungElektrischerEnergie](https://diversewolken.ddns.net/nextcloud/index.php/s/49i35ds3osncYLc/download)
*********

{{3}}
*********
<p style="text-indent:10%; color:black">

> -> elektrische Energie kann aus vielen primären Energieträgern umgewandelt werden
>
> -> elektrische Energie ist leicht transportabel
>
> -> elektrische Energie lässt sich vor Ort in viele andere Energieformen umwandeln

</p>
*********

---

3. 1. Lies den Text "Bereitstellung elektrischer Energie durch Kraftwerke (S.38).

3. 2. Notiere bespielhaft für drei Kraftwerkstypen den Wirkungsgrad

3. 3. Betrachte die schematische Dartellung verschiedener Kraftwerksformen (S.38/39 unten)

{{4}}
************
![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/Xbf7QmBSmwzN4GK/download)
************

3. 4. Überprüfe und notiere Elemente, welche in beinahe jedem Kraftwerkstyp zum Einsatz kommen

{{5}}
*********
<p style="text-indent:10%; color:black">

> -> in beinahe jedem Kraftwerkstyp (ausgenommen Solarkraftwerk) kommt ein @color(Generator,red) zum Einsatz
>
> -> Generatoren wandeln mechanische Energie(z.B. Rotationsenergie) in elektrische Energie um

</p>
*********

---

</i>

**********


{{6}}
**********

__Gründe für die Nutzung elektrischer Energie als @color(sekundäre Energiequelle , red):__

> -> elektrische Energie kann aus vielen primären Energieträgern umgewandelt werden
>
> -> elektrische Energie ist leicht transportabel
>
> -> elektrische Energie lässt sich vor Ort in viele andere Energieformen umwandeln

__Generatoren als Energiewandler für elektrische Energie:__

> -> in beinahe jedem Kraftwerkstyp (ausgenommen Solarkraftwerk) kommt ein @color(Generator,red) zum Einsatz
>
> -> Generatoren wandeln mechanische Energie(z.B. Rotationsenergie) in elektrische Energie um
**********

## Wie funktioniert ein Generator?

!?[MausStrom](https://www.youtube.com/watch?v=Je22SgH8TCk)
