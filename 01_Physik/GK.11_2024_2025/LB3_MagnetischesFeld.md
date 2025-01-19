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


## 1.2 Berechnungen des magnetischen Feldes - Die magnetische Flussdichte B

<p class="newspaper">

__Magnetisches Feld__

<p class="cb">

__Elektrisches Feld__

</p>

</p>

---

{{1}}
********
<p class="newspaper">

Die __magnetische Flussdichte__ $B$ beschreibt die Stärke und Richtung des magnetischen Feldes in einem Punkt. Sie wird definiert durch die Kraft auf eine bewegte Ladung oder einen stromdurchflossenen Leiter:

$$ \boxed{B = \frac{F}{I \cdot l}}$$

- $F$: Magnetische Kraft [Newton, $N$]
- $I$: Stromstärke [Ampere, $A$]
- $l$: Leiterlänge [Meter, $m$]

<p class="cb">

Die elektrische Feldstärke $E$ berechnet sich aus der Kraft $F$ auf eine elektrische Ladung $Q$.

$$ \boxed{E = \frac{F}{Q}} $$

- $F$: Elektrische Kraft [Newton, $N$]
- $Q$: Ladung im Feld [Coulomb, $C$]


</p>

</p>

---
********

{{2}}
********
<p class="newspaper">

__Einheit__: [1 Tesla = 1 T]

$$\Big[T=\dfrac{N}{A \cdot m}\Big]$$

<p class="cb">

__Einheit__: $$\Big[\dfrac{N}{C}=\dfrac{V}{m}\Big]$$

</p>

</p>

---
********


### 1.2.2 Übung: Berechnung der magnetischen Flussdichte

<bdi style="color:blue">__Löse die folgenden Aufgaben, indem du die gegebene Formel anwendest__.</bdi>

#### Aufgabe 1.2.1
Ein gerader Leiter mit einer Länge von 2 m wird von einem Strom von 5 A durchflossen. Er befindet sich in einem Magnetfeld mit einer Flussdichte $B$. Die magnetische Kraft auf den Leiter beträgt 0,5 N. Berechne $B$!

@rangeQuiz2(B, 0.05, T)

#### Aufgabe 1.2.2
Ein stromdurchflossener Leiter (Länge $ℓ = 1,5 \, m$, Stromstärke $I = 3 \, A$) befindet sich in einem Magnetfeld mit $B = 0,2 \, T$. Berechne die magnetische Kraft $F$ auf den Leiter.

@rangeQuiz2(F, 0.9, N)


#### Aufgabe 1.2.3
Ein Leiter der Länge $ℓ = 3 \, m$ und Stromstärke $I = 2 \, A$ erfährt eine magnetische Kraft von $F = 0,6 \, N$. Berechne die magnetische Flussdichte $B$.

@rangeQuiz2(B, 0.1, T)

#### Aufgabe 1.2.4 

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



## 1.3 Berechnungen der magnetischen Flussdichte B in einer langen Spule

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


#### Aufgabe 1.3.1  
Eine Spule hat $N = 800$ Windungen und eine Länge von $ℓ = 0,4 \, m$. Sie wird von einem Strom mit $I = 3 \, A$ durchflossen. Die Spule ist luftgefüllt ($\mu_r = 1$). Berechne die magnetische Flussdichte $B$ im Inneren der Spule.  

@rangeQuiz2(B, 0.00754, T)

#### Aufgabe 1.3.2  
Eine Spule mit $N = 500$ Windungen und $ℓ = 0,5 \, m$ erzeugt eine magnetische Flussdichte von $B = 2,51 \, mT$. Berechne die Stromstärke $I$, die durch die Spule fließt.  

@rangeQuiz2(I, 2, A)

#### Aufgabe 1.3.3  

Eine Spule hat $N = 1000$ Windungen und eine Länge von $ℓ = 1 \, m$. Der Strom beträgt $I = 4 \, A$. Wie verändert sich die magnetische Flussdichte $B$, wenn: 

1. Die Anzahl der Windungen $N$ verdoppelt wird?  
2. Der Strom $I$ halbiert wird?  
3. Die Länge der Spule $ℓ$ verdreifacht wird?

