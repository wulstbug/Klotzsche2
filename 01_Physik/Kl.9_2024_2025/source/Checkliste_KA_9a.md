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


# Checkliste Klassenarbeit Physik 21.01.25

> Liebe 9a,
>
> die KA Physik enthält das Stoffgebiet 2. Energieversorgung komplett. Auf dieser Seite sind die Schwerpunkte, in Klammern die Nummern der Überschriften. 
>
> Die Übungsaufgaben aus dem Unterricht findet ihr auf den folgenden Seiten.

Grundlagen sind: 

- 2.1. Energieformen (Übung 2.1)

- 2.2. Energieerhaltung (2.2)

- 2.3. Energieflussdiagramme (EFD) = Energieumwandlungsketten 


Lernschwerpunkte sind:

- 2.4. Wirkungsgrad (Übung -> 2.4.1 & 2.4.2)

- 2.5. Energiebedarf moderner Gesellschaften (es müssen keine Zahlen auswendig gelernt werden, aber ein Energieverteilungsdiagramm [siehe Hefter] soll interpretiert werden können, z.B. _Schätze den Anteil der erneuerbaren Energien im Jahr 2000_)

- 2.5. Begriff __primäre Energiequelle/primärer Energieträger__ und Beispiele

- 2.6. Bereitstellung elektrischer Energie
  
    - Gründe für Nutzung elektrischer Energie

    - Grundprinzip der Energieumwandlung (EFD) (2.3) einzelner Kraftwerke (z.B. Kohlekraftwerk, Windkraftwerk, Wasserkraftwerk) 
   
    - gemeinsame Elemente aller Kraftwerkstypen (außer Solarkraftwerk)

- 2.7. Funktionsweise eines Generators (Aufbau, Bezeichnungen, Funktionsprinzip) (Übung: Fragen zum Generator 2)

- 2.8. Induktionsgesetz (Gesetz können, Einflussfaktoren auf induzierte Spannung, Grundprinzip der Energieumwandlung bei Induktion)

- 2.9. Induktion am Generator -> Wechselspannung

    - Eigenschaften der Wechselspannung (z.B. am Beispiel Haushaltssteckdose -> Aufgabe 2.8.1)

    - -> Aufgaben zur Wechselspannung 1-4

- Transformator (Aufbau, Funktionsweise, Transformatorgleichung, Unterschied zwischen idealem und realem Transformator) -> Übung 2.12.2 / 2.12.3

- Hochtransformieren & Heruntertransformieren

- Wiederholung Transformator -> Übung 2.12.4

- Funktionsweise Kernkraftwerk, Kernspaltung (Was ist das?),Kettenreaktion, Nuklidschreibweise


### 2.1. _Übung: Zuordnung Energieformen_

Übung 1: _Zuordnung Energieformen_

<iframe src="https://learningapps.org/watch?app=23986132" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

Übung 2: _Zuordnung Energieformen_
<iframe src="https://learningapps.org/watch?app=28854190" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>


### 2.4.1 Übung: Wirkungsgrad am Beispiel von Glühlampe und LED

> __Energieumwandlungen von__

<p class="newspaper">

> __Glühlampe__

{{1}}
*********
<!-- style="width:50%" -->
``` ascii
            '----------'
            | Lichten. |
           ^|----------|
'--------'/ |  5 J     |
| el. En.|  '----------'
|--------|  
|  100 J |
'--------'\ '----------'
           v| Wärmeen. |
            |----------|
            |  95 J    |
            '----------'
```
*********

<p class="cb">

> __LED__

{{2}}
*********

<!-- style="width:50%" -->
``` ascii
            '----------'
           ^| Lichten. |
'--------'/ |----------|
| el. En.|  |  40 J    |
|--------|  '----------'
|  100 J |
'--------'\ '----------'
           v| Wärmeen. |
            |----------|
            |  60 J    |
            '----------'
```

*********

</p>

</p>

> __Aufgabe:__ Bestimme den Wirkungsgrad von Glühlampe und LED.

<p class="newspaper">

{{3}}
**************

__Glühlampe__

geg.: <br>
 
$\hspace{0.5cm}$ $E_{el}$ = 100 J

$\hspace{0.5cm}$ $E_{Licht}$ = 5 J

$\hspace{0.5cm}$ $E_{therm}$ = 95 J

ges.: <br>

$\hspace{0.5cm}$ $\eta$

{{4}}
**************
Lsg.:

$\hspace{0.5cm}$ $\eta = \dfrac{E_{nutz}}{E_{zu}} = \dfrac{E_{Licht}}{E_{el}}$

$\hspace{0.5cm}$ $\eta = \dfrac{5 J}{100 J} = 0,05 = 5\%$ 
**************

**************

<p class="cb">

__LED__

{{5}}
*************
geg.: <br>
 
