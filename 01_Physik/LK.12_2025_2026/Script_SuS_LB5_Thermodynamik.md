<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://diversewolken.ddns.net/nextcloud/s/SfR8K6Tn6mDEFkf/download

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
window.LIA.settings.font_size = 1
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
    input = Math.abs(eval(input)-(@1))/Math.abs(@1)
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
    input = Math.abs(eval(input)-(@1))/Math.abs(@1)
    input <= 0.2
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;margin-left:10px">
@2
</div>
</div>
@end

@rangeQuiz0
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;margin-right:10px">
@0 = 
</div> 
<div style="float:left;display:block">
<!-- data-solution-button="off" style="display:block" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-(@1))
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

# LB 13 Thermodynamik (Wärmelehre)

![Thermodynamik](https://diversewolken.ddns.net/nextcloud/s/SfR8K6Tn6mDEFkf/download)

## 13. 1. Einführung

<section class="flex-container">

<div class="flex-child-2" style="min-width: 400px; margin-bottom: -10px">

Wir betrachten zunächst ein Gas in einem Behälter.


__Ideales Gas:__ Modell, bei dem die Gasteilchen als punktförmige Massepunkte ohne Eigenvolumen betrachtet werden, die keine Anziehungskräfte aufeinander ausüben. Einzige Wechselwirkung sind elastische Stöße zwischen den Teilchen.

</div>

<div class="flex-child-2" style="min-width: 200px; margin-bottom: -10px">

![GasImBehälter](https://www.grund-wissen.de/physik/_images/geschwindigkeitsverteilung-gasteilchen.png)

</div>

</section>



<br> <br>
<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Zustandsgröße:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Temperatur T__, blue)



</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Druck p__, blue)


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(__Volumen V__, blue)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Definition:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Die Temperatur ist ein Maß für die _mittlere Bewegungsenergie_ der einzelnen Teilchen. 

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Der Druck gibt an, welche Kraft $F$ ein Gas auf eine Fläche $A$ ausübt. <br> <br> $$ p = \dfrac{F}{A} $$

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Volumen gibt an, welchen Raumbereich ein Gas einnimmt.

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Einheit:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

K .. Kelvin (absolute Temperatur)

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

Pa .. Pascal (Standardeinheit) <br>
bar .. Bar 


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

m$^{3}$ .. Kubikmeter <br>

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Bemerkungen:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">


_Eine Temperatur von $$T=0\,\mathrm{K} = -273,15^\circ\mathrm{C}$$ bedeutet, dass die Teilchen __keine Bewegungsenergie__ mehr besitzen, d.h. ihre Geschwindigkeit ist Null._

_Wird die Temperatur in $^\circ\mathrm{C}$ angegeben, so verwendet man das Formelzeichen $\vartheta$_. <br>

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">


_Ein Pascal entspricht einer Kraft von einem Newton pro Quadratmeter. <br> $$ \Big[ 1\,\mathrm{Pa} = 1 \dfrac{\mathrm{N}}{\mathrm{m}^2} \Big]$$  $$ \Big[ 1\,\mathrm{bar} = 100\,000\,\mathrm{Pa} \Big] $$


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

_Umrechnung von Volumina z.B. Liter -> m³ oder mm³ in m³ sollte geübt werden _

$$ \Big[ 1\,\mathrm{ℓ} = 10^{-3}\,\mathrm{m}^3\Big]$$

</div>

</section>


## 13. 2. Zustandsgleichung für das ideale Gas

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> $$ \boxed{\dfrac{p \cdot V}{T} = konst.} $$

Ändert sich bei einem Gas eine der Zustandsgrößen $T$, $V$ oder $p$, so ändern sich auch die anderen Größen.

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

