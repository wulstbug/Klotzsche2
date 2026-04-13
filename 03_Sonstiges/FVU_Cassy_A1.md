<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://www.sciencedaily.com/images/1920/Quantum-Clock.webp

@style
.lia-effect__circle {
    display: none !important;
} 
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 20px;
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

@media (max-width: 500px) {
    .flex-child,
    .flex-child-1,
    .flex-child-2,
    .flex-child-3,
    .flex-child-4,
    .flex-child-5,
    .flex-child-6,
    .flex-child-7,
    .flex-child-8 {
        flex: 100%; /* Makes the child divs take up the full width on slim devices */
        margin-right: 0; /* Removes the right margin */
    }
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
    display: block;
}

@end

@onload
window.LIA.settings.font_size = 2


const canvas = document.querySelector('.lia-canvas')
if (canvas) {
  canvas.classList.remove('lia-navigation--visible')
  canvas.classList.add('lia-navigation--hidden')
}

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
<div style="float:left;margin-left:10px">
@2
</div>
</div>
@end

@rangeQuiz20
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
    input = Math.abs(eval(input)-(@1))/Math.abs(@1)
    input <= 0.2
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

@rangeQuiz0
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

## Teil 2 - Automatisierte Messwertaufname von Spannung und Stromstärke

<!-- 
    data-randomize 
    data-solution-button=false 
    data-max-trials="5"
-->
> Mit dem Cassy Messgerät können sehr viele [[ (__physikalische Größen__) | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]]  gemessen werden. Viele Größen benötigen einen eigenen [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | (__Sensor__) | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> <br> Für die __Spannung__ $U$ nutzen wir: [[ __physikalische Größen__ | (__Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ ) | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> Für die __Stromstärke__ $I$ nutzen wir [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | ( __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ ) | __Sensor__ | __Trigger__ | __Messzeit__ | __Messintervall__ ]] . <br> <br> Damit eine Messung automatisiert startet benötigt sie ein __Startsignal__, man nennt das [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | (__Trigger__) | __Messzeit__ | __Messintervall__ ]] . Dieses Startsignal kann z.B. das Überschreiten der Spannung $U>0,5\,\mathrm{V}$ sein. <br> <br> Bevor die Messung gestartet werden kann, muss die Gesamtzeit für die Messung eingestellt werden: die [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | (__Messzeit__) | __Messintervall__ ]] . <br> Außerdem muss  der Zeitabstand zwischen den Messwerten definiert werden, das heißt [[ __physikalische Größen__ | __Kanal A (Stecker: @color(rot, red)+@color(schwarz))__ | __Kanal B (Stecker @color(schwarz)+@color(blau, blue))__ | __Sensor__ | __Trigger__ | __Messzeit__ | (__Messintervall__) ]] .

@color(Löse diesen Merksatz und notiere ihn anschließend in deinem Hefter!, blue)



