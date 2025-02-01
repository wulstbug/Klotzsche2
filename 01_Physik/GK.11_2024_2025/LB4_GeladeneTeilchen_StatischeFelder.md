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



# Grundkurs Physik 2024/2025 - LB IV - Geladene Teilchen in statischen Feldern

![ProtonCollisionCern](https://getwallpapers.com/wallpaper/full/f/8/b/408658.jpg)

## 1.1. Geladene Teilchen in statischen Magnetfeldern

_Tafelbildvideo zur Lorentzkraft:_

<details>

<summary> Fertiges Tafelbild zum Nachschlagen </summary>

![TB_Lorentzkraft](https://diversewolken.ddns.net/nextcloud/index.php/s/tE56E3MWpqtozxx/download)

</details>

!?[TB_Video_Lorentzkraft](https://youtu.be/f0BNQ6uSvIQ)

## 1.2. Hand-Regel zur Richtungsbestimmung der Lorentzkraft

_Bitte anschauen und ausprobieren_

!?[HandRegel](https://www.youtube.com/watch?v=snM3g4zWeNw)



## Übungsaufgaben zur Lorentzkraft

1. Bitte schau dir zunächst dieses kleine Quiz zur Richtungsbestimmung der Lorentz-Kraft an.

      [QuizZurLorentzkraftRichtung](https://www.leifiphysik.de/elektrizitaetslehre/bewegte-ladungen-feldern/aufgabe/quiz-zu-bewegten-ladungen-im-magnetfeld)

      _Hinweis: Die magnetischen Feldlinien verlaufen vom @color(Nordpol, red) zum @color(Südpol, green)._

---

2. Berechne für das Beispiel im Tafelbild die Lorentzkraft, wenn die Geschwindigkeit des Elektrons $v_e = 1\cdot 10^5 \frac{m}{s}$ und die magnetische Flussdichte $B = 0,2 mT$ beträgt.

<p style="margin-left:10%">

__Endergebnis:__

@rangeQuiz2($F_L$, 3.204e-18 , $N$)

__Zwischenwert:__

@rangeQuiz2($q_e$, 1.602e-19 , $C$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Ermittle mit der Formelsammlung die Ladung eines Elektrons $q_e$. Setze diese Werte in die Formel für die Lorentzkraft ein.

</details>

<details>

<summary> __Lösung__ </summary>

Die Bedingung Geschwindigkeit steht senkrecht auf Feldlinien ist gegeben.

$$F_L = q_e \cdot v_e \cdot B$$

$$ F_L = 1,602\cdot10^{-19}C \cdot 1\cdot 10^5 \frac{m}{s} \cdot 0,2 \cdot 10^{-3} T $$

$$ \underline{F_L = 3,204\cdot 10^{-18} N}$$

</details>


</p>

---

3. Die Lorentzkraft wirkt in jedem Moment senkrecht zur Flugbahn des Elektrons. Nenne die Form der Flugbahn auf der sich das Elektron bewegt, wenn eine Kraft immer senkrecht zur Bewegungsrichtung wirkt.

<p style="margin-left:10%">

- [( )] geradlinig
- [( )] parabelförmig
- [(x)] kreisförmig
- [( )] eckig

</p>

4. Die Flugbahn eines Elektrons in einem statischen magnetischen Feld ist eine Kreisbahn. Die Lorentzkraft $F_L$ wirkt als Zentritedalkraft $F_Z$ (siehe LB I, Kreisbewegung). Ermittle den Radius der Kreisbahn für die Aufgabe 2.

<p style="margin-left:10%">

@rangeQuiz2($r$, 0.00284 ,$m$)

<details>

<summary> __Hinweis zur Lösung__ </summary>

Um die Kreisbahn zu berechnen muss man (wie in der Aufgabe beschrieben) die Formel für die Zentripetalkraft $F_Z$ gleich der Formel für die Lorentzkraft $F_L$ setzen. $F_Z$ wurde in __LB I -> Kreisbewegung__ notiert.

<details style="margin-left:10%">

<summary> __Hinweis zur Formel__ </summary>

$F_Z = F_L$

$\hspace{2cm}$ mit $\boxed{F_Z = \dfrac{m\cdot v^2}{r}}$ und $\boxed{F_L = q \cdot v \cdot B}$

$ \dfrac{m\cdot v^2}{r} = q \cdot v \cdot B$

$\hspace{2cm}$ Nun noch nach $r$ umstellen und ausrechnen.

</details>

</details>

<details>

<summary> __Lösung__ </summary>

Aus dem Ansatz: 
$$F_Z = F_L$$

wobei die Zentripetalkraft $F_Z$ gleich 

$$F_Z = \dfrac{m\cdot v^2}{r}$$ 

und die Lorentzkraft $F_L$ gleich

$$F_L = q \cdot v \cdot B$$

ergibt sich für $r$

$$ r = \dfrac{m\cdot v}{q\cdot B}$$

mit den Werten:

$$ m_e = 9,11\cdot10^{-31} kg$$

$$ q_e = 1,602\cdot10^{-19} C$$

$$ v_e = 1 \cdot 10^5 \frac{m}{s}$$

$$ B = 0,2 mT = 0,2 \cdot 10^{-3} T$$

$$\boxed{\underline{\Rightarrow r = 2,84\cdot10^{-3} m}}$$

</details>

</p>
