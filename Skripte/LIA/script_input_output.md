# Scripte

Was vielleicht für den Physik-Kurs interessant wäre, wäre die Nutzung von Scripten, diese funktionieren in LiaScript etwas anders:

<script>99**12</script>

das Ergebnis wird ausgerechnet und dargestellt ... Solche einfachen Scripte können auch miteinander und mit einer Eingabe verknüpft werden:

Hier ein kleiner Schiebe-Regler: <script output="x" value="12" input="range">@input</script> ... hier einmal auf die 12 klicken und den Wert verändern ...

Und hier ein anderes Script:
<script output="x">
let quadrat = @input(`x`)**2

"LIASCRIPT: $ @input(`x`)^2 = " + quadrat + "$"
</script>

# Input CSS oder HTML oder sowas

<input type="number" default="0" min="0" max="10" id="d" size="5">

__Experiment:__

> d = <input type="number" default="0" min="0" max="10" id="d" size="5"> m $ \hspace{0.5cm}$ a = <input type="number" default="0" min="0" max="10" id="a" size="5"> m $\hspace{0.5cm}$ e = <input type="number" default="0" min="0" max="10" id="e" size="5">m

__Wellenlänge des Lichts berechnen:__

> $\lambda = \dfrac{a \cdot d}{e} = $ <script input="button">
    let d = document.getElementById("d").value;
    let a = document.getElementById("a").value;
    let e = document.getElementById("e").value;
    a*d*e
</script> m