<!-- data-solution-button="off" -->
[[x]] 1. Verdoppelt sich, 2. halbiert sich, 3. verringert sich auf ein Drittel.  
[[ ]] 1. Verdoppelt sich, 2. bleibt gleich, 3. verringert sich auf die Hälfte.  
[[ ]] 1. Bleibt gleich, 2. halbiert sich, 3. verringert sich auf ein Viertel.  
[[ ]] 1. Verringert sich, 2. bleibt gleich, 3. bleibt gleich.

#### Aufgabe 1.3.4  

Eine luftgefüllte Spule hat $N = 1000$ Windungen, $ℓ = 0,8 \, m$ und $I = 2 \, A$. Im Innenraum der Spule wird ein Material mit einer unbekannten relativen Permeabilität $\mu_r$ ersetzt, wodurch die magnetische Flussdichte $B$ auf $1,7 \, T$ ansteigt. Berechne $\mu_r$.  

@rangeQuiz2($\mu_r$, 539.7, -)

Um welchen ferromagnetischen Stoff könnte es sich handeln?

<!-- data-solution-button="off" -->
[[Eisen]]

#### Aufgabe 1.3.5

Die magnetische Flussdichte $B$ in einer luftgefüllten Spule beträgt $1,26 \, mT$. Die Spule hat $N = 400$ Windungen und eine Länge von $ℓ = 0,5 \, m$. Berechne den Strom $I$, der durch die Spule fließt?  

@rangeQuiz2(I, 1.25, A)


### Übungen zum magnetischen Feld allgemein

@timer(15,00)

<br>

<br>

<br>

__Grundwissen Magnetismus__

