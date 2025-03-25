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

.red {
    color: red;
}

.blue {
    color: blue;
}

.darkgreen {
    color: darkgreen;
}

.orange {
    color: orange;
}

.purple {
    color: purple;
}

@end

@color
<bdi style="color:@1">@0</bdi>
@end


@rangeQuiz2

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

@onload
window.LIA.settings.font_size = 2
@end

-->


# LB6 - Magnetisches Feld

__Übungsaufgaben zur LK__

![DreiFingerRegel](https://diversewolken.ddns.net/nextcloud/index.php/s/mnjjesXkkPMEGc8/download)

---

Übungen zur [Elektronenröhre](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#16) und [Wolkenkondensator](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#19).

---

Übungen zur [Berechnung an Kondensatoren](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#42) und zum Kondensator in realen Schaltkreisen [Aufgabe I](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#50) und [Aufgabe II](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche2/2024_2025/01_Physik/LK.11_2024_2025/Script_SuS_LB5_ElektrischesFeld.md#52)



---

---

![MagnetischesFeld](https://www.mozaweb.com/de/mozaik3D/FOL/termeszet/foldi_magneses_mezo/960.jpg)

{{1}}
***********
> __Das magnetische Feld__ ist, ebenso wie das elektrische Feld, @color(ein Modell, red) um den Einfluss von @color(magnetischen Kräften im Raum um einen Magneten, blue) darzustellen.
***********


## 6.1 Vergleich von elektrischen und magnetischen Feldern

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

{2}{__@color(Dauermagnete,red)__ und __@color(bewegte,red) elektrische Ladungen (elektrischer Strom)__}

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

- LB Duden S. 277-279

</p>

---

********


{{10}}
********
!?[XeniusMagnetismusUnsichtbareKraft](https://www.youtube.com/watch?v=mlt9JcRpzYg)
********

{{11}}
********
<p class="newspaper3">

_Arten von Feldern_

<p class="cb">

homogenes Feld (im Plattenkondensator)

![HomogenesFeld](https://diversewolken.ddns.net/nextcloud/index.php/s/fpKSpwGykqjMJZP/download)


<p class="cb">

homogenes Feld (im Inneren eines Hufeisenmagneten)

![HomogenesFeld](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-spule.png)

homogenes Feld (im Inneren einer Spule)

![HomogenesFeldHufeisenmagnet](https://www.abi-physik.de/images/devpages/homogenes-magnetfeld-1.png)

</p>

</p>

</p>

---
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

8. Durch welche Anordnung könnten die abgebildeten Magnetfelder erzeugt worden sein.

![GK_Duden_S124_A20](https://diversewolken.ddns.net/nextcloud/index.php/s/gDybkgMkALZHmoq/download)

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


## Demonstrationsexperiment: Kräfte auf bewegte elektrische Ladungen in Magnetfeldern

![FotoLorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/mLFceeEL2jP7BDC/download)

## 6.2. Hand-Regel zur Richtungsbestimmung der Lorentzkraft

!?[HandRegel](https://www.youtube.com/watch?v=snM3g4zWeNw)

__Bemerkungen zur Lorentzkraft:__

??[Lorentzkraft_LearningApps](https://learningapps.org/4454537)

_Bitte schau dir zunächst dieses kleine Quiz zur Richtungsbestimmung der Lorentz-Kraft an._

      [QuizZurLorentzkraftRichtung](https://www.leifiphysik.de/elektrizitaetslehre/bewegte-ladungen-feldern/aufgabe/quiz-zu-bewegten-ladungen-im-magnetfeld)

      _Hinweis: Die magnetischen Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, green)._

## 6.3 Berechnung des magnetischen Feldes - Die magnetische Flussdichte B

<p class="newspaper">

__Elektrisches Feld__

<p class="cb">

__Magnetisches Feld__

</p>

</p>

---

<p class="newspaper">

{{1}}
********

Die elektrische Feldstärke $E$ berechnet sich aus der Kraft $F$ auf eine elektrische Ladung $Q$.

$$ \boxed{E = \frac{F_{el}}{Q}} $$

- $F$: Elektrische Kraft [Newton, $N$]
- $Q$: Ladung im Feld [Coulomb, $C$]

> Hinweis: Das elektrische Feld ist eine vektorielle Größe $\vec{E}$, ebenso wie die Kraft $\vec{F_{el}}$. Kraft und Feld wirken entlang einer Linie.

********

<p class="cb">

{{2}}
********

Die __magnetische Flussdichte__ $B$ beschreibt die Stärke und Richtung des magnetischen Feldes in einem Punkt. Sie wird definiert durch die Kraft auf eine bewegte Ladung oder einen stromdurchflossenen Leiter:

$$ \boxed{B = \frac{F}{I \cdot l}}$$

- $F$: Magnetische Kraft [Newton, $N$]
- $I$: Stromstärke [Ampere, $A$]
- $l$: Leiterlänge [Meter, $m$]

> Hinweis: Die magnetische Flussdichte ist eine vektorielle Größe ($\vec{B}$), ebenso wie die Lorentzkraft $\vec{F_L}$. Die Richtungen von $\vec{B}$ bzw. $\vec{F}$ ergeben sich aus der Handregel.

********

</p>

</p>

---

{{3}}
********
<p class="newspaper">

__Einheit__: $$\Big[\dfrac{N}{C}=\dfrac{V}{m}\Big]$$

<p class="cb">

__Einheit__: [1 Tesla = 1 T]

$$\Big[T=\dfrac{N}{A \cdot m}\Big]$$

</p>

</p>

---
********


### 6.3.2 Übung: Berechnung der magnetischen Flussdichte

#### Aufgabe 6.3.1
Ein gerader Leiter mit einer Länge von 2 m wird von einem Strom von 5 A durchflossen. Er befindet sich in einem Magnetfeld mit einer Flussdichte $B$. Die magnetische Kraft auf den Leiter beträgt 0,5 N. Berechne $B$!

@rangeQuiz2(B, 0.05, T)

#### Aufgabe 6.3.2
Ein stromdurchflossener Leiter (Länge $ℓ = 1,5 \, m$, Stromstärke $I = 3 \, A$) befindet sich in einem Magnetfeld mit $B = 0,2 \, T$. Berechne die magnetische Kraft $F$ auf den Leiter.

@rangeQuiz2(F, 0.9, N)

#### Aufgabe 6.3.3
Ein Leiter der Länge $ℓ = 3 \, m$ und Stromstärke $I = 2 \, A$ erfährt eine magnetische Kraft von $F = 0,6 \, N$. Berechne die magnetische Flussdichte $B$.

@rangeQuiz2(B, 0.1, T)

#### Aufgabe 6.3.4 

__Analyse von Änderungen__

Ein stromdurchflossener Leiter befindet sich in einem Magnetfeld. Die Stromstärke $I$ wird verdoppelt, während die Leiterlänge $ℓ$ und die magnetische Flussdichte $B$ unverändert bleiben. Wie ändert sich die magnetische Kraft $F$?

<!-- data-solution-button="off" -->
[[ ]] Sie bleibt gleich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie halbiert sich.  
[[ ]] Sie vervierfacht sich. 

---

<!-- data-solution-button="off" -->
Die magnetische Flussdichte $B$ wird auf das Doppelte erhöht, während Stromstärke $I$ und Leiterlänge $ℓ$ konstant bleiben. Was passiert mit der magnetischen Kraft $F$?

[[ ]] Sie bleibt gleich.  
[[ ]] Sie halbiert sich.  
[[x]] Sie verdoppelt sich.  
[[ ]] Sie vervierfacht sich.  



## 6.4. Berechnungen der magnetischen Flussdichte B in einer langen Spule

<p class="newspaper">

__Magnetisches Feld__

![FeldInSpule](https://diversewolken.ddns.net/nextcloud/index.php/s/z7CNJzqkxjf4bf7/download)

<p class="cb">

__Elektrisches Feld__

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

</p>

</p>

---



{{1}}
********

<p class="newspaper">

Die magnetische Flussdichte $B$ innerhalb einer __langen, stromdurchflossenen Spule__ wird durch folgende Formel beschrieben:

$$
\boxed{B = \mu_0 \cdot \mu_r \cdot \frac{N\cdot I}{ℓ}}
$$

- $B$: Magnetische Flussdichte [ Tesla, $T$]
- $\mu_0$: Magnetische Feldkonstante $\boxed{\mu_0 = 1,26 \cdot 10^{-6} \frac{V \cdot s}{A \cdot m}}$
- $\mu_r$: Magnetische Permeabilität des Mediums [einheitenlos -> FS S.54]
- $N$: Anzahl der Windungen der Spule
- $ℓ$: Länge der Spule [Meter, $m$]
- $I$: Stromstärke [Ampere, $A$]

<p class="cb">

{{2}}
********

Die elektrische Feldstärke E innerhalb eines Plattenkondensators wird durch folgende Formel beschrieben:

$$ \boxed{E = \dfrac{U}{d}} $$

- $U$: Spannung zwischen den Platten $\big[ V \big]$ 
- $d$: Abstand der Platten $\big[ m \big]$ 

********

</p>

</p>

********

### Aufgaben zur B-Feld Berechnung an Spulen

<bdi style="color:blue">__Löse die folgenden Aufgaben, indem du die gegebene Formel zur _langen Spule_ anwendest__.</bdi>

---

__Aufgabe 6.4.1 __ 

Eine Spule hat $N = 800$ Windungen und eine Länge von $ℓ = 0,4 \, m$. Sie wird von einem Strom mit $I = 3 \, A$ durchflossen. Die Spule ist luftgefüllt ($\mu_r = 1$). Berechne die magnetische Flussdichte $B$ im Inneren der Spule.  

@rangeQuiz2(B, 0.00754, T)

---

__Aufgabe 6.4.2__

Eine Spule mit $N = 500$ Windungen und $ℓ = 0,5 \, m$ erzeugt eine magnetische Flussdichte von $B = 2,51 \, mT$. Berechne die Stromstärke $I$, die durch die Spule fließt.  

@rangeQuiz2(I, 2, A)

__Aufgabe 6.4.3__  

Eine Spule hat $N = 1000$ Windungen und eine Länge von $ℓ = 1 \, m$. Der Strom beträgt $I = 4 \, A$. Wie verändert sich die magnetische Flussdichte $B$, wenn: 

1. Die Anzahl der Windungen $N$ verdoppelt wird?  
2. Der Strom $I$ halbiert wird?  
3. Die Länge der Spule $ℓ$ verdreifacht wird?

<!-- data-solution-button="off" -->
[[x]] 1. Verdoppelt sich, 2. halbiert sich, 3. verringert sich auf ein Drittel.  
[[ ]] 1. Verdoppelt sich, 2. bleibt gleich, 3. verringert sich auf die Hälfte.  
[[ ]] 1. Bleibt gleich, 2. halbiert sich, 3. verringert sich auf ein Viertel.  
[[ ]] 1. Verringert sich, 2. bleibt gleich, 3. bleibt gleich.

__Aufgabe 6.4.4__

Eine luftgefüllte Spule hat $N = 1000$ Windungen, $ℓ = 0,8 \, m$ und $I = 2 \, A$. Im Innenraum der Spule wird ein Material mit einer unbekannten relativen Permeabilität $\mu_r$ ersetzt, wodurch die magnetische Flussdichte $B$ auf $1,7 \, T$ ansteigt. Berechne $\mu_r$.  

@rangeQuiz2($\mu_r$, 539.7, -)

Um welchen ferromagnetischen Stoff könnte es sich handeln?

<!-- data-solution-button="off" -->
[[Eisen]]

__Aufgabe 6.4.5__

Die magnetische Flussdichte $B$ in einer luftgefüllten Spule beträgt $1,26 \, mT$. Die Spule hat $N = 400$ Windungen und eine Länge von $ℓ = 0,5 \, m$. Berechne den Strom $I$, der durch die Spule fließt?  

@rangeQuiz2(I, 1.25, A)


### Übungen zum magnetischen Feld allgemein

__Grundwissen Magnetismus__

??[LueckentextMagnetismus](https://learningapps.org/1319776)

__Grundwissen magnetisches Feld__

??[LueckentextMagnetfeld](https://learningapps.org/35523603)

__Fragen zu magnetischen Experimenten__

??[MagnetischeExperimente](https://www.leifiphysik.de/elektrizitaetslehre/permanentmagnetismus/aufgabe/quiz-zu-magnetischen-eigenschaften)


## 6.5 Materie im magnetischen und elektrischen Feld

<p class="newspaper">

__Magnetisches Feld__

<p class="cb">

__Elektrisches Feld__

</p>

</p>

---

Wird ein __Stoff (d.h. Materie)__ in ein magnetisches oder elektrisches Feld eingefügt, so verändert der Stoff die Stärke des Feldes, beschrieben durch 

<p class="newspaper">

die @color(magnetische Permeabilität $\mu_r$, orange) (-> FS. S 54).

<p class="cb">

die @color(Dielektrizitätszahl $\varepsilon_r$, orange) (-> FS. S 54).

</p>

</p>

---

__Beispiele:__

<p class="newspaper">

Cobalt: $\mu_r \approx 80-200$

Eisen: $\mu_r \approx 250-680$

Nickel: $\mu_r \approx 280-2500$

<p class="cb">

Glas: $\varepsilon_r \approx 5-16$

Bariumtitanat: $\varepsilon_r \approx 100-1000$

Wasser: $\varepsilon_r \approx 81$

</p>

</p>

---

__In beiden Beispielen__ richten sich elementare Strukturen des Material im umliegenden Feld aus.

<p class="newspaper">

@color(Elementar,red)@color(magnete,green) richten sich aus (__Magnetisierung__)

![ElementarMagnete](https://diversewolken.ddns.net/nextcloud/index.php/s/7H9rDQfp9fsAixS/download)

<p class="cb">

@color(Elementare,red) @color(Dipole, green) richten sich aus (__Polarisierung__)

![ElementareDipole](https://diversewolken.ddns.net/nextcloud/index.php/s/XfwLBXEkJSMJPTL/download)

</p>

</p>

---

__Unterschied:__

Während ferromagnetische Stoffe (Eisen, Cobalt, Nickel) das magnetische Feld __verstärken__, wird das elektrische Feld durch ein Dielektrikum (z.B. Glas, Wasser) __geschwächt/gedämpft__.

### Aufgabe zum magnetischen Feld

1. Eine Spule ist 9cm lang, hat 1500 Windungen und wird von einem Strom der Stärke 1,52 A durchflossen. Im Innern der Spule wird die magnetische Flussdichte 2,54 T gemessen.<br> Weise rechnerisch nach, dass sich im Innern der Spule nicht ausschließlich Luft befindet.

<details style="margin-left:10%">

<summary> Hilfe: Hinweis Zur Lösung</summary>

Ermitteln Sie die magnetische Flussdichte im Inneren der Spule unter der Annahme, dass diese mit Luft gefüllt ist. Vergleichen Sie Ihr Ergebnis mit der Angabe aus der Aufgabe und schlussfolgern Sie auf das vorhandene $\mu_r$.

</details>

<details style="margin-left:10%">

<summary> Rechenweg </summary>

![Abi21_Lsg2.1_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/4dsX4QKj4FgWz6q/download)

</details>

<details style="margin-left:10%">

<summary> Begründung </summary>

![Abi21_Lsg2.1_Begründung](https://diversewolken.ddns.net/nextcloud/index.php/s/som5GarSYN8yHPR/download)

</details>

<details style="margin-left:10%">

<summary> Alternativer Lösungsweg </summary>

Stelle die Formel für $B$ nach $\mu_r$ um, nutze für für B=2,54T und zeige, dass $\mu_r > 1$ gilt.

Hier ist: $\mu_r \approx 85$ 

</details>


---

2. Eine andere Spule hat 50 Windungen, ist 20 cm lang und ist ausschließlich mit Luft gefüllt. Die Flussdichte im Inneren der Spule beträgt 0,63 mT. Gib die Stromstärke an. <br> Die Spule wird nun auf 40 cm gedehnt, dabei ändert sich die Flussdichte im Inneren der Spule, Stromstärke und Windungszahl bleiben konstant.<br> Zeiche den Graphen $B = B(ℓ)$ für das Intervall 20cm bis 40cm.

@rangeQuiz2($\hspace{1cm}$ $I$, 2, $A$)

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zur Stromstärke</summary>

Nutzen Sie die Formel zur Berechnung der magnetischen Flussdichte und ermitteln Sie den fehlenden Wert der elektrischen Stromstärke.

</details>

<details style="margin-left:10%">

<summary> Rechenweg Stromstärke </summary>

![Abi21_Lsg2.2_Rechnung](https://diversewolken.ddns.net/nextcloud/index.php/s/Xd5nS692Wwd97cD/download)

</details>

<details style="margin-left:10%">

<summary> Hilfe: Hinweis zum Graph</summary>

Nutze Sie die Formel für die magnetische Flussdichte, ermittlen Sie die Funktion $B(ℓ)$, setzen Sie die gegebenen Werten ein und erstellen Sie eine Datentabelle | $ℓ$ | $B(ℓ)$ | für den Bereich 20cm bis 40 cm.

</details>

<details style="margin-left:10%">

<summary> Berechnungen für den Graph $B(ℓ)$ </summary>

![Abi21_Lsg2.2_Berechnung_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/mddY9WFHAT59ofx/download)

</details>

<details style="margin-left:10%">

<summary> Datentabelle und Graph $B(ℓ)$ </summary>

<p class="newspaper">

<!-- data-type="none" -->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |

<p class="cb">

<!--
     data-show
     data-title=""
     data-type="line"
     data-xlabel="ℓ in m"
     data-ylabel="B in mT"
-->
| $ℓ$ in m | $B(ℓ)$ in mT |
| :---: | :---: |
| 0.2 | 0.63 |
| 0.25 | 0.50 |
| 0.3 | 0.42 |
| 0.35 | 0.36 |
| 0.4 | 0.31 |


</p>

</p>

</details>


---

3. Es wird eine lange Spule der Länge $l = 21cm$ betrachtet. Fließt durch die Spule eine Stromstärke von 2A so erhällt man eine magnetische Flussdicht von $30\,mT$. Fügt man in die Spule einen ferromagnetischen Kern, so erhöht sich die magnetische Flussdichte auf den Wert $2,4\,T$.

3. 1. Nennen Sie ein Material aus welchem der ferromagnetische Kern bestehen könnte. Begründen Sie Ihre Aussage. 

     <!-- data-solution-button="off" -->
     [[ Cobalt ]]

<details style="margin-left:10%">

<summary> Begründung </summary>

Ohne Ferromagnetikum ist die magnetische Flussdichte $0,03 T$ und mit Ferromagnetikum erhöht sich die Flussdichte um das 80-fache auf $2,4 T$. Der Wert für $\mu_r$ muss demzufolge 80 betragen und dafür kommt aus der FS S. 54 nur Cobalt in Frage.

</details>

3. 2. Ermitteln Sie die Anzahl der Windungen der Spule.

     <!-- data-solution-button="off" -->
     [[ 2500 ]]

<details style="margin-left:10%">

<summary> Lösung </summary>

Formel für magnetische Flussdichte im Inneren einer Spule nutzen und nach $N$ auflösen.

</details>

3. 3. __Partnerarbeit__ Geben Sie zwei Möglichkeiten an, mit der man die magnetische Flussdichte der Spule(inklusive Kern) verdoppeln kann.

<details style="margin-left:10%">

<summary> Möglichkeiten </summary>

- Stromstärke verdoppeln
- Windungszahl verdoppeln
- Länge der Spule halbieren
- Ferromagnetikum mit $\mu_r=2$ gibt es laut Tabelle nicht

</details>

3. 4. __Partnerarbeit__ Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht.

<details style="margin-left:10%">

<summary> Lösungen </summary>

Ein ferromagnetischer Stoff hat mikroskopische magnetische Elemente, genannt @color(Elementarmagnete, red). Diese sind im Normalzustand des Ferromagnetikums @color(ungeordnet, red). Unter dem Einluss eines @color(äußeren Feldes, red) ordnen sich Elementarmagnete mit Ihren Polen entlang der Feldlinien des äußeren Feldes, man nennt das @color(Magnetisierung, red). <br>
Die geordneten Elementarmagnete verstärken mit ihren ausgerichteten Elementarmagneten das äußere Feld

</details>


### KI-Aufgabe zu ferromagnetischen Stoffen

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Prompt Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Ferromagnetikum-Aufgabe:__<br> Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht.
<div class="container" style="margin-left:10%">
    __Prompt__ <br>
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Beschreiben Sie die Vorgänge, welche beim Einfügen eines ferromagnetischen Stoffes in ein äußeres Magnetfeld auf mikroskopischer Ebene im Ferromagnetikum ablaufen. Erklären Sie auch, warum sich die magnetische Flussdichte bei einem geeigneten Material erhöht. Bitte warte auf meine Antwort und bewerte diese. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Bewerte meine Antwort auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
</div>

<script input="submit" style="margin-left:10%"  default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

??[OpenWebUI](https://subtle-corgi-firmly.ngrok-free.app)

