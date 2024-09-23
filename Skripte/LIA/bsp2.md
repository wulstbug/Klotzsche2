<!--
author: Christian Golnik

language: de

link: https://gist.githubusercontent.com/andre-dietrich/3c69f68b2c4d80c8c6eb177229ae1ae8/raw/31cde15c4a7f3c2eda7d5ebdea440205f366acad/hideCircle.css

-->

# Lösung: Beispielrechnung Dichte

Lösung: 

geg.: 

$\hspace{1cm}$ Volumen $V = 10\text{m}\cdot 7\text{m} \cdot 8\text{m} = 560\text{m}^3$

$\hspace{1cm}$  Masse $m=700\text{t}=700.000\text{kg}$

ges.: 
$\hspace{1cm}$ Dichte $\rho$

Lsg.: 

$\hspace{1cm}$  $\rho = \dfrac{m}{V} = \dfrac{700.000\text{kg}}{560\text{m}^3}$

<!-- data-solution-button="off" -->
$\hspace{1cm}$  $\rho = $ [[ 1250 ]] $\frac{\text{kg}}{\text{m}^3}$

<!-- data-solution-button="off" -->
Antwort: Der Körper [[ (sinkt) | schwimmt ]], da seine Dichte [[ kleiner | (größer) ]] als die Dichte von Wasser ist.

Anhand der Dichte könnte das Material des Körpers [[ Ziegel ]] sein.


# Test-Multiply

__Experiment:__

> d = <input type="number" default="0" min="0" max="10" id="d" size="5"> m $ \hspace{0.5cm}$ a = <input type="number" default="0" min="0" max="10" id="a" size="5"> m $\hspace{0.5cm}$ e = <input type="number" default="0" min="0" max="10" id="e" size="5">m

$\lambda = $
<script input="button">

    let d = document.getElementById("d").value;
    let a = document.getElementById("a").value;
    let e = document.getElementById("e").value;

    a*d*e
</script>
m