??[Simulation](https://phet.colorado.edu/sims/html/gas-properties/latest/gas-properties_all.html?locale=de)

</div>

</section>

---

Wir unterscheiden dabei folgende __Zustandsänderungen:__ <br> <br>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Art der Änderung:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(iso__bare__ Zustandsänderung, red) <br>

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(iso__therme__ Zustandsänderung, red)

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

@color(iso__chore__ Zustandsänderung, red)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Beschreibung:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

> Während der Änderung bleibt der __Druck konstant__, Volumen und Temperatur ändern sich. <br> $$ p = konst. $$

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

> Während der Änderung bleibt die Temperatur __konstant__. <br> $$ T = konst. $$

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

> Während der Änderung bleibt das Volumen __konstant__. <br> $$ V = konst $$

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 50px; margin-bottom: -10px">

Änderung von 1->2:

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

<details style='color:blue;margin-left:10%'>

<summary>  </summary>

$$ \dfrac{V_1}{T_1} = \dfrac{V_2}{T_2} $$

</details>


</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

<details style='color:blue;margin-left:10%'>

<summary>  </summary>

$$ p_1 \cdot V_1 = p_2 \cdot V_2 $$

</details>

</div>

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

<details style='color:blue;margin-left:10%'>

<summary>  </summary>

$$ \dfrac{p_1}{T_1} = \dfrac{p_2 }{T_2} $$

</details>

</div>

</section>

![IdealeGasgleichung](https://diversewolken.ddns.net/nextcloud/s/FrrqBqKHJkYifWe/download)

#### Gasberechnungen am Stickstoff

In einem Labor wird Stickstoff bei der konstanten Temperatur $20,0 \, ^\circ\text{C}$ in eine $100$-Liter-Stahlflasche gedrückt. Dabei wächst der Druck von $100 \, \text{kPa}$ auf $22,1 \, \text{MPa}$.

1. Benennen Sie die Art der Zustandsänderung bei der Befüllung.

<p style='margin-left:10%'>

[[ isotherm ]]

</p>

---

__Maximal zulässige Temperatur__

Die Flasche ist bis zu einem Maximaldruck von $p_{max} = 28,0 \, \text{MPa}$ zugelassen. Für die Lagerung kann sich die Temperatur um die Flasche herum langsam ändern. 

---

2. 1. Benennen Sie die Art der Zustandsänderung bei der Lagerung.

<p style='margin-left:10%'>

[[ isochor ]]

</p>

---

2. 2. Berechnen Sie die maximal zulässige Temperatur $\vartheta_{max}$ in der Einheit $^\circ\mathrm{C}$, bei der die gefüllte Flasche gelagert werden darf.

<p style='margin-left:10%'>

@rangeQuiz2( $\vartheta_{max}$ , 98.26, $\mathrm{^\circ C}$ )

</p>


<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Da das Volumen der Stahlflasche konstant bleibt ($V = const.$), handelt es sich um eine **isochore Zustandsänderung**. Es gilt:
$\frac{p_1}{T_1} = \frac{p_2}{T_2} \Rightarrow T_2 = \frac{p_2 \cdot T_1}{p_1}$.

1. Umrechnung der Ausgangstemperatur $T_1$ in Kelvin.

<p style='margin-left:10%'>

@rangeQuiz2($T_1$,293.15,$\mathrm{K}$)

</p>

2. Einsetzen der Drücke $p_1 = 22,1 \, \text{MPa}$ und $p_2 = 28,0 \, \text{MPa}$.

<p style='margin-left:10%'>

@rangeQuiz2($T_2$,371.41,$\mathrm{K}$)

</p>

3. Rückrechnung der Ergebnistemperatur $T_2$ in Grad Celsius: 

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

$T_2 = \frac{28,0 \, \text{MPa} \cdot 293 \, \text{K}}{22,1 \, \text{MPa}} \approx 371 \, \text{K}$.

$\vartheta_{max} = 371 \, \text{K} - 273 = \mathbf{98 \, ^\circ C}$.

Die Flasche darf bis zu einer Temperatur von $98 \, ^\circ\text{C}$ gelagert werden.

</details>

---


---

2. 3. Berechnen Sie die Masse $\Delta m$ des zusätzlich eingefüllten Stickstoffs.

<p style='margin-left:10%'>

@rangeQuiz2( $\Delta m$ , 25.3, $\mathrm{kg}$ )

</p>

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

Zur Berechnung wird die **thermische Zustandsgleichung** für ideale Gase genutzt:
$p \cdot V = n \cdot R \cdot T$ mit $n=\frac{m_{N_2}}{M_{N_2}} \Rightarrow m_{N_2} = \frac{p \cdot V}{T}\cdot\frac{M_{N_2}}{R}$.

$m_{N_2}$ ist die Masse des Stickstoffs.

$M_{N_2}$ ist die molare Masse des Stickstoffs.

Die molare Masse von Stickstoff (hier als $N_2$-Molekül) ergibt sich aus der Masse, die ein Mol Stickstoff-Moleküle besitzt. Ermitteln Sie diese und setzen Sie sie in obige Formel ein.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg2</summary>

Ein Stickstoff-Atom besitzt eine Masse von ungefähr $14\,\mathrm{u}$ <br> -> $u$ .. atomare Masseneinheit $u=1,66\cdot10^{-27}\,\mathrm{kg}$.

Das Stickstoffmolekül $N_2$ hat demzufolge die Masse 

<p style='margin-left:10%'>

@rangeQuiz2($m_{N_2}$ , 4.648e-26 , $\mathrm{kg}$)

</p>

Die Stoffmenge $n=1\,\mathrm{mol}$ enthält $6,022\cdot10^{23}$ Teilchen. Die molare Masse von Stickstoff ist demzufolge

<p style='margin-left:10%'>

@rangeQuiz2($M_{N_2}$ , 0.028 , $\mathrm{\frac{kg}{mol}}$)

</p>

Mit der Formel $m_{N_2} = \frac{p \cdot V}{T}\cdot\frac{M_{N_2}}{R}$ lässt sich nun die Masse an Stickstoff ermitteln.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

Ein Stickstoff-Atom besitzt eine Masse von ungefähr $14\,\mathrm{u}$ <br> -> $u$ .. atomare Masseneinheit $u=1,66\cdot10^{-27}\,\mathrm{kg}$.

Das Stickstoffmolekül $N_2$ hat demzufolge die Masse 

$m_{N_2} = 2 \cdot 14 \cdot 1,66\cdot10^{-27}\,\mathrm{kg} = 4,648\cdot 10^{-26} \,\mathrm{kg}$


Die Stoffmenge $n=1\,\mathrm{mol}$ enthält $6,022\cdot10^{23}$ Teilchen. Die molare Masse von Stickstoff ist demzufolge

$M_{N_2} = m_{N_2} \cdot 6,022\cdot10^{23} = 0,028 \,\mathrm{\frac{kg}{mol}}$

Mit der Formel $m_{N_2} = \frac{p \cdot V}{T}\cdot\frac{M_{N_2}}{R}$ lässt sich nun die Masse an Stickstoff ermitteln.

$m_{N_2} = 25,4\,\mathrm{kg}$

</details>


---

2. 4. Für Versuchszwecke wird der Flasche nach dem Füllvorgang $5,00$ Stunden lang Stickstoffgas bei der konstanten Temperatur $20,0 \, ^\circ\text{C}$ entnommen. Dabei strömt in jeder Stunde gleichmäßig $1,00 \, \text{kg}$ Gas aus. <br> Geben Sie eine Gleichung an, die den funktionalen Zusammenhang zwischen dem Gasdruck $p$ in der Flasche und der Zeit $t$ beschreibt ($0 \le t \le 5 \, \text{h}$). <br> _Hinweise: Setzen Sie alle bekannten Größen ein. Gehen Sie davon aus, dass die Zeit in der Einheit $\mathrm{[h]}$ angegeben wird._

<details style="margin-left:10%;color:blue">
<summary>Lösungshinweis</summary>

Der Druck ergibt sich aus der zeitabhängigen Masse $m(t)$. Da pro Stunde $1 \, \text{kg}$ entweicht, gilt:
$m(t) = m_{Anfang} - \frac{1,00 \, \text{kg}}{\text{h}} \cdot t$

Aus der Zustandsgleichung folgt: $p(t) = \frac{m(t) \cdot R_s \cdot T}{V}$.

Setzen Sie $m_{Anfang} = 25,3 \, \text{kg}$ (aus Aufgabe 3.2), $R_s = 297 \, \frac{\text{J}}{\text{kg} \cdot \text{K}}$, $T = 293 \, \text{K}$ und $V = 0,1 \, \text{m}^3$ ein.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

Die Masse nach $t$ Stunden beträgt: $m(t) = (25,3 - t) \, \text{kg}$ (mit $t$ in Stunden).

$p(t) = (25,3 - t) \cdot \frac{297 \cdot 293}{0,1} \, \text{Pa}$

$\underline{p(t) = (25,3 - t) \cdot 870210 \, \text{Pa}}$.

Der Graph dieser Funktion ist eine **fallende Gerade**, die bei ca. $22,0 \, \text{MPa}$ startet und nach $5$ Stunden einen Druck von ca. $17,7 \, \text{MPa}$ erreicht.

</details>



## 13. 3. Erster Hauptsatz der Thermodynamik

> Der erste Hauptsatz beschreibt die Energieerhaltung in einem thermodynamischen System:
>
> $$ \boxed{\Delta U = Q + W} $$
>
> mit
>
> $\hspace{1cm}$ $\Delta U$ .. Änderung der inneren Energie
>
> $\hspace{1cm}$ $Q$ .. abgegebene oder zugeführte Wärmeenergie
>
> $\hspace{1cm}$ $W$ .. Volumenarbeit, die das System verrichtet/die am System verrichtet wird

---
 
<p style="margin-left:10%">

__Konvention zu Vorzeichen:__ 

- @color( Ist eine Energie/Arbeit __negativ__ gibt das System Energie an die Umgebung ab., red) 

- @color(__Postive__ Werte beschreiben die Aufnahme von Energie., red)

</p>

---

<section class="flex-container" style="margin-left:10%">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

@color(__abgegebene/aufgenommene__, blue) <br> __Wärmeenergie $Q$__

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Volumenarbeit $W$__

</div>

</section>

---

<section class="flex-container" style="margin-left:10%">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

$ \boxed{Q = m \cdot c \cdot \Delta T} $

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

$ \boxed{W = -\displaystyle\int^{V_2}_{V_1} p\,\mathrm{d}V} $

</div>

</section>

<br>

<section class="flex-container" style="margin-left:10%">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

$c$ .. spezifische Wärmekapazität <br> -> $c_p$: bei konstantem Druck <br> -> $c_V$: bei konstantem Volumen

$\Delta T$ .. Temperaturänderung 

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

Volumenarbeit ist Volumenänderung $\mathrm{d}V$ bei herrschendem Druck $p$

_Bildlich: Fläche unter p(V)-Graph_

</div>

</section>


---

<section class="flex-container" style="margin-left:10%">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Abkühlung:__ $\Delta T<0$ -> $Q<0$ -> System gibt Energie an Umgebung ab

__Erwärmung:__ $\Delta T>0$ -> $Q>0$ -> dem System wird Energie zugeführt

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Ausdehnung:__ -> $V_2 > V_1$ -> $W < 0$ -> System gibt Energie an Umgebung ab

__Kompression:__ -> $V_2 < V_1$ -> $W > 0$ -> dem System wird Energie zugeführt 

</div>

</section>

---

> __Definition Innere Energie__: Die Innere Energie beschreibt die Summe der kinetischen Energien aller Gas-Teilchen.


#### Übungsaufgaben zum ersten Hauptsatz

1. Ergänze die Temperaturdifferenzen.

<p style="margin-left:5%">

|Anfangstemperatur | Endtemperatur | Differenz | 
| $T_1$ | $T_2$ | $\Delta T$ |
| $18,5^\circ$ | $95,3^\circ$ | [[76,8]]K |
| $-14,2^\circ$ | $4,2^\circ$ | [[18,4]]K |
| $-7,1^\circ$ | $-13,6^\circ$ | [[-6,5]]K |

</p>


2. Der Inhalt der mit Stickstoff gefüllten Gasflasche aus der vorherigen Aufgabe ($m_{N_2}=25,4\,\mathrm{kg}$), $V=100\,\mathrm{ℓ}$, $\vartheta=20^\circ C$, soll auf $50^\circ C$ erwärmt werden.

2. 1. Wählen Sie für jeden Energiebetrag die qualitativ richtige Aussage.

<p style="margin-left:10%">

- [[X]] $Q>0$
- [[ ]] $Q=0$
- [[ ]] $Q<0$
- [[ ]] $W>0$
- [[X]] $W=0$
- [[ ]] $W<0$

</p>

---

2. 2. Ermitteln Sie die Beträge für Wärmeenergie und Volumenarbeit.

<p style='margin-left:10%'>

@rangeQuiz2($Q$,5.715e5,$\mathrm{J}$)

@rangeQuiz0($W$,0,$\mathrm{J}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Ermitteln Sie im Tafelwerk den Wert für die spezifische Wärmekapazität von Stickstoff. Entscheiden Sie, ob Sie $c_V$ oder $c_p$ nutzen müssen.

- [[X]] $c_V$
- [[ ]] $c_p$

@rangeQuiz2($c$,0.75,$\mathrm{\frac{kJ}{kg\cdot K}}$)


_Hinweis: Achten Sie darauf, dass das Tafelwerk den Wert für c in kJ im Nenner angibt._

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

Da sich das Volumen bei der Erwärmung nicht ändert, muss für c der Wert bei konstantem Volumen genutzt werden.

$ c_V = 0,75\,\mathrm{\frac{kJ}{kg\cdot K}} = 750\,\mathrm{\frac{\red{J}}{kg\cdot K}} $

Die Wärmeenergie $Q$ ergibt sich zu

$ Q = 22,4\,\mathrm{kg}\cdot 750 \,\mathrm{\frac{\red{J}}{kg\cdot K}} \cdot 30\,\mathrm{K} = 5,715\cdot 10^5\,\mathrm{J}$

</details>

---

3. ![Plastiktüte](https://www.stuttgarter-nachrichten.de/media.media.fdfaf648-aac3-4a6a-ad04-ac4e6200ddca.16x9_700.jpg) Mit dem Inhalt der Stickstoff-Flasche soll nun eine sehr dünne $20\,\mathrm{ℓ}$ Plastiktüte aufgepustet werden. Dieser Vorgang soll so langsam stattfinden, dass die Temperatur des Gases innerhalb der Tüte bei $20°C$ konstant bleibt. Zur Vereinfachung wird angenommen, dass der Innendruck der Tüte während des Aufpustens immer gleich dem Außendruck (Luftdruck) entspricht. <br> _Hinweise: In der Realtität wäre der Innendruck geringfügig höher als der Außendruck, da sich die Tüte sonst nicht aufbläht. Die Tüte wird als nicht elastisch betrachtet, d.h. sobald die $20\,\mathrm{ℓ}$ eingefüllt sind, stoppt der Vorgang._

3. 1. Ermitteln Sie die Stoffmenge und die Anzahl der Stickstoff-Atome, die sich in der Plastiktüte befindet.

<p style='margin-left:10%'>

@rangeQuiz2($n$,0.821,$\mathrm{mol}$)

@rangeQuiz2($N_{N_2}$,4.944e23, $N_2$-Moleküle)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Nutzen Sie die ideale Gasgleichung um für den Endzustand die Stoffmenge $n$ zu berechnen. Für die Anzahl an Teilchen pro Mol nutzen Sie die Avogadro-Konstante $6,022\cdot 10^{23} \frac{1}{\mathrm{mol}}$.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$p = 10^5 \,\mathrm{Pa}$

$T = 293 K$

$V = 0,02 m^3$

$R = 8,314 \frac{J}{mol \cdot K}$

$\dfrac{p\cdot V}{T} = n \cdot R$ -> $n=0,821\,\mathrm{mol}$

$N_{N_2} = n \cdot N_A$

</details>

---

3. 2. Ermitteln Sie Volumenarbeit $W$, die das Gas beim Füllen der Tüte verrichet hat.

<p style='margin-left:10%'>

@rangeQuiz2($W$,-2000,$J$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Die Volumenarbeit wird mit der Formel aus dem ersten Hauptsatz der Thermodynamik bestimmt. Dabei ist das Anfangsvolumen $V_1=0$ und das Zielvolumen $V_2=20\,\mathrm{ℓ}$. Der Druck ist mit $1\,\mathrm{bar}$ konstant.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$W = -\displaystyle\int^{V_2}_{V_1} p\,\mathrm{d}V = -\displaystyle\int^{0,02\,\mathrm{m^3}}_{0} 10^5\,\mathrm{Pa}\,\mathrm{d}V = -10^5\,\mathrm{Pa} \cdot 0,02\,\mathrm{m^3}$

$W = -2000\,\mathrm{J}$

</details>


## 13. 4. Kreisprozesse - Reversible Prozesse bei idealen Gasen

> Wird ein ideales Gas wird in einem __zyklischen (d.h. sich wiederholendem) Prozess__ über mehrere Zustandsänderungen in seinen Ausgangszustand zurück versetzt, so nennen wir das @color(Kreisprozess, red).

__Beispiel (einfacher Kreisprozess):__ 

<section class="flex-container">

<div class="flex-child-2" style="min-width: 100px; margin-bottom: -10px">

![Kreisprozess2](https://diversewolken.ddns.net/nextcloud/s/Fps2Mt6bstMmrCC/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">


__Art der Zustandsänderung:__

A->B: [[ (isobar) | isochor | isotherm ]] <br>
B->C: [[ isobar | (isochor) | isotherm ]] <br>

__Volumenarbeit $W$:__

$W_{A->B} = $ <br> <br>
 
$W_{B->C} = $

__Beispielrechnung:__

Das ideale Gas durchläuft den dargestellten zyklischen Prozess. In Punkt A beträgt das Volumen $1\,\mathrm{ℓ}$ und der Druck $2\,\mathrm{bar}$. Das Volumen wird auf $2,5\mathrm{ℓ}$ erhöht (B). In Punkt $C$ beträgt der Druck $1\,\mathrm{bar}$.

</div>

</section>

---

__Ermitteln Sie die Volumenarbeiten:__

<section class="flex-container" style="margin-left:5%">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

@rangeQuiz2($W_{A->B}$,-300,$\mathrm{J}$)

@rangeQuiz2($W_{B->C}$,0,$\mathrm{J}$)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px; margin-left:10%">

@rangeQuiz2($W_{C->D}$,150,$\mathrm{J}$)

@rangeQuiz0($W_{D->A}$,0,$\mathrm{J}$)

</div>

</section>


#### Übungsaufgabe Kreisprozesse

Ein (vereinfachter) thermodynamischer Kreisprozess in einem geschlossenen System soll in drei Stufen ablaufen. Abb. 1 stellt den Prozess in einem p-V-Diagramm dar. <br> _Hinweis: Diagramm nur qualitativ_.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Kreisprozess3](https://diversewolken.ddns.net/nextcloud/s/ATKZxG5PirDSyMB/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Beschreibung:__ $0,32\,\mathrm{mol}$ Stickstoff ($N_2$) nehmen bei einem Druck von $2,4\,\mathrm{bar}$ ein Volumen von $2,2\,\mathrm{ℓ}$ ein (A). Dann durchläuft das Gas einen zyklischen Prozess mit folgenden Vorgängen.

__A->B:__ Das Gas wird bei konstantem Druck erwärmt bis sein Volumen $4,4\,\mathrm{ℓ}$ beträgt (B).

__B->C:__ Das Gas wird bei konstantem Volumen abgekühlt, bis der Druck auf $1,2\,\mathrm{bar}$ gefallen ist (C).

__C->A:__ Das Gas erfährt eine isotherme Kompression zurück zum Punkt A.

</div>

</section>

---

1. Ermitteln Sie die Temperatur an den Punkten A, B und C.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

@rangeQuiz2($T_A$,198.46,$\mathrm{K}$)

@rangeQuiz2($T_B$,396.92,$\mathrm{K}$)

@rangeQuiz2($T_C$,198.46,$\mathrm{K}$)

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> Lösungshinweis </summary>

$T_A$: Nutzen Sie die ideale Gasgleichung, um für den Punkt A die Temperatur zu ermitteln.

$T_B$: Entnehmen Sie aus den Angaben die Werte für den Druck und das Volumen in Punkt B. Ermitteln Sie damit die Temperatur $T_B$.

$T_C$: Schlußfolgern Sie aus den beschriebenen Zustandsänderungen auf die Temperatur $T_C$.

</details>

<details style='color:blue'>

<summary> Lösung </summary>

$T_A = \dfrac{p_A \cdot V_A}{n \cdot R} = 198,5 K$

---

$p_B = p_A$ (isobare)

$V_B = 4,4\,\mathrm{ℓ}$

$T_B = \dfrac{p_B \cdot V_B}{n \cdot R} = 396,92\,\mathrm{K}$

$T_C=T_A=198,5\,\mathrm{K}$

</details>

</div>

</section>

---

2. Ermitteln Sie für die beschriebenen Zustandsänderungen jeweils die Größen $\Delta U$, $W$ und $Q$.


<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

__A->B:__ <br> <br>

<p style='margin-left:10%'>


@rangeQuiz2($W_{A->B}$,-528,$\mathrm{J}$)

@rangeQuiz2($Q_{A->B}$,1849,$\mathrm{J}$)

@rangeQuiz2($\Delta U_{A->B}$,1321,$\mathrm{J}$)

</p>

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> Lösungshinweis </summary>

$W_{A->B}$: Die Volumenarbeit ist gegeben durch die Fläche unter dem Graphen (Vorzeichen beachten).

$Q_{A->B}$: Die zugeführte Wärmemenge ergibt sich aus der Temperaturänderung und der spezifischen Wärmekapazität bei konstantem Druck $c_p$. 

$\Delta U_{A->B}$: Ermitteln Sie die Änderung der inneren Energie aus den Werte für $Q$ und $W$.

</details>

<details style='color:blue'>

<summary> Lösung </summary>

$W_{A->B} = - \displaystyle\int_{2,2\,\mathrm{ℓ}}^{4,4\,\mathrm{ℓ}} p \cdot \mathrm{d}V = - 2,4\,\mathrm{bar} \cdot (2,2\,\mathrm{ℓ})$

$W_{A->B} = -528\,\mathrm{J}$

---

$Q_{A->B} = m \cdot c_p \cdot \Delta T_{A->B}$

<p style="margin-left:5%">

Masse: $m = n_{N_2} \cdot M_{N_2} = 0,32\,\mathrm{mol} \cdot 0,028\,\mathrm{\dfrac{kg}{mol}} = 0,00896\,\mathrm{kg}$

spez. WK (laut Formelsammlung): $c_p = 1,04 \mathrm{\dfrac{kJ}{kg\cdot K}}$

$\Delta T = (396,9-198,5)\,\mathrm{K} = 198,4 \,\mathrm{K}$

</p>

$Q_{A->B} = 1,849\,\mathrm{kJ} = 1849\,\mathrm{J}$

---

$\Delta U_{A->B} = Q_{A->B} + W_{A->B} = 1321\,\mathrm{J}$

</details>

</div>

</section>

---


<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

__B->C:__ <br> <br>

<p style='margin-left:10%'>


@rangeQuiz0($W_{B->C}$,0,$\mathrm{J}$)

@rangeQuiz2($Q_{B->C}$,-1849,$\mathrm{J}$)

@rangeQuiz2($\Delta U_{B->C}$,-1849,$\mathrm{J}$)

</p>

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> Lösungshinweis </summary>

$W_{B->C}$: Die Volumenarbeit ist gegeben durch die Fläche unter dem Graphen (Vorzeichen beachten).

$Q_{B->C}$: Die zugeführte Wärmemenge ergibt sich aus der Temperaturänderung und der spezifischen Wärmekapazität bei konstantem Druck $c_p$. 

$\Delta U_{B->C}$: Ermitteln Sie die Änderung der inneren Energie aus den Werte für $Q$ und $W$.

</details>

<details style='color:blue'>

<summary> Lösung </summary>

$W_{B->C} = 0 $ (keine Volumenänderung, keine Volumenarbeit)

---

$Q_{B->C} = m \cdot c_p \cdot \Delta T_{B->C}$

<p style="margin-left:5%">

Masse: $m = 0,00896\,\mathrm{kg}$

spez. WK: $c_p = 1,04 \mathrm{\dfrac{kJ}{kg\cdot K}}$

$\Delta T = (198,5-396,9)\,\mathrm{K} = -198,4 \,\mathrm{K}$

</p>

$Q_{B->C} = -1849\,\mathrm{J}$

---

$\Delta U_{B->C} = Q_{B->C} + W_{B->C} = -1849\,\mathrm{J}$

</details>

</div>

</section>

---


<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

__C->A:__ <br> <br>

<p style='margin-left:10%'>


@rangeQuiz2($W_{C->A}$,366,$\mathrm{J}$)

@rangeQuiz2($Q_{C->A}$,-366,$\mathrm{J}$)

@rangeQuiz0($\Delta U_{C->A}$,0,$\mathrm{J}$)

</p>

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue'>

<summary> Lösungshinweis </summary>

$W_{C->A}$: Die Volumenarbeit ist gegeben durch die Fläche unter dem Graphen (Vorzeichen beachten). Hier muss aus der isothermen Bedingung $p\cdot V=konst$ ein Ausdruck für $p(V)$ gefunden werden und dieser dann in das Integral eingesetzt werden.

$Q_{C->A}$: Die zugeführte Wärmemenge ergibt sich aus der Temperaturänderung und der spezifischen Wärmekapazität bei konstantem Druck $c_p$. 

$\Delta U_{C->A}$: Ermitteln Sie die Änderung der inneren Energie aus den Werte für $Q$ und $W$.

</details>

<details style='color:blue'>

<summary> Lösung </summary>

$W_{C->A} = - \displaystyle\int_{4,4\,\mathrm{ℓ}}^{2,2\,\mathrm{ℓ}} p(V) \cdot \mathrm{d}V $

Für eine isotherme Zuständsänderung gilt: $ p \cdot V = const $.

Man kann für die Druckabhängigkeit: 

$p(V) = p_C \cdot V_C \cdot \dfrac{1}{V}$

ansetzen. Es ergibt sich

$W_{C->A} = - \displaystyle\int_{4,4\,\mathrm{ℓ}}^{2,2\,\mathrm{ℓ}} p_C \cdot V_C \cdot \dfrac{1}{V} \cdot \mathrm{d}V $

Entweder in den CAS eintippen und numerisch lösen lassen:

$W_{C->A} = 366\,\mathrm{J}$

---

Da sich die Temperatur nicht ändert, ändert sich auch die Bewegungsenergie der Teilchen nicht, somit ist die Änderung der inneren Energie gleich Null.

$\Delta U_{C->A} = 0$

---

Aus dem ersten Hauptsatz ergibt sich dann

$\Delta Q_{C->A} = -W_{C->A} = -366\,\mathrm{J}$

</details>

</div>

</section>


## 13. 5. Adiabatische Zustandsänderungen

> Viele Zuständsänderungen von Gasen laufen __so schnell oder gut isoliert__ ab, dass für einen Wärmeaustausch mit der Umgebung keine Zeit ist. Einen Vorgang ohne Wärmeaustausch mit der Umgebung nennt man @color(adiabatisch, red), d.h. $$ \boxed{Q = 0} $$


<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> Für eine @color(adiabatische Zustandsänderung, red) gilt:
>
> $$ \boxed{p \cdot V^\kappa = const.} $$ und $$ \boxed{T \cdot V^{\kappa-1} = const.} $$
>
> wobei $\kappa = \dfrac{c_p}{c_V}$ als @color(Adiabatenexponent, red) definiert ist.
> Für ideale einatomige Gase gilt $\kappa=\frac{5}{3}$, für zweiatomige Gase ist $\kappa=\frac{7}{5}$.
>
> __Achtung:__ Die Temperatur des Gases ändert sich, aber $Q=0$.

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Adiabate](https://diversewolken.ddns.net/nextcloud/s/XSQyMaokoLDqY7q/download)

</div>

</section>

---

> __Energiebetrachtung:__
>
> $$\Delta U = W \hspace{0.5cm} \mathrm{weil\,} \hspace{0.5cm} Q=0$$
>
> $$ W = -\displaystyle\int^{V_2}_{V_1} p(V) \,\mathrm{d}V $$
>
> $$ W = - p_1 \cdot V_1^\kappa \cdot \displaystyle\int^{V_2}_{V_1} \dfrac{1}{V^\kappa} \,\mathrm{d}V $$

---

__Beispiel:__ $0,32\,\mathrm{mol}$ Stickstoff ($N_2$) nehmen bei einem Druck von $2,4\,\mathrm{bar}$ ein Volumen von $2,2\,\mathrm{ℓ}$ ein (1). Dann durchläuft das Gas eine adiabatische Zustandsänderung zu einem Volumen von $4,4\,\mathrm{ℓ}$ (2). Ermitteln Sie die Volumenarbeit $W$. Ermitteln Sie die Temperatur $T_2$, sowie den Druck $p_2$.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

@rangeQuiz2($W$,-319.6,$\mathrm{J}$)

@rangeQuiz2($p_2$,0.90943,$\mathrm{bar}$)

@rangeQuiz2($T_2$,150.3,$\mathrm{K}$)

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$\kappa=\frac{7}{5}$

CAS -> Integral zur Berechnung der Volumenarbeit ermitteln.

$W = -319,6\,\mathrm{J}$

Der Druck $p_2$ ergibt sich mit Hilfe der Gleichung für die adiabatische Zustandsänderung:

$p_1 \cdot V_1^\kappa = p_2 \cdot V_2^\kappa$

$p_2 = \dfrac{p_1 \cdot V_1^\kappa}{V_2^\kappa} = 90,9\,\mathrm{kPa} = 0,909\,\mathrm{bar}$

Die Temperatur $T_2$ ergibt sich auch der idealen Gasgleichung

$T_2 = \dfrac{p_2 \cdot V_2}{n \cdot R} = 150,3 K$

</details>

</div>

</section>

## 13. 6. Carnotscher Kreisprozess

> Der Carnotsche Kreisprozess ist ein idealisierter thermodynamischer Kreisprozess mit @color(maximal möglichem Wirkungsgrad, red) zwischen zwei Wärmereservoiren (warm $T_{high}$, kalt $T_{low}$). $$ \textbf{Wirkungsgrad:}\hspace{1cm}\boxed{\eta_\text{Carnot} = 1 - \frac{T_{low}}{T_{high}}}$$

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Vier reversible__ Zustandsänderungen:

1. __Isotherme Expansion bei $T_{high}$:__ <br> Das Arbeitsmedium nimmt Wärme $Q_H$ aus dem heißen Reservoir auf und verrichtet Arbeit.

2. __Adiabatische (isentrope) Expansion:__ <br> Keine Wärmeübertragung, die Temperatur sinkt von $T_{high}$ auf $T_{low}$.

3. __Isotherme Kompression bei $T_{low}$:__ <br> Wärme $Q_C$ wird an das kalte Reservoir abgegeben.

4. __Adiabatische (isentrope) Kompression:__ <br> Keine Wärmeübertragung, die Temperatur steigt von $T_{low}$ auf $T_{high}$.


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![CarnotProzess](https://diversewolken.ddns.net/nextcloud/s/o2ynFtAAY3ZH7cf/download)

</div>

</section>


#### Aufgabe: Der Carnot-Kreisprozess

Carnot-Prozess eines idealen Gases

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

Die obere Isotherme mit $T_1 = 500 \text{ K}$ des Carnot-Prozesses eines idealen Gases ($\kappa = 1,4$) verläuft zwischen den Zuständen $p_1 = 8 \text{ bar}$, $V_1 = 2 \text{ m}^3$ und $p_2 = 4 \text{ bar}$, $V_2 = 4 \text{ m}^3$.

Zu berechnen sind:

1. Die Zustandsgrößen $p_3, V_3$ und $p_4, V_4$ am Ende der adiabatischen Expansion bzw. Kompression, wenn die untere Temperatur $T_3 = 350 \text{ K}$ beträgt.

2. Die ausgetauschten Wärmemengen $Q_1$ (zugeführt) und $Q_2$ (abgeführt) 

3. Der thermische Wirkungsgrad $\eta$ 

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![CarnotKreisprozess](https://physikaufgaben.de/bild/a479_1.jpg)

</div>

</section>

---

1. Berechnung der Zustandsgrößen

<p style="margin-left:10%">

Ermitteln Sie zunächst die Volumina $V_3$ und $V_4$ sowie die zugehörigen Drücke.

@rangeQuiz2( $V_3$ , 9.78, $\mathrm{m^3}$ )

@rangeQuiz2( $p_3$ , 1.15e5, $\mathrm{Pa}$ )

@rangeQuiz2( $V_4$ , 4.88, $\mathrm{m^3}$ )

@rangeQuiz2( $p_4$ , 2.3e5, $\mathrm{Pa}$ )

<details style="margin-left:0%;color:blue">
<summary>Lösungsweg</summary>

**1. Adiabatische Expansion (Zustand 2 zu 3):**
Da der Übergang adiabatisch ist, gilt die Adiabatengleichung:
$T_2 \cdot V_2^{\kappa-1} = T_3 \cdot V_3^{\kappa-1}$
Umgestellt nach $V_3$:
$V_3 = V_2 \cdot \left(\frac{T_2}{T_3}\right)^{\frac{1}{\kappa-1}} = 4 \text{ m}^3 \cdot \left(\frac{500 \text{ K}}{350 \text{ K}}\right)^{\frac{1}{0,4}}$
$V_3 \approx 4 \cdot (1,428)^{2,5} \approx \mathbf{9,78 \text{ m}^3}$

---

Den Druck $p_3$ erhält man über die thermische Zustandsgleichung ($p \cdot V / T = const.$):
$p_3 = p_2 \cdot \frac{V_2}{V_3} \cdot \frac{T_3}{T_2} = 4 \text{ bar} \cdot \frac{4}{9,78} \cdot \frac{350}{500} \approx \mathbf{1,15 \text{ bar}}$

---

**2. Adiabatische Kompression (Zustand 4 zu 1):**
Analog gilt für $V_4$:
$V_4 = V_1 \cdot \left(\frac{T_1}{T_4}\right)^{\frac{1}{\kappa-1}} = 2 \text{ m}^3 \cdot \left(\frac{500 \text{ K}}{350 \text{ K}}\right)^{2,5} \approx \mathbf{4,88 \text{ m}^3}$
$p_4 = p_1 \cdot \frac{V_1}{V_4} \cdot \frac{T_4}{T_1} = 8 \text{ bar} \cdot \frac{2}{4,88} \cdot \frac{350}{500} \approx \mathbf{2,30 \text{ bar}}$

</details>

</p>

---

2. Wärmemengen

<p style="margin-left:10%">

Berechnen Sie die zugeführte Wärme $Q_1$ (isotherme Expansion) und die abgeführte Wärme $Q_2$ (isotherme Kompression).

@rangeQuiz2( $Q_1$ , 1.11, $\mathrm{MJ}$ )

@rangeQuiz2( $Q_2$ , -0.78, $\mathrm{MJ}$ )

<details style="margin-left:0%;color:blue">
<summary>Lösungsweg</summary>

Bei einer isothermen Zustandsänderung entspricht die Wärme der verrichteten Volumenarbeit:
$Q = p \cdot V \cdot \ln\left(\frac{V_{ende}}{V_{anfang}}\right)$

**Zugeführte Wärme $Q_1$ (1 zu 2):**
$Q_1 = 8 \cdot 10^5 \text{ Pa} \cdot 2 \text{ m}^3 \cdot \ln\left(\frac{4}{2}\right) \approx 1,11 \cdot 10^6 \text{ J} = \mathbf{1,11 \text{ MJ}}$

**Abgeführte Wärme $Q_2$ (3 zu 4):**
$Q_2 = p_3 \cdot V_3 \cdot \ln\left(\frac{V_4}{V_3}\right) = 1,15 \cdot 10^5 \text{ Pa} \cdot 9,76 \text{ m}^3 \cdot \ln\left(\frac{4,88}{9,76}\right)$
$Q_2 \approx 11,22 \cdot 10^5 \text{ J} \cdot (-0,693) \approx \mathbf{-0,78 \text{ MJ}}$

</details>

</p>

---

3. Thermischer Wirkungsgrad

<p style="margin-left:10%">

Bestimmen Sie den Wirkungsgrad $\eta$ des Prozesses.

@rangeQuiz2( $\eta$ , 0.3, )

<details style="margin-left:0%;color:blue">
<summary>Lösungsweg</summary>

Für den idealen Carnot-Prozess hängt der Wirkungsgrad nur von den Temperaturen ab:
$\eta = 1 - \frac{T_{niedrig}}{T_{hoch}}$
$\eta = 1 - \frac{350 \text{ K}}{500 \text{ K}} = 1 - 0,7 = \mathbf{0,3}$

Alternativ über die Wärmemengen:
$\eta = \frac{Q_1 + Q_2}{Q_1} = \frac{1,11 \text{ MJ} - 0,78 \text{ MJ}}{1,11 \text{ MJ}} \approx 0,3$

</details>

</p>


## 13. 7. Der Stirling-Motor

> Der Stirling-Motor ist eine __Wärmekraftmaschine__ mit geschlossenem Arbeitsgas (He, Luft). Zugeführte thermische Energie wird in mechanische Energie umgewandelt.

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Idealisierter Stirling-Kreisprozess:__

1. __Isotherme Expansion__ am heißen Ende: Gas nimmt Wärme auf und leistet Arbeit.
2. __Isochore Abkühlung__ über den Regenerator: Gas gibt Wärme an den Regenerator ab.
3. __Isotherme Kompression__ am kalten Ende: Gas wird zusammengepresst und gibt Wärme ab.
4. __Isochore Erwärmung__ über den Regenerator: Gas nimmt die gespeicherte Wärme wieder auf.

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Sterling](https://physikaufgaben.de/bild/a981_1.jpg)

</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Vorteile:__

- viele Quellen als externe Wärmezufuhr möglich (Solar, Abwärme, Verbrennungen)

- leiser lauf, hoher Wirkungsgrad

- keine Ventilsteuerung (wie beim Verbrennungs-Motor)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Nachteile:__ 

- Leistung und Kaltstart träge (anschubsen)

- hohe Anforderungen an Dichtungen und Wärmetauscher

- teuer, wenn hohe Leistung gefordert ist

</div>

</section>

[Video-Idealisierter-SterlingMotor](https://www.youtube.com/watch?v=cxqBK_mwKP4)


## 13. 8. Thermodynamische Grundlagen - Übersicht

__Zustandsänderung für ein geschlossenes System__

| | | | | |
| | isochor | isobar | isotherm | adiabatisch |
| Bedingung | keine Volumenänderung <br> $\Rightarrow \Delta V=0$ | keine Druckänderung <br> $\Rightarrow \Delta p=0$ | keine Temperaturänderung <br> $\Rightarrow \Delta T=0$ | kein Wärmaustausch <br> $\Rightarrow \Delta Q=0$ |
| 1. Hauptsatz | $$W=0$$ $$\Rightarrow Q=\Delta U$$ | $$\Delta U=Q+W$$ | $$\Delta U = 0$$ $$\Rightarrow Q = - W $$ | $$Q=0$$ $$\Delta U = W$$ |
| Beziehungen | $$\dfrac{p}{T}=\text{konst.}$$  | $$\frac{V}{T}=\text{konst.} $$ | $$p \cdot V = \text{konst.} $$| $$p\cdot V^{\kappa}=\text{konst.}$$ $$T\cdot V^{\kappa-1}=\text{konst}$$|
| Wärmemenge | $$Q=c_v\cdot m\cdot \Delta T$$| $$Q=c_p\cdot m\cdot \Delta T$$ | $$Q=-W$$ | $$Q=0$$ |
| Volumentarbeit | $$W=0$$ | $$W=-p\,(V_2-V_1)$$ | $$W=-p_1\cdot V_1\displaystyle\int_{V_1}^{V_2} \frac{1}{V}\,\mathrm{d}V$$ $$W=-p_1\cdot V_1 \cdot \ln\left(\frac{V_2}{V_1}\right)$$ | $$ W= -p_1\cdot V_1^\kappa\displaystyle\int_{V_1}^{V_2} \frac{1}{V^\kappa}\,\mathrm{d}V$$ |

### Übungsaufgabe Stirling-Prozess

1. ![Stirling](https://physikaufgaben.de/bild/a981_1.jpg) Die Abbildung zeigt das p(V)-Diagramm eines Stirling'schen Kreisprozesses. Welches V(T)-Diagramm passt zu diesem Kreisprozess?

<p style="margin-left:10%">

![Stirling1](https://physikaufgaben.de/bild/a981_2.jpg)

- [[X]] A
- [[ ]] B
- [[ ]] C

</p>

---

2. Die Arbeitsweise einer Wärmekraftmaschine wird durch einen Stirling’schen Kreisprozess idealisiert. Dieser besteht aus zwei isothermen und zwei isochoren Zustandsänderungen.

---

2. 1. Herleitung der Volumenarbeit

<p style="margin-left:10%">

Leiten Sie ausgehend von der allgemeinen Integralschreibweise $W = -\int_{V_1}^{V_2} p(V) \, \mathrm{d}V$ die Gleichung zur Berechnung der Volumenarbeit $W_V$ für eine isotherme Zustandsänderung eines idealen Gases her.

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

1. Nutzen Sie die thermische Zustandsgleichung $p \cdot V = n \cdot R \cdot T$, um den Druck $p$ als Funktion des Volumens $V$ auszudrücken: $p(V) = \frac{n \cdot R \cdot T}{V}$.
2. Da die Temperatur $T$ bei einer isothermen Änderung konstant ist, können $n, R$ und $T$ vor das Integral gezogen werden.
3. Integrieren Sie $\frac{1}{V}$ über das Intervall $[V_1; V_2]$. Das Ergebnis ist der natürliche Logarithmus $\ln(V)$.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

$W = -\int_{V_1}^{V_2} \frac{n \cdot R \cdot T}{V} \, \mathrm{d}V$

$W = -n \cdot R \cdot T \cdot \int_{V_1}^{V_2} \frac{1}{V} \, \mathrm{d}V$

$W = -n \cdot R \cdot T \cdot [\ln(V)]_{V_1}^{V_2}$

$\mathbf{W = -n \cdot R \cdot T \cdot \ln\left(\frac{V_2}{V_1}\right)}$

</details>

</p>

---

2. 2. Berechnung der Nutzarbeit

<p style="margin-left:10%">

Dieser Prozess wird mit einer Stoffmenge von $n = 2,0 \, \text{mol}$ eines idealen Gases zwischen den Volumina $V_1 = 2000 \, \text{cm}^3$ und $V_2 = 5000 \, \text{cm}^3$ durchgeführt. Die beteiligten Temperaturen betragen $T_{hoch} = 630 \, \text{K}$ und $T_{niedrig} = 330 \, \text{K}$.

Ermitteln Sie die bei einem vollständigen Umlauf verrichtete Nutzarbeit $W_{nutz}$.

@rangeQuiz2( $W_{nutz}$ , 4571.0, $\mathrm{J}$ )

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

Die Nutzarbeit eines Stirling-Prozesses ergibt sich aus der Summe der Volumenarbeiten der beiden isothermen Schritte (die isochoren Schritte verrichten keine Arbeit).

$W_{nutz} = |W_{1 \to 2}| - |W_{3 \to 4}|$

$W_{nutz} = n \cdot R \cdot \ln\left(\frac{V_2}{V_1}\right) \cdot (T_{hoch} - T_{niedrig})$

Setzen Sie die Werte ein: $R \approx 8,314 \, \frac{\text{J}}{\text{mol} \cdot \text{K}}$, $\Delta T = 300 \, \text{K}$ und das Volumenverhältnis $2,5$.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

$W_{nutz} = 2,0 \, \text{mol} \cdot 8,314 \, \frac{\text{J}}{\text{mol} \cdot \text{K}} \cdot (630 \, \text{K} - 330 \, \text{K}) \cdot \ln\left(\frac{5000}{2000}\right)$

$W_{nutz} = 16,628 \cdot 300 \cdot \ln(2,5)$

$W_{nutz} \approx 4988,4 \cdot 0,9163$
$\mathbf{W_{nutz} \approx 4571 \, J}$

Pro Umlauf verrichtet die Maschine eine Nutzarbeit von ca. $4,57 \, \text{kJ}$.

</details>

</p>

---

2. 3. Wirkungsgrad


<p style="margin-left:10%">

Geben Sie den maximal möglichen Wirkungsgrad (Carnot-Wirkungsgrad) für diese Maschine an.

@rangeQuiz2( $\eta_{max}$ , 0.476, )

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Der maximale Wirkungsgrad hängt nur von den Temperaturen ab:

$\eta_{max} = 1 - \frac{T_{niedrig}}{T_{hoch}} = 1 - \frac{330 \, \text{K}}{630 \, \text{K}}$

$\mathbf{\eta_{max} \approx 0,476}$ (bzw. $47,6 \%$).

</details>

</p>

<!-- style="display:block" -->
<div style="display:none">

## 13. 9. Energiebilanz einer Wärmekraftmaschine

<H3>Beispiel: Stirling-Prozess</H3>

<section class="flex-container">

<div class="flex-child-1" style="min-width:200px; margin-bottom: -10px">

![Stirling6](https://diversewolken.ddns.net/nextcloud/s/5ExyaAtk4gLjjAR/download)

</div>

<div class="flex-child-1" style="min-width:200px; margin-bottom: -10px">

| __1->2:__ | __Isotherme Expansion__ | 
| $\Delta U=0 \Rightarrow$  | $W_{1\rightarrow2}=-Q_{1\rightarrow2} $  | 

Das System nimmt Wärmeenergie $\blue{Q_{1\rightarrow2}}$ auf.

---

| __3->4:__ | __Isotherme Kompression__ | 
| $\Delta U=0 \Rightarrow$  | $W_{3\rightarrow4}=-Q_{3\rightarrow4} $  | 

Das System gibt die Wärmeenergie $\red{Q_{3\rightarrow4}}$ ab.

</div>

<div class="flex-child-1" style="min-width:300px; margin-bottom: -10px">

| __2->3:__ | __Isochore Abkühlung__ | 
| $W_{2\rightarrow3}=0 \Rightarrow$  | $\Delta U_{2\rightarrow3}=Q_{2\rightarrow3} $  | 

Das System gibt die Wärmeenergie $\orange{Q_{2\rightarrow3}}$ ab.

---

| __4->1:__ | __Isochore Erwärmung__ | 
| $W_{4\rightarrow1}=0 \Rightarrow$  | $\Delta U_{1\rightarrow4}=Q_{4\rightarrow1} $  | 

Das System nimmt die Wärmeenergie $\green{Q_{4\rightarrow1}}$ auf.

</div>

</section>

---

<H4>__Energiebilanz:__</H4>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> 1. Da die Temperaturenänderungen 2->3 und 4->1 betragsmäßig gleich sind, gilt:
>
> $$\green{Q_{4\rightarrow1}}=-\orange{Q_{2\rightarrow3}}$$

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


> 2. Aufgrund der Energieerhaltung ($\Delta U = 0$) gilt für die geleistete Arbeit
>
> $$\purple{W} = \blue{Q_{1\rightarrow2}} + \red{Q_{3\rightarrow4}}$$


</div>

</section>

---

<H4>__Wirkungsgrad:__</H4>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

> Der Wirkungsgrad $\eta$ ist definiert als die genutzte Energie (hier Volumenarbeit $\purple{W}$) pro zugeführter Energie (hier Wärme $\blue{Q_{1\rightarrow2}}$.)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


> $$ \eta = \dfrac{\purple{W}}{\blue{Q_{1\rightarrow2}}} = \dfrac{\blue{Q_{1\rightarrow2}}+\red{Q_{3\rightarrow4}}}{\blue{Q_{1\rightarrow2}}} = 1 + \dfrac{\red{Q_{3\rightarrow4}}}{\blue{Q_{1\rightarrow2}}} = 1 - \dfrac{T_2}{T_1}$$


_Hinweis (isotherm): $Q = -W = n \cdot R \cdot T \cdot \ln\frac{V_\text{Ende}}{V_\text{Anfang}}$_


</div>

</section>

</div>

<!-- style="display:block" -->
<div style="display:none">

## 13. 10. Wärmepumpe: Umkehrung der Wärmekraftmaschine

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Wärmepumpe1](https://diversewolken.ddns.net/nextcloud/s/5mGXTZyBbgGygNp/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


>Jede @color(__Wärmekraftmaschine__, red) kann als @color(__Wärmepumpe__, blue) betrieben werden, wenn der Kolben angetrieben und der Kreisprozess in die entgegengesetze Richtung durchlaufen wird.

Die Wärmeenergie $\blue{Q_{1\rightarrow2}}$ wird von der niedrigen Temperatur $T_{low}$ auf die höhere Temperatur $T_{high}$ gepumpt.

<H4>Wirkungsgrad</H4>

Der _technische Wirkungsgrad_ ist dann

$$ \eta_{\text{WP}} = \dfrac{\red{Q_{3\rightarrow4}}}{\purple{W}} = \dfrac{\red{Q_{3\rightarrow4}}}{\red{Q_{3\rightarrow4}}+\blue{Q_{1\rightarrow2}}}=\dfrac{T_{\text{high}}}{T_{\text{high}}-T_{\text{low}}} $$

$\eta_{WP}$ ist offensichtlich größer als 1. 

</div>

</section>

<H4>Beispiel: Kühlschrank</H4>

Ein Haushaltskühlschrank arbeitet bei einer typischen Umgebungstemperatur von etwa 25°C und einer Temperatur im Inneren von etwa 4°C. 

1. Ermitteln Sie den maximal möglichen (idealen) technischen Wirkungsgrad dieser Wärmepumpe.

<p style='margin-left:10%'>

@rangeQuiz2($\eta_{\text{WP}}$, 13.95 , )

</p>

</div>