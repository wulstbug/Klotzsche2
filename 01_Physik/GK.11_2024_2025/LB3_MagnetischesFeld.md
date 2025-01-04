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

.blue {
    color:blue
}

.green {
    color:darkgreen
}

.red {
    color:darkgreen
}
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@onload
window.LIA.settings.font_size = 2
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

@rangeQuiz20
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left">
@0 = 
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
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
<div style="float:left">
@2
</div>
</div>
@end

@@@ ogy.de/11ph3 deaktivieren: https://ogy.de/del.cvv2y5l7old0u7gamlc1

-->


# Grundkurs Physik 2024/2025 - LB III Das Magnetische Feld

![MagnetischesFeld](https://www.mozaweb.com/de/mozaik3D/FOL/termeszet/foldi_magneses_mezo/960.jpg)

{{1}}
***********
> __Das magnetische Feld__ ist, ebenso wie das elektrische Feld, @color(ein Modell, red) um den Einfluss von @color(magnetischen Kräften im Raum um einen Magneten, blue) darzustellen.
***********

## 1.1 Vergleich von elektrischen und magnetischen Feldern

<p class="newspaper3">

__Name__

<p class="cb">

__Elektrisches Feld__


<p class="cb">

__Magnetisches Feld__

</p>

</p>

</p>

---

<p class="newspaper3">

_Ursache sind_

<p class="cb">

{1}{__elektrische Ladungen Q__}

<p class="cb">

{2}{__Dauermagnete__ und __bewegte elektrische Ladungen (elektrischer Strom)__}

</p>

</p>

</p>

---

<p class="newspaper3">

_Darstellung durch_

<p class="cb">
{{3}}
********
Elektrische Feldlinien

![Dipolfeld](https://diversewolken.ddns.net/nextcloud/index.php/s/RoDMrztJdHLrSyN/download)
********
<p class="cb">
{{4}}
********
Magnetische Feldlinien

![WikimediaMagnetischesFeld](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0c/VFPt_cylindrical_magnet_thumb.svg/1280px-VFPt_cylindrical_magnet_thumb.svg.png)
********
</p>

</p>

</p>

---

<p class="newspaper3">

_Verdeutlicht wird die_

<p class="cb">

{5}{__Wirkung der elektrischen Kraft__ auf eine <span style="color:orange">positive Probeladung</span>.}

<p class="cb">

{6}{__Wirkung der magnetischen Kraft__ auf einen @color(anderen Magneten,orange) oder auf @color(eine bewegte Ladung, orange).}

</p>

</p>

</p>

---

<p class="newspaper3">

_Eigenschaften sind_

<p class="cb">
{{7}}
********
- Feldlinien verlaufen von @color($\oplus$, red) nach @color($\ominus$, blue)

<br>

- elektrischen Kräfte wirken __entlang (d.h. tangetial)__ der Feldlinien

- je dichter die Feldlinien, desto größer die Kraft
********

<p class="cb">

{{8}}
********
- Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, blue)

- magnetische Kräfte mit Hilfe der Feldlinien ableitbar (siehe __Lorentzkraft__)

- je dichter die Feldlinien, desto größer die Kraft

- Feldlinien sind @color(__immer__,red) geschlossen (kein Anfang oder Ende)

- sie verlaufen außerhalb des Magneten von @color(__N__,red)->@color(__S__, blue) und innerhalb von @color(__S__, blue)->@color(__N__,red)
********

</p>

</p>

</p>

---

{{9}}
********

@color(Selbstständiges Arbeiten, blue)

<p style="margin-left:5%">

<br>

@color(__Aufgabe:1.1__ Ergänze diese Übersicht zu magnetischen Feldern durch eine eigene Recherche. Zeichne dazu einige Arten von Magneten und die zugehörigen Felder in deinen Hefter., blue)

<br>

@color(__Aufgabe 1.2.__ Ergänze diese Übersicht mit zwei Beispielen für homogene magnetische Felder. Wiederhole die Definition von __homogen__., blue)

<br>

@color(__Aufgabe 1.3.__ Ergänze diese Übersicht mit Erklärungen zur anziehenden und abstoßenden Kraftwirkung zwischen Magneten., blue)

<br>

<bdi style="color:blue">__Aufgabe 1.4.__ Notiere Stichpunkte zum Erdmagnetfeld. Gehe dabei auf die Lage der magnetischen Pole, das Feldlinienbild und die Funktion als Schutzschild für die Erde ein.</bdi>

<br><br>

@color(Nutze hierfür z.B. folgende Quellen:, blue)

<br>

- [Arten von Magneten](https://www.abi-physik.de/buch/das-magnetfeld/dauer--und-elektromagnete/)

- [Homogene Felder](https://www.abi-physik.de/buch/das-magnetfeld/homogenes-magnetfeld/)

- LB S. 102, 103, 104

</p>

---

********


{{10}}
********
!?[XeniusMagnetismusUnsichtbareKraft](https://www.youtube.com/watch?v=mlt9JcRpzYg)
********

### Aufgaben zur Überprüfung

1. Das Magnetfeld der Erde gleich dem eines/r .. <br>
_Hinweis: Die folgenden Formen der magnetischen Felder solltest du im Hefter haben._

<!-- data-solution-button="off" -->
[( )] Hufeisenmagneten
[(x)] Stabmagneten
[( )] Stromdurchflossenen Leites
[( )] Stromdurchflossenen Spule

---

2. Das hier gezeigte Magnetfeld gehört zu einem/r

![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)

<!-- data-solution-button="off" -->
[(x)] Hufeisenmagneten
[( )] Stabmagneten
[( )] Stromdurchflossenen Leiters
[( )] Stromdurchflossenen Spule

---

3. Welche der folgenden Aussagen über das Erdmagnetfeld ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Der magnetische Nordpol der Erde befindet sich nahe dem geografischen Südpol.
[[ ]] Das Erdmagnetfeld schützt die Erde vor kosmischer Strahlung.
[[x]] Die Stärke des Erdmagnetfelds ist überall auf der Erde gleich.
[[ ]] Die Polarität des Erdmagnetfelds kann sich im Laufe der Zeit umkehren.

---

4. Erkunden Sie, ob auch andere Planeten ein Magnetfeld besitzen.

---

5. Markieren Sie das Magnetfeld eines stromdurchflossenen Leiters.

<!-- data-solution-button="off" -->
[( )] ![Hufeisenmagnet](https://www.abi-physik.de/images/devpages/hufeisenmagnet.png)
[( )] ![Stabmagnet](https://www.abi-physik.de/images/devpages/stabmagnet.png)
[(x)] ![Leiter](https://www.abi-physik.de/images/devpages/leiter.png)
[( )] ![Spule](https://www.abi-physik.de/images/devpages/spule.png)

---

6. Dauermagnete (Permanentmagnete) sind Stoffe, die ihre Umgebung dauerhaft magnetisch beeinflussen. Sie bestehen aus.. (_Vgl. LB S. 102_)

<!-- data-solution-button="off" -->
[[ ]] Magnesium
[[x]] Eisen
[[ ]] Aluminium
[[ ]] Zink
[[ ]] Kupfer
[[ ]] Zinn
[[x]] Cobalt
[[x]] Nickel

---

7. Der magnetische Nordpol der Erde befindet sich in der Nähe des

<!-- data-solution-button="off" -->
[( )] geographischen Nordpols
[(x)] geographischen Südpols
[( )] Nullmeridians
[( )] Äquators

---

8. Durch welche Anordnung könnten die abgebildeten Magnetfelder erzeugt worden sein (siehe LB S. 124/Aufgabe 27).

a)

<!-- data-solution-button="off" -->
[[ ]] Hufeisenmagneten
[[x]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

b)

<!-- data-solution-button="off" -->
[[x]] Hufeisenmagneten
[[ ]] Stabmagneten
[[ ]] Stromdurchflossener Leiter
[[x]] Stromdurchflossene Spule

---

9. Welcher der folgenden Prozesse erzeugt kein Magnetfeld?

<!-- data-solution-button="off" -->
[[ ]] Ein elektrisch geladenes Teilchen bewegt sich mit konstanter Geschwindigkeit.
[[ ]] Ein stromdurchflossener Leiter.
[[x]] Ein statischer elektrischer Dipol.
[[ ]] Eine Spule mit wechselndem Strom.

---

10. Welche Aussage über Magnetfeldlinien ist falsch?

<!-- data-solution-button="off" -->
[[ ]] Magnetfeldlinien sind geschlossene Kurven und haben keinen Anfang und kein Ende.
[[ ]] Magnetfeldlinien verlaufen außerhalb eines Magneten vom Nordpol zum Südpol.
[[x]] Magnetfeldlinien können sich in einem homogenen Magnetfeld überschneiden.
[[ ]] Die Dichte der Magnetfeldlinien gibt die Stärke des Magnetfeldes an.

11. Welche der folgenden Aussagen ist korrekt?

<!-- data-solution-button="off" -->
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist entlang der Leiterachse ausgerichtet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter ist radial nach außen gerichtet.
[[x]] Das Magnetfeld um einen stromdurchflossenen Leiter ist kreisförmig und konzentrisch um den Leiter angeordnet.
[[ ]] Das Magnetfeld um einen stromdurchflossenen Leiter existiert nur, wenn der Strom sinusförmig wechselt.