??[LueckentextMagnetismus](https://learningapps.org/1319776)

__Grundwissen magnetisches Feld__

??[LueckentextMagnetfeld](https://learningapps.org/35523603)

__Fragen zu magnetischen Experimenten__

??[MagnetischeExperimente](https://www.leifiphysik.de/elektrizitaetslehre/permanentmagnetismus/aufgabe/quiz-zu-magnetischen-eigenschaften)

## 1.4 Schülerexperiment: Messungen der magnetischen Flussdichte

__Teil 1: Bestimmung der magnetischen Flussdichte des Erdmagnetfeldes__

> Aufgabe: Bestimme mit Hilfe des Magnetfeldsensors an dem Cassy-Gerät die magnetische Flussdichte $B_{Erde} des Erdmagnetfeldes.

__Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$__

> Aufgabe: Bestimme die magnetische Feldkonstante $\mu_0$ mit Hilfe der Messung der magnetischen Flussdichte B an einer Spule.

@color(Führe die beiden Messungen durch. Erstelle jeweils ein Kurzprotokoll, blue).

_optional (min. 15min)_

__Teil 3: Überprüfung der Proportionalität von $B$ ~ $N$__

> Aufgabe: Überprüfe experimentell die Proportionalität der magnetischen Flussdichte $B$ und der Windungszahl $N$


### Experiment Teil 1: Erdmagnetfeld

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__1.1 Vorbereitung:__

> - recherchiere im Internet die Stärke der magnetischen Flussdichte $B_{Erde}$ des Erdmagnetfeldes in Deutschland
>
> - notiere den Wert und die Quelle
>
> $$ B_{Erde} = ... $$
>
> - erhalte von der Lehrkraft einen Magnetfeldsensor und ein Cassy-Messgerät
>
> - schließe de Magnetfeldsensor an das Cassy-Messgerät an und lass dir die aktuelle magnetische Flussdichte B anzeigen
>
> - wechsle im Menu zu den Einstellungen von B und
>
>      - wähle als Messmethode tangential
>
>      - wähle als Messbereich 0 - 10 mT

__1.2 Durchführung:__

> - bestimme mit dem Cassy-Messgerät die natürliche magnetische Feldstärke an zwei Punkten im Physikraum und an anderen Orten im Schulhaus
>
> - notiere dir kurz Stichpunkte zu deinem Messablauf
>
> - erstelle dabei folgende Tabelle
>
> - fülle die Messwerte mit den Ergebnissen

__1.3 Ergebnisse:__

|    | Ort der Messung | magnetische Flussdichte B |
|:--:|:---------------:|:-------------------------:|
| 1  | |
| 2  | |
| 3  | |
| 4  | |

__1.4 Auswertung:__

> - ermittle den Mittelwert deiner Messungen und notiere dein Ergebnis:
>
> Das natürliche Magnetfeld der Erde hat am Gym.Klotzsche den mittleren Wert:
> $$B_{Erde} \approx ... $$
>
> Vergleiche den Wert mit dem recherchierten Ergebnis aus den Vorbetrachtungen in 1.1 in einem Satz.

### Experiment Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__2.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - stelle die Formel nach $\mu_0$ um und notiere die Berechnungsvorschrift für $\mu_0$
>
> $$ \boxed{\mu_0 = ... } $$
>
> - notiere die Bedeutung der Formelzeichen
>
> Die magnetische Feldkonstante $\mu_0$ hat den theoretischen Wert
>
> $$ \boxed{\mu_0 = ... } $$
>
> - emittle mit Hilfe der Formelsammlung den Wert von $\mu_0$ und notiere ihn
>
>> Um die magnetische Feldkonstante $\mu_0$ zu bestimmen, müssen die fehlenden Werte der Formel aus 1.1 gemessen werden. Um den Einfluss von Messfehlern zu reduzieren, wird die Messung für __dreimal__ durchgeführt.

__2.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BestimmungMu0](https://diversewolken.ddns.net/nextcloud/index.php/s/ndXRogTZJCCDByY/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V
>
> - bestimme für drei verschiedene Windungszahlen ($N=800,\, 1600,\, 2400$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die halbe Spule aufgewickelt)
>
>     - die Stromstärke $I$ 
>
>     - die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule vorsichtig nach dem Ort mit der maximalen Flussdichte, red)
>
> - notiere alle Messwerte in einer Tabelle

__2.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| # | $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
|:--:|:--:|:--:|:--:|:--:|
| 1 | 800  | .. | .. | .. |
| 2 | 1600 | .. | .. | .. |
| 3 | 2400 | .. | .. | .. |

__2.4 Auswertung:__

> - ermittle aus den Messungen #1-3 und der Formel aus 2.1 jeweils die magnetische Feldkonstante $\mu_0$ und notiere deine Ergebnisse
>
> - ermittle aus den Werten für $\mu_0$ den Mittelwert, notiere dein Endergebnis und vergleiche ihn mit dem theoretischen Wert aus 2.1 (in einem Satz)

__wenn noch min. 15 min Zeit ist:__

> - schau dir Experiment Teil 3 an, du kannst direkt mit der Durchführung (unterhalb der Abnahme) beginnen und die Werte notieren

### Experiment Teil 3: Überprüfung der Proportionalität $B$ ~ $N$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__3.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - notiere die Bedeutung der Formelzeichen
>
> - aufgrund der Formel kann man erkennen, dass die Flussdichte $B$ im Inneren der Spule proportional zur Anzahl der Windungen $N$ sein sollte
>
> - um die Proportionalität von $B$ ~ $N$ zu überprüfen, muss die magnetische Flussdichte $B$ für verschiedene Windungszahlen $N$ bestimmt werden. Dabei muss die Stromstärke $I$ konstant gehalten werden. In einem $B(N)$-Diagramm sollte sich näherungsweise eine Ursprungsgerade ergeben.

__3.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BpN](https://diversewolken.ddns.net/nextcloud/index.php/s/e5eGt4GAqkdK7ws/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V zunächst
>
> - bestimme für drei verschiedene Windungszahlen ($N=2400,\, 1600,\, 800$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die halbe Spule aufgewickelt)
>
>     - bestimme die Stromstärke $I$ für die erste Messung mit $N=2400$
>
>     - bestimme die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule nach dem Ort mit der maximalen Flussdichte, red)
>
>     - verändere bei deiner zweiten Messung mit $N=1600$ die Spannung soweit, dass die Stromstärke $I$ mit der ersten Messung identisch ist
>
>     - wiederhole die Messung für $N=800$
>
> - notiere alle Messwerte in einer Tabelle

__3.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| # | $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
|:--:|:--:|:--:|:--:|:--:|
| 1 | 2400  | .. | .. | .. |
| 2 | 1600  | .. | .. | .. |
| 3 | 800   | .. | .. | .. |

__3.4 Auswertung:__

> - erstelle aus den Messwerten ein Diagramm in dem du die Windungszahl $N$ auf der x-Achse und die magnetische Flussdichte auf der y-Achse einträgst
>
> - markiere in deinem Diagramm die drei Messpunkte #1-3, sowie den Punkt (0|0)
>
> - verbinde die Messpunkte mit einer Ausgleichsgeraden
>
> - überprüfe ob diese Ausgleichsgerade die Messergebnisse in guter Näherung darstellt, notiere einen Ergebnissatz

