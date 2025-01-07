<!--
author: Christian Golnik

language: de

@style
.lia-effect__circle {
    display: none !important;
}
.lia-slide__footer {
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
<div style="float:left">
@0$\ $=$\ $ 
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


-->

# Übungsblatt: Brüche, Dezimalbrüche und Prozentrechnung

<p class="newspaper">

__Aufgabe 1: Brüche erweitern__
Erweitere die folgenden Brüche mit der angegebenen Zahl:

1. $\frac{3}{5}$ erweitern mit 2 = [[ 6 ]] / [[ 10 ]]
2. $\frac{7}{8}$ erweitern mit 4 = [[ 28 ]] / [[ 32 ]]
3. $\frac{2}{3}$ erweitern mit 5 = [[ 10 ]] / [[ 15 ]]

__Aufgabe 2: Brüche kürzen__

Kürze die folgenden Brüche vollständig:

1. $\frac{12}{16}$ = [[ 3 ]] / [[ 4 ]]
2. $\frac{18}{27}$ = [[ 2 ]] / [[ 3 ]]
3. $\frac{15}{35}$ = [[ 3 ]] / [[ 7 ]]

__Aufgabe 3: Brüche in Dezimalzahlen umwandeln__

Wandle die folgenden Brüche in Dezimalzahlen um:

1. $\frac{1}{4}$ = [[ 0.25 ]]
2. $\frac{3}{5}$ = [[ 0.6 ]]
3. $\frac{7}{8}$ = [[ 0.875 ]]

<p class="cb">

__Aufgabe 4: Dezimalzahlen in Brüche umwandeln__

Wandle die folgenden Dezimalzahlen in Brüche um (bitte vollständig gekürzt):

1. $0.5$ = [[ 1/2 ]]
2. $0.75$ = [[ 3/4 ]]
3. $0.2$ = [[ 1/5 ]]

__Aufgabe 5: Prozentrechnung__

Berechne die folgenden Prozentaufgaben:

1. Wie viel sind 25 % von 200? [[ 50 ]]
2. Wie viel sind 60 % von 150? [[ 90 ]]
3. Wie viel sind 12 % von 50? [[ 6 ]]

__Aufgabe 6: Prozent in Brüche und Dezimalzahlen umwandeln
Wandle die folgenden Prozentangaben in Brüche und Dezimalzahlen um:__

1. 50 % = [[ 1/2 ]] und [[ 0.5 ]]
2. 25 % = [[ 1/4 ]] und [[ 0.25 ]]
3. 75 % = [[ 3/4 ]] und [[ 0.75 ]]

---

Viel Erfolg bei den__Aufgaben! Überprüfe deine Ergebnisse, indem du die Zahlen in den Klammern kontrollierst.

</p>

</p>