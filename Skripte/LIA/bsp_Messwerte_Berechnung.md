# Berechnung $c_w$-Wert Papierkegel

<p class="newspaper">

__Messwerte:__

> $\hspace{0.5cm}$ geg.:
>
> $\hspace{1cm}$ $\rho_{Luft}=$ <input type="number" default="0" min="0" max="10" size="5" id="rho"> $\dfrac{kg}{m^3}$
>
> $\hspace{1cm}$ $d=$ <input type="number" default="0" id="d" min="0" max="10" size="5"> $m$
>
>$\hspace{1cm}$ $m = $ <input type="number" default="0" id="m" min="0" max="10" size="5"> $kg$
>
>$\hspace{1cm}$ $s=$ <input type="number" default="0" id="s" min="0" max="10" size="5"> $m$
>
>$\hspace{1cm}$ $t=$ <input type="number" default="1" id="t" min="0" max="10" size="5"> $s$
>
>$\hspace{0.5cm}$ ges.:
>
>$\hspace{1cm}$ $c_W$ 

<p class="cb">

__Papierkegel:__

![PapierKegel](https://diversewolken.ddns.net/nextcloud/index.php/s/7Gi2pbyzdAyjD5J/download)

</p>

</p>

{{1}}
*************
> Berechung:
>
>$\hspace{1cm}$ $A=\frac{\pi}{4}{d^2}$=<script input="button">
    let d = document.getElementById("d").value;
    let A = d*d/4*3.1415
    if (isNaN(A)) 0
    else A.toPrecision(3)
 </script> $m^2$
>
>$\hspace{1cm}$ $v=\dfrac{s}{t}=$ <script input="button">
    let t = document.getElementById("t").value;
    let s = document.getElementById("s").value;
    let v = s/t
    if (isNaN(v)) 0
    else v.toPrecision(3)
 </script> $\dfrac{m}{s}$
>
>$\hspace{1cm}$ $c_w=\dfrac{2\cdot F_{Luft}}{A \cdot \rho_{Luft} \cdot v^2}$ = <script input="button">
    let d = document.getElementById("d").value;
    let g = 9.81
    let m = document.getElementById("m").value;
    let t = document.getElementById("t").value;
    let s = document.getElementById("s").value;
    let rho = document.getElementById("rho").value;
    let v = s/t;
    let A = 3.1415/4*d*d
    let result = 2*m*g/(A*rho*v*v)
    if (isNaN(result)) 0
    else result.toPrecision(3)
 </script>
*************
