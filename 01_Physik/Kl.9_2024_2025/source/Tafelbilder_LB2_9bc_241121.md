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

## Wie funktioniert ein Generator?

!?[MausStrom](https://www.youtube.com/watch?v=Je22SgH8TCk)

## 2.7 Die Funktionsweise eines Generators

Ein einfacher __Generator__ besteht typischer Weise aus einem @color(Magneten, orange) und einer @color(Spule,orange), welche sich im Magnetfeld drehen kann.

{{1}}
**************
<p class="newspaper">

__Skizze:__

![Generator_Skizze](https://asset.conrad.com/media10/isa/160267/c1/-/de/Generator/grundfunktion-eines-generators.jpg)

<p class="cb">

1. Fester Dauermagnet (kann auch Elektromagnet sein) -> @color(__STATOR__,red)

2. Magnetfeld des Dauermagneten (_nicht sichtbar_)

3. Drehbare Spule (hier nur Leiterschleife) -> @color(__ROTOR__,red)

4. Schleifringe

5. Schleifkontakte zur Spannungsabführung

_Hinweis: Magnet und Spule (d.h. **Rotor** und **Stator**) können auch vertauscht sein. Dann ist Magnet beweglich und die Spule fest._

</p>

</p>
**************

{{2}}
**************
__Video: Wie funktioniert ein Generator?__

!?[EVN-Wie-Funktioniert-Ein-Generator](https://www.youtube.com/watch?v=qJCWKwpt1lg)
**************


## 2.8 Grundlage Generator: Das Induktionsgesetz

- @color(Lies LB. S. 53, blue)

- @color(Notiere das Induktionsgesetz [erster Merksatz], blue)

- @color(Ermittle die Einflussfaktoren auf die erzeugte [d.h. induzierte] Spannung, blue)

{{1}}
***********
> __Das Induktionsgesetz:__ Zwischen den Enden einer Spule wird eine Spannung @color(induziert, red), wenn sich das von ihr umfasste Magnetfeld ändert. 
***********

{{2}}
***********
> __Die Induktionsspannung:__ Die Induktionsspannung ab hängt vom 
> 
> 1. Bau der Spule (__Windungszahl__, __Querschnittsfläche__) 
>
> 2. wie schnell und wie stark sich das __Magnetfeld__ in der Spule ändert.
***********

{{3}}
***********
> __Nutzen der Induktion:__ Da bei der Induktion die Bewegung des Rotors in elektrische Spannung "umgesetzt" wird, war es mit der Entdeckung der Induktion (1831) erstmals möglich 
>
>> @color(__mechanische Energie__, blue) in @color(__elektrische Energie__, red) umzuwandeln.
***********

### Fragen zum Generator 2

@timer(08,00)

[Arbeitsblatt-Generator](https://diversewolken.ddns.net/nextcloud/index.php/s/wZo5D9935noCSzw/download)

<p style="margin-right:250px">

@color(Beantwortet die Fragen 1 und 2 auf dem Arbeitsblatt __allein__. Überprüft anschließend mit dem Nachbarn/der Nachbarin gegenseitig die Fragen 3.-8., blue)

1. Bei einem Generator wird das Induktionsgesetz genutzt. Notiere es.

    {1}{<bdi style="color:orange">In einer Spule wird eine Spannung induziert, solange sich das von der Spule umfasste Magnetfeld ändert.</bdi>}

<p class="newspaper">

2. Beschreibe anhand der Skizze den Aufbau eines Wechselstromgenerators. 

    {2}{<bdi style="color:orange"> Ein Wechselstromgenerator besteht aus einem rotierenden Magneten (Rotor) und fest stehenden Induktionsspulen (Stator). </bdi>}

<p  class="cb">

![AB_Generator](https://diversewolken.ddns.net/nextcloud/index.php/s/5m3cZF62Y7DoNms/download)

</p>

</p>

{{3}}
**********
<p class="newspaper">

3. Wahr oder falsch? Wenn sich der Generator schneller dreht, erhöht sich die elektrische Spannung.

     [(X)] wahr
     [( )] falsch

4. Wahr oder falsch? Wenn man die elektrische Spannung am Generator erhöhen will, kann man das Magnetfeld verstärken.

     [(X)] wahr
     [( )] falsch

5. Um die Spannung am Generator zu erhöhen, kann man

     [[ ]] Die Anzahl der Windungen der Spule verringern
     [[X]] Die Anzahl der Windungen der Spule vergrößern
     [[ ]] Die Querschnittsfläche der Spule verkleinern
     [[X]] Die Querschnittsfläche der Spule vergrößern

<p class="cb">

6. Wahr oder falsch? Bei einem Generator muss der Magnet fest sein (Stator) und die Spule drehend (Rotor).

     [( )] wahr
     [(X)] falsch
     
7. Welches Prinzip liegt der Stromerzeugung in einem Generator zugrunde?

     [( )] Thermische Leitung
     [(X)] Elektromagnetische Induktion
     [( )] Kernspaltung
     [( )] Schallwellen

8. Was erzeugt in einem Generator die Spannung?

     [( )]  Eine chemische Reaktion in der Spule
     [( )]  Die Erwärmung des Magneten
     [(X)] Die Bewegung einer Spule in einem Magnetfeld     
     [( )]  Die Anwesenheit eines elektrischen Leiters


</p>

</p>
**********

</p>
