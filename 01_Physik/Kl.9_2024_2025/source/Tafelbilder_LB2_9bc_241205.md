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

mode: presentation

-->

## 2.12 Der Transformator

@timer(15,00)

<br> <br> <br>

| ![Trafo1](https://diversewolken.ddns.net/nextcloud/index.php/s/zbqC3RJzMLi6sM9/download) | ![Trafo2](https://diversewolken.ddns.net/nextcloud/index.php/s/9fcnRM9Rdy3Amkm/download) | ![Trafo3](https://diversewolken.ddns.net/nextcloud/index.php/s/qsKCjt4j7EwTEyj/download) |

{{1}}
**************
@color(_Bearbeite mit Hilfe des Tablets die Punkte 2.12-2.12.2_,blue)

<details>

<summary>Tablets 9b</summary>

![Tablets_9b](https://diversewolken.ddns.net/nextcloud/index.php/s/BfXtBqXZNTb58KH/download)

</details>

<details>

<summary>Tablets 9c</summary>

![Tablets_9c](https://diversewolken.ddns.net/nextcloud/index.php/s/npmiF6zXeoDtyKD/download)

</details>

**************

### 2.12.1 Definition

@color(Übernimm folgendes Tafelbild in deinen Hefter , blue)

![TB-Transformator](https://diversewolken.ddns.net/nextcloud/index.php/s/GzrAGpEeLCcJBDQ/download)

__Formelzeichen:__

<p style="margin-left:10%">

$U_p$ .. Primärspannung

$U_s$ .. Sekundärspannung

$N_p$ .. Windungszahl auf Primärseite

$N_s$ .. Windungszahl auf Sekundärseite

</p>

### 2.12.2 Funktionsweise Trafo (Übung+Hefter)

@color(_Bringe die Sätze von links nach rechts in die richtige Reihenfolge. <br> Notiere Sie anschließen im Hefter._ , blue)

<iframe src="https://learningapps.org/watch?v=pyuu71zx524" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### 2.12.2 Funktionsweise Trafo (Übung)

@color(_Bringe die Bilder von links nach rechts in die richtige Reihenfolge._, blue)

<iframe src="https://learningapps.org/watch?v=p40qc7nht24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### 2.12.3 Hoch-/Heruntertransformieren von Spannungen

{{0-1}}
********
<p style="color:blue">

1. Lies den Text zur Hochtransformation oder Heruntertransformation von Spannungen.

2. Definiere den Begriff Hochtransformation oder Heruntertransformation und notiere dir zwei Beispiele in deinen Hefter.

3. Tauscht euch mit einem Partner gemeinsam über die Texte aus.

</p>
********

{{1}}
*************
![TB_HochRunterTrafo](https://diversewolken.ddns.net/nextcloud/index.php/s/wcMmNWL9DcBCX82/download)

@color(_Übernimm das Tafelbild in den Hefter_, blue)

<br>

@color(_Probiere anschließend das Domino-Spiel_, blue)
*************

### 2.12.4 Die Transformator-Gleichung

@color(_Übernimm das Tafelbild zur Transformator-Gleichung in deinen Hefter. Löse anschließend die Aufgaben_, blue)

![Transformator-Gleichung](https://diversewolken.ddns.net/nextcloud/index.php/s/N7kn35eZQBsaxET/download)

{{1}}
************
__1. Übung: Transformator__

<iframe src="https://learningapps.org/watch?v=pqtryg2mt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

__2. Idealer Transformator: Berechnen__

<iframe src="https://learningapps.org/watch?v=pyk3q81sk24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>
************