$\hspace{0.5cm}$ $E_{el}$ = 100 J

$\hspace{0.5cm}$ $E_{Licht}$ = 40 J

$\hspace{0.5cm}$ $E_{therm}$ = 60 J

ges.: <br>

$\hspace{0.5cm}$ $\eta$

Lsg.:
************

{{6}}
*************
$\hspace{0.5cm}$ $\eta = \dfrac{E_{nutz}}{E_{zu}} = \dfrac{E_{Licht}}{E_{el}}$

$\hspace{0.5cm}$ $\eta = \dfrac{40 J}{100 J} = 0,4 = 40\% $ 
*************


</p>

</p>

{{7}}
***********
> __Vergleich:__ Die LED wandelt die elektrische Energie viel effizienter in Licht um als die Glühlampe, denn sie hat einen höheren Wirkungsgrad (40% > 5%)
***********

### 2.4.2 Übung: Wirkungsgrad eines Benzinmotors

> Über die Benutzung eines Benzinmotors bei einem Auto sind folgende Dinge bekannt:
>
> $E_{chem} = 6000 J$
>
> $E_{kin} = 1800 J$ (_hier sei Rotationsenergie enthalten_)
>
> $E_{therm} = 3900 J$
>
> $E_{el} = 150 J$.

__Aufgabe:__ Berechne den Wirkungsgrad, wenn es das Ziel ist:

- a) mit dem Auto zu fahren

- b) das Auto als Heizung zu verwenden

- c*) die Glühlampe im Auto zum Lesen zu verwenden.

__Lösung überprüfen:__ 

{{1}}
*************
<!-- data-solution-button=off -->
a) $\eta$ = [[ 0,3 ]] 
[[?]] Überlege, welches im Fall a) die zugeführte und welches die genutze Energieform ist. Verwende dann die Formel für $\eta$
[[?]] Die zugeführte Energieform beim Benzinmotor ist chemische Energie. Die genutzte Energieform (wenn man fahren will) ist kinetische Energie.
[[?]] $\eta = \frac{E_{kin}}{E_{chem}}=\frac{1800 J}{6000 J}$
*************

{{2}}
*************
<!-- data-solution-button=off -->
b) $\eta$ = [[ 65 ]] %
[[?]] Hier ist $\eta$ in Prozent gefordert
[[?]] Überlege, welches im Fall a) die zugeführte und welches die genutze Energieform ist. Verwende dann die Formel für $\eta$
[[?]] Die zugeführte Energieform beim Benzinmotor ist chemische Energie. Die genutzte Energieform (wenn man heizen will) ist thermische Energie.
[[?]] $\eta = \frac{E_{therm}}{E_{chem}} \cdot 100\%=\frac{3900 J}{6000 J}\cdot 100\%$
*************

{{3}}
*************
<!-- data-solution-button=off -->
c) $\eta$ = [[ 0,125 ]] %
[[?]] Dies ist eine zweistufige Energieumwandlung
[[?]] Zunächste wird chemische Energie vom Motor in elektrische umgewandelt. Dann wird die elektrische Energie von der Glühlampe in Lichtenergie umgewandelt
[[?]] chem -> el: 6000 J -> 150J. <br> Im Anschluss muss der Wirkungsgrad der Glühlampe berücksichtigt werden (siehe 2.4.1)
[[?]] Mit dem Wirkungsgrad der Glühlampe von 5% ergibt sich, dass die 150J elektrische Energie in $150\cdot0,05=7,5 J$ Lichtenergie umgewandelt werden.
[[?]] Der gesamte Wirkungsgrad beträgt also $\eta = \frac{7,5 J}{6000 J} \cdot 100\% = 0,125 \%$
*************

{{1}}
*************
_Hinweis: Klicke auf die Glühlampen für Lösungshinweise_
*************

### 2.8.1 Übung: Fragen zum Generator

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

### 2.10.1 Aufgaben zur Wechselspannung


Bestimme für die Netzspannung einer Haushaltssteckdose Amplitude, Periodendauer und Frequenz (_Achte auf die Einheiten_).

