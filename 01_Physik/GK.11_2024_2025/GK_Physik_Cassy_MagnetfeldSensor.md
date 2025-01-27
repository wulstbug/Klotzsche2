
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
@end

@color
<bdi style="color:@1">@0</bdi>
@end

@orange
<bdi style="color:orange">@0</bdi>
@end

@align
<p style="text-align: @1">@0</p>
@end

@indent
<div style="text-indent:@1">@0</div>
@end

@onload
window.LIA.settings.font_size = 2
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

## 1.4 Schülerexperiment: Messungen der magnetischen Flussdichte

__Teil 1: Bestimmung der magnetischen Flussdichte des Erdmagnetfeldes__

> Aufgabe: Bestimme mit Hilfe des Magnetfeldsensors an dem Cassy-Gerät die magnetische Flussdichte $B_{Erde}$ des Erdmagnetfeldes.

__Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$__

> Aufgabe: Bestimme die magnetische Feldkonstante $\mu_0$ mit Hilfe der Messung der magnetischen Flussdichte B an einer Spule.

@color(Führe die beiden Messungen durch. Erstelle jeweils ein Kurzprotokoll, blue).

_optional (min. 15min)_

__Teil 3: Überprüfung der Proportionalität von $B$ ~ $N$__

> Aufgabe: Überprüfe experimentell die Proportionalität der magnetischen Flussdichte $B$ und der Windungszahl $N$


### Experiment Teil 1: Erdmagnetfeld

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__1.1 Vorbereitung:__

> - recherchiere im Internet die Stärke der magnetischen Flussdichte $B_{Erde}$ des Erdmagnetfeldes in Deutschland
>
> - notiere den Wert und die Quelle
>
> $$ B_{Erde} = ... $$
>
> - erhalte von der Lehrkraft einen Magnetfeldsensor und ein Cassy-Messgerät
>
> - schließe de Magnetfeldsensor an das Cassy-Messgerät (__linke Seite -> Kanal A__) an und lass dir die aktuelle magnetische Flussdichte B anzeigen
>
> - wechsle im Menu zu den Einstellungen von B und
>
>      - wähle als Messmethode axial
>
>      - wähle als Messbereich 0 - 10 mT

__1.2 Durchführung:__

> - bestimme mit dem Cassy-Messgerät die natürliche magnetische Feldstärke an zwei Punkten im Physikraum und an anderen Orten im Schulhaus
>
> - notiere dir kurz Stichpunkte zu deinem Messablauf
>
> - erstelle dabei folgende Tabelle
>
> - fülle die Messwerte mit den Ergebnissen

__1.3 Ergebnisse:__

|    | Ort der Messung | magnetische Flussdichte B |
|:--:|:---------------:|:-------------------------:|
| 1  | |
| 2  | |
| 3  | |
| 4  | |

__1.4 Auswertung:__

> - ermittle den Mittelwert deiner Messungen und notiere dein Ergebnis:
>
> Das natürliche Magnetfeld der Erde hat am Gym.Klotzsche den mittleren Wert:
> $$B_{Erde} \approx ... $$
>
> Vergleiche den Wert mit dem recherchierten Ergebnis aus den Vorbetrachtungen in 1.1 in einem Satz.

### Experiment Teil 2: Bestimmung der magnetischen Feldkonstante $\mu_0$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__2.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - stelle die Formel nach $\mu_0$ um und notiere die Berechnungsvorschrift für $\mu_0$
>
> $$ \boxed{\mu_0 = ... } $$
>
> - notiere die Bedeutung der Formelzeichen
>
> Die magnetische Feldkonstante $\mu_0$ hat den theoretischen Wert
>
> $$ \boxed{\mu_0 = ... } $$
>
> - emittle mit Hilfe der Formelsammlung den Wert von $\mu_0$ und notiere ihn
>
>> Um die magnetische Feldkonstante $\mu_0$ zu bestimmen, müssen die fehlenden Werte der Formel aus 1.1 gemessen werden. Um den Einfluss von Messfehlern zu reduzieren, wird die Messung für __dreimal__ durchgeführt.

__2.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - nutze in den Einstellungen des Cassy-Messgerätes zur magnetischen Flussdichte B die Möglichekeit, dass Erdmagnetfeld zu korrigieren: Wähle dazu: __Korrektur: Offset und stelle den Wert so ein, dass das Gerät ungefähr $\pm$ 0,01 mT anzeigt. Der Offset muss mit OK bestätigt werden (kleines Häkchen).__
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BestimmungMu0](https://diversewolken.ddns.net/nextcloud/index.php/s/ndXRogTZJCCDByY/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V
>
> - bestimme für drei verschiedene Windungszahlen ($N=800,\, 1600,\, 2400$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die @color(gesamte,red) Spule aufgewickelt)
>
>     - die Stromstärke $I$ 
>
>     - die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule vorsichtig nach dem Ort mit der maximalen Flussdichte, red)
>
> - notiere alle Messwerte in einer Tabelle

__2.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| # | $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
|:--:|:--:|:--:|:--:|:--:|
| 1 | 800 | <input type="number" default="0" id="l" min="0" max="10" size="5"> | <input type="number" default="0" id="I" min="0" max="10" size="5"> | <input type="number" default="0" id="B" min="0" max="10" size="5"> |
| 2 | 1600 |  |  |
| 3 | 2400 |  |  |

