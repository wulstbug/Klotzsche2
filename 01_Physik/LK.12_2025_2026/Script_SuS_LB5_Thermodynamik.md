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

# LB 13 Thermodynamik (Wärmelehre)

![Thermodynamik](https://diversewolken.ddns.net/nextcloud/s/SfR8K6Tn6mDEFkf/download)

### 13. 1. Einführung

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


### 13. 2. Zustandsgleichung für das ideale Gas

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

@rangeQuiz2($W$,0,$\mathrm{J}$)

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