![Netzspannung](https://diversewolken.ddns.net/nextcloud/index.php/s/jmBedzyFa2xBTLF/download "Quelle: https://www.sonnentaler.net/dokumentation/wiss/elektrizitaet/grundlagen/elektrik-im-haus/")<!-- style="min-width:60%"-->

@color(_Hinweis: 1000 ms = 1 s_, red)

__Lösungen:__

1. Amplitude 

@rangeQuiz2($\hspace{1cm}$ $\hat{U}$, 325, $V$)

2. Periodendauer 

@rangeQuiz2($\hspace{1cm}$$T$, 0.02, $s$)

3. Frequenz

@rangeQuiz2($\hspace{1cm}$$f$, 50, $\dfrac{1}{s}$)

### 2.10.2. Aufgaben zur Wechselspannung

<iframe src="https://learningapps.org/watch?v=p23wxsi7224" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### 2.10.3. Quiz Generator

[QuizZumGenerator](https://www.leifiphysik.de/elektrizitaetslehre/induktion-und-transformator/aufgabe/quiz-zum-generator)

### 2.12.2. Übungen: Funktionsweise Trafo

@color(_Bringe die Sätze von links nach rechts in die richtige Reihenfolge. <br> Notiere Sie anschließen im Hefter._ , blue)

<iframe src="https://learningapps.org/watch?v=pyuu71zx524" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

@color(_Bringe die Bilder von links nach rechts in die richtige Reihenfolge._, blue)

<iframe src="https://learningapps.org/watch?v=p40qc7nht24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### 2.12.3. Übung: Berechnungen Trafo

__1. Übung: Transformator__

<iframe src="https://learningapps.org/watch?v=pqtryg2mt24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

__2. Idealer Transformator: Berechnen__

<iframe src="https://learningapps.org/watch?v=pyk3q81sk24" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

### 2.12.4. Wiederholungübung: Transformator 


1. Bei einem idealen Transformator sei die Sekundärwindungszahl größer als die Primärwindungszahl. Kreuze die richtige Aussage an.

<p style="margin-left:5%;margin-right:5%">

- [[ ]] $U_s < U_p$
- [[ ]] $U_s = U_p$
- [[x]] $U_s > U_p$

</p>

2. Betrachte folgende Transformator-Daten. Entscheide, ob der Transformator zum Hoch- und Heruntertransformieren verwendet wir. <br> _Für das Übersetzungsverhältnis $n$ gilt: $n = \frac{U_p}{U_s} = \frac{N_p}{N_s}$_.<br> @color(Ergänze dieses Übersetzungsverhält in deinem Hefter unter __2.12.4 Transformatorgleichung__, blue)

<p style="margin-left:5%;margin-right:5%">

<p class="newspaper3">

$n=5$

<!-- data-solution-button="off" -->
- [[ ]] Hochtransformiern
- [[x]] Heruntertransformieren
- [[ ]] weder noch

<p class="cb">

$N_p=1000; N_s=50000$

<!-- data-solution-button="off" -->
- [[x]] Hochtransformieren
- [[ ]] Heruntertransformieren
- [[ ]] Weder noch

<p class="cb">

$N_p=100; N_s=100$

<!-- data-solution-button="off" -->
- [[ ]] Hochtransformieren
- [[ ]] Heruntertransformieren
- [[x]] Weder noch

</p>

</p>

</p>

</p>

4. ![TrafoHaus](https://upload.wikimedia.org/wikipedia/commons/1/19/Elfmorgenbruch_220kV-Transformator.jpg) In Transformatorstationen wird die Elektrizität des regionalen Verteilnetzes mit der Mittelspannung ca. 20 kV zur Versorgung der Niederspannungsendkunden auf die im Ortsnetz verwendeten 400-V-Leiter-Leiter-Spannung transformiert. Wähle die Transformator-Einstellungen aus, die hier verwendet werden können. <br> _Hinweise: 1kV = 1000 V_

<p style="margin-left:5%;margin-right:5%">

<p class="newspaper3">

<!-- data-solution-button="off" -->
- [[x]] $N_s < N_p$
- [[ ]] $N_s = N_p$
- [[ ]] $N_s > N_p$

<p class="cb">

<!-- data-solution-button="off" -->
- [[ ]] $n=0,1$
- [[ ]] $n=10$
- [[x]] $n=50$

<p class="cb">

<!-- data-solution-button="off" -->
- [[x]] $N_p=50000; N_s=1000$
- [[ ]] $N_p=20000; N_s=100$
- [[ ]] $N_p=10000; N_s=200$

</p>

</p>

</p>

</p>

3. Für einen unbelasteten Transformator sind zeilenweise die folgenden Daten bekannt. Ergänze die fehlenden Werte. Für das Übersetzungsverhältnis $n$ gilt: $n = \frac{U_p}{U_s} = \frac{N_p}{N_s}$

<p style="margin-left:5%;margin-right:5%">

---

a)

<!-- data-solution-button="off" -->
| $N_p$ | $N_s$ | $U_p$ | $U_s$ | n |
| 2500 | 500  | 100V   | [[ 20 ]] V     | [[ 5 ]] |

---

b)

<!-- data-solution-button="off" -->
| $N_p$ | $N_s$ | $U_p$ | $U_s$ | n |
| 250 | [[ 1000 ]] | [[ 10 ]] V | 40V   | 0,25 |

---

c)

<!-- data-solution-button="off" -->
| $N_p$ | $N_s$ | $U_p$ | $U_s$ | n |
| 125 | [[ 1000 ]]     | 3V    | 240V | [[ 0,0125 ]] |

</p>