{{1}}
***************
__2.4 Gemeinsame Auswertung:__

>__Lsg.:__
>
> $\hspace{0.2cm}$ $\mu_0 =$ {2}{$\frac{B \cdot ℓ}{I \cdot N}$}
{{3}}
***********
> $\hspace{0.2cm}$ __Für Messung #1:__
>
> $\hspace{0.2cm}$ $\mu_0 = $ <script input="button">
    let N = 800;
    let I = document.getElementById("I").value;
    let l = document.getElementById("l").value;
    let B = document.getElementById("B").value;
    let mu = (B*l)/(I*N) 
    if ((isNaN(mu))||(mu==0)) "..."
    else mu.toExponential(2)
 </script> $\frac{V\cdot s}{A \cdot m}$

<details style="margin-left:0.2cm">

<summary> Tabellenwert </summary>

> $\mu_0 = 1,26\cdot 10^{-6} \frac{V\cdot s}{A \cdot m}$

</details>
***********



***************

__2.4 Auswertung:__

> - ermittle aus den Messungen #1-3 und der Formel aus 2.1 jeweils die magnetische Feldkonstante $\mu_0$ und notiere deine Ergebnisse
>
> - ermittle aus den Werten für $\mu_0$ den Mittelwert, notiere dein Endergebnis und vergleiche ihn mit dem theoretischen Wert aus 2.1 (in einem Satz)

__wenn noch min. 15 min Zeit ist:__

> - schau dir Experiment Teil 3 an, du kannst direkt mit der Durchführung (unterhalb der Abnahme) beginnen und die Werte notieren

### Experiment Teil 3: Überprüfung der Proportionalität $B$ ~ $N$

@color(__ACHTUNG: Der Magnetfeld-Sensor ist sehr empfindlich und teuer. Bitte geht sorgsam damit um.__,red)

<br>

@color(_Fertige auf Basis der folgenden Arbeitsschritte ein Kurzprotokoll an._, blue)

<br>

__3.1 Vorbetrachtung:__

> Die magnetische Flussdichte im Inneren eine langen, schlanken, luftgefüllten Spule kann mit der Formel 
>
> $$ B = ... $$ 
>
> berechnet werden. 
>
> - ermittle diese Formel (siehe Hefter oder Formelsammlung)
>
> - notiere die Bedeutung der Formelzeichen
>
> - aufgrund der Formel kann man erkennen, dass die Flussdichte $B$ im Inneren der Spule proportional zur Anzahl der Windungen $N$ sein sollte
>
> - um die Proportionalität von $B$ ~ $N$ zu überprüfen, muss die magnetische Flussdichte $B$ für verschiedene Windungszahlen $N$ bestimmt werden. Dabei muss die Stromstärke $I$ konstant gehalten werden. In einem $B(N)$-Diagramm sollte sich näherungsweise eine Ursprungsgerade ergeben.

__3.2 Durchführung:__

> - erhalte von der Lehrkraft eine Spule, ein Stromversorgungsgerät und einige Experimentierkabel
>
> - schließe die Spule und das Cassy so an die Stromversorgung an, dass die Stromstärke $I$, die durch die Spule fließt, und die magnetische Flussdichte mit dem Cassy-Messgerät gemessen werden kann
>
> - nutze dafür folgenden Schaltkreis, zeichne diesen in dein Kurzprotokoll
>
> - ![Schaltkreis_BpN](https://diversewolken.ddns.net/nextcloud/index.php/s/e5eGt4GAqkdK7ws/download)
>
> - @color(__lass dir die Schaltung vor dem Einschalten abnehmen__, red)
>
> - wähle als Spannung 5 V zunächst
>
> - bestimme für drei verschiedene Windungszahlen ($N=2400,\, 1600,\, 800$):
>
>     - die Länge $ℓ$ der Spule (achte hier auf die Windungen: die Windungszahlen 800 und 1600 sind jeweils auf die halbe Spule aufgewickelt)
>
>     - bestimme die Stromstärke $I$ für die erste Messung mit $N=2400$
>
>     - bestimme die magnetische Flussdichte $B$ -> @color(suche im Inneren der Spule nach dem Ort mit der maximalen Flussdichte, red)
>
>     - verändere bei deiner zweiten Messung mit $N=1600$ die Spannung soweit, dass die Stromstärke $I$ mit der ersten Messung identisch ist
>
>     - wiederhole die Messung für $N=800$
>
> - notiere alle Messwerte in einer Tabelle

__3.3 Messwerte:__

> - erstelle eine Tabelle mit folgenden Einträgen.

| $N$ | $ℓ$ in m | $I$ in A | $B$ in T |
| :---: | :---: | :---: | :---: |
| 2400  | 0 | 0 | 0 |
| 1600  | 0 | 0 | 0 |
| 800   | 0 | 0 | 0 |

__3.4 Auswertung:__

> - erstelle aus den Messwerten ein Diagramm in dem du die Windungszahl $N$ auf der x-Achse und die magnetische Flussdichte auf der y-Achse einträgst
>
> - markiere in deinem Diagramm die drei Messpunkte #1-3, sowie den Punkt (0|0)
>
> - verbinde die Messpunkte mit einer Ausgleichsgeraden
>
> - überprüfe ob diese Ausgleichsgerade die Messergebnisse in guter Näherung darstellt, notiere einen Ergebnissatz
