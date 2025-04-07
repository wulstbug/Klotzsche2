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


# LB V - Elektromagnetische Felder

!?[CG-Physics-Generator](https://www.youtube.com/watch?v=34z97ULvmpM)

## Motivation - Kraftwerke zur Energieversorgung

![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/Xbf7QmBSmwzN4GK/download)

## 1. Elektromagnetische Induktion

{{1}}
********
> __Induktion:__ Eine Spannung wird induziert, wenn sich der @color(magnetische Fluss $\Phi$,red) einer Leiterschleife oder Spule @color(ändert, red).
********

{{2}}
********
---

> __Definition:__ Der @color(magnetische Fluss $\Phi$, red) ist definiert als
>
> $$ \boxed{\red{\Phi = B \cdot A}} $$
>
> $\hspace{1cm}$ B .. magnetische Flussdichte
>
> $\hspace{1cm}$ A .. vom Magnetfeld durchsetzte Fläche
********

{{3}}
********
---

> __Induktionsspannung:__ Der Betrag der Induktionsspannung $U_{ind}$ ist definiert ergibt sich aus der Windungszahl der Spule $N$ multipliziert mit der @color(zeitlichen Änderung des magnetischen Flusses $\frac{\Delta\Phi}{\Delta t}$, red).
>
> $$ \boxed{U_{ind} = N \cdot \dfrac{\red{\Delta \Phi}}{\Delta t}} $$
********

{{4}}
********
---

__1. Schlussfolgerung:__ Je größer die Windungszahl $N$ der Spule, desto größer ist die induzierte Spannung $U_{ind}$.

---
********

<p class="newspaper">
{{5}}
********
> __Induktion durch Änderung der Fläche A__
>
> $$ \boxed{U_{ind} = N \cdot \red{B} \cdot \dfrac{\red{\Delta A}}{\Delta t}} $$
>
> __Beispiel:__ @color(Generator, blue)
********

<p class="cb">
{{6}}
********

> __Induktion durch Änderung der Flussdichte B__ 
>
> $$ \boxed{U_{ind} = N \cdot \red{A} \cdot \dfrac{\red{\Delta B}}{\Delta t}} $$
>
> __Beispiel:__ @color(Transformator, blue)
********
</p>

</p>

### 1.1. Aufgaben zum Generator


<p style="color:blue">

- [ ] Notiere das Tafelbild _1. Elektromagnetische Induktion_ in deinen Hefter

- [ ] Probiere die Aufgaben _Grundversuche Elektromagnetische Induktion_ und Fülle die Lückentexte

- [ ] Übernimm den Absatz _Aufbau eines Generators_ in deinen Hefter

- [ ] Diskutiere mit der KI im Abschnitt _Elektromagnetische Induktion_

- [ ] Nutze den Bausatz Generator und baue ein Generatormodell auf, schließe ein Cassy-Spannungsmessgerät an und miss die induzierte Spannung

- [ ] Beantworte die Fragen zum Generator 2

</p>


#### Grundversuche Elektromagnetische Induktion

@color(Nutze die drei Simulationen um die zugehörigen Lückentexte auszufüllen., blue)

[LEIFI-Lückentexte](https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-induktion/versuche/drei-grundversuche-zur-elektromagnetischen-induktion-simulationen)

#### Aufbau eines Generators

Ein einfacher __Generator__ besteht typischer Weise aus einem @color(Magneten, orange) und einer @color(Spule,orange), welche sich im Magnetfeld drehen kann.

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


#### KI: Elektromagnetische Induktion am Generator

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---

__Aufgabe Induktion:__

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2">Ich werde dir jetzt 4 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10. Frage mich nach jeder Einschätzung von dir, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln.
    1. Definiere den Begriff magnetischer Fluss.
    2. Notiere, welche physikalischen Größen sich bezüglich des magnetischen Flusses ändern können, damit einer Induktionsspannung erzeugt wird.
    3. Nenne eine technische Anwendung, bei dem eine Änderung der durchsetzten Fläche eine Spule in einem Magnetfeld zu einer Induktionsspannung führt.
    4. Notiere Einflussfaktoren auf die Induktionsspannung in einem Generator.
    Alle Fragen sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.
</span>
</div>
<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)


#### Generator selber bauen

__Aufgabenstellung:__ Nutze in einer Gruppe von zwei Leuten den Bausatz und baue den Generator auf. Am Lehrertisch gibt es ein Demogerät. Experimentiere mit dem Generator anhand folgender Aufgaben

{{1}}
*******
__Der Generator:__

1. Schließe an den Generator das Cassy-Messgerät zur Spannungsmessung an. (nur @color(roten,red) und @color(schwarzen, black) Pol verwenden.)

2. Stelle das Cassy-Messgerät bei der Spannungseinstellung (__Messbereich__) auf -0,3 bis 0,3 V.

3. Drehe an der Welle und überprüfe die angezeigte Spannung. <br> {2}{@color(-> Das Voltmeter sollte ausschlagen.,orange)}

4. Überprüfe, ob du die maximale Spannung beeinflussen kannst.

5. Wähle das Diagramm (oben rechts) und dann die Stoppuhr (oben links) und lass dir den zeitlichen Spannungsverlauf anzeigen.

*******


#### Fragen zum Generator 2

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

### 1.2. Arbeitsaufträge zum Transformator

<p style="color:blue">

- [ ] Zeichne das Schema eines Transformators in deinen Hefter. Übernimm das Tafelbild komlett

- [ ] Bearbeite die Übungen zum Trafo

- [ ] Bearbeite die KI-Aufgaben zur Induktion


</p>

#### Aufbau Transformator

<p class="newspaper">

![TB-Transformator](https://diversewolken.ddns.net/nextcloud/index.php/s/mGSfKNSR8C9s8XM/download)

<p>

__Formelzeichen:__

<p style="margin-left:10%">

$U_1$ oder $U_p$ .. Primärspannung

$U_2$ oder $U_s$ .. Sekundärspannung

$N_1$ oder $N_p$ .. Windungszahl auf Primärseite

$N_2$ oder $N_s$ .. Windungszahl auf Sekundärseite

</p>

__Funktionsprinzip:__

<p style="margin-left:10%">

Auf der Primärseite wird eine @color(__Wechselspannung__, darkblue) angelegt. Diese Wechselspannung erzeugt ein @color(__zeitlich veränderliches Magnetfeld__, orange), welches im wesentlichen im @color(__Eisenkern__, darkgray) verläuft. <br> Die @color(Sekundärspule,crimson) wird von dem Magnetfeld durchsetzt. In dieser Spule ändert sich der Magnetische Fluss $\Phi$ und somit wird eine Spannung induziert.

</p>

</p>

</p>

> Bei einem unbelasteten Transformator gilt:
>
> $$ \boxed{\dfrac{U_1}{U_2} = \dfrac{N_1}{N_2}} $$

#### Übung Funktionsweise Trafo

@color(_Bringe die Sätze von links nach rechts in die richtige Reihenfolge., blue)

<iframe src="https://learningapps.org/watch?v=pyuu71zx524" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

#### Einfache Rechnungen - Transformator

1. Betrachte folgende Transformator-Daten. Entscheide, ob der Transformator zum Hoch- und Heruntertransformieren verwendet wir. <br> _Für das Übersetzungsverhältnis $n$ gilt: $n = \frac{U_p}{U_s} = \frac{N_p}{N_s}$_.

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
- [[ ]] Hochtransformieren
- [[x]] Heruntertransformieren
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

2. ![TrafoHaus](https://upload.wikimedia.org/wikipedia/commons/1/19/Elfmorgenbruch_220kV-Transformator.jpg) In Transformatorstationen wird die Elektrizität des regionalen Verteilnetzes mit der Mittelspannung ca. 20 kV zur Versorgung der Niederspannungsendkunden auf die im Ortsnetz verwendeten 400-V-Leiter-Leiter-Spannung transformiert. Wähle die Transformator-Einstellungen aus, die hier verwendet werden können. <br> _Hinweise: 1kV = 1000 V_

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

</p>


#### KI-Aufgaben zur Induktion

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.
</p>

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessern, oder zur nächsten Frage springen.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2">Ich werde dir jetzt 5 Aufgaben nennen. Bitte stelle mir diese Fragen in der Reihenfolge und warte nach jeder Frage auf meine Antwort. Bewerte mir jede meiner Antworten auf einer Skala von 0 bis 10. Frage mich nach jeder Einschätzung von dir, ob ich meine Antwort verbessern möchte, oder zur nächsten Frage wechseln.
    1. Definiere den Begriff magnetischer Fluss.
    2. Notiere, welche physikalischen Größen sich bezüglich des magnetischen Flusses ändern können, damit einer Induktionsspannung erzeugt wird.
    3. Nenne eine technische Anwendung, bei dem eine Änderung der durchsetzten Fläche eine Spule in einem Magnetfeld zu einer Induktionsspannung führt.
    4. Nenne eine technische Anwendung, bei dem die Änderung der magnetischen Flussdichte eine Spannung hervorruft.
    5. Erkläre, wie bei einem Transformator die Induktion Anwendung findet.
    Alle Fragen sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.</span>
</div>

<script input="submit" style="margin-left:10%" default="Prompt Kopieren">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Prompt Kopieren"
</script>

---

Login: phy-@color(xx,red)@gykl.ipads

Passwort: phy-@color(xx,red)

[KI-OpenWebUI](http://10.102.1.3:3001)

alternativer Link für eigene Geräte

[KI-OpenWebUI-BYOD](https://subtle-corgi-firmly.ngrok-free.app)



#### Experiment: Realer Transformator

<p class="newspaper">

__Aufgabe:__ 

Baue einen Transformator nach folgendem Vorbild auf. Nutze die Cassy-Messgeräte um Primär- und Sekundärspannung für verschiedene Kominationen aus Primär- und Sekundärwindungszahl zu untersuchen.

__Analyse:__ 

Zeichne einen Graphen mit $n=\dfrac{N_1}{N_2}$ auf der x-Achse und $n'= \dfrac{U_1}{U_2}$ auf der y-Achse.

<p class="cb">

![Aufbau_Transformator](https://diversewolken.ddns.net/nextcloud/index.php/s/pmQD7JM7pBTG45k/download)

</p>

</p>

{{0-2}}
*********
<!--
     data-schow="false"
     data-title=""
     data-type="line"
     data-xlabel="N1/N2"
     data-ylabel="U1/U2"
-->
| $n=\dfrac{N_1}{N_2} $ | $U_1$ in V | $U_2$ in V | $n' = \dfrac{U_1}{U_2}$ |
| ---- | ---- | ---- | ---- |
| $\dfrac{2400}{800}=3$ | 5 | .. | .. |
| $\dfrac{2400}{1600}=2$ | 5 | .. | .. |
| $\dfrac{2400}{2400}=1$ | 5 | .. | .. |
| $\dfrac{1600}{800}=2$ | 5 | .. | .. |
| $\dfrac{1600}{1600}=1$ | 5 | .. | .. |
| $\dfrac{1600}{2400}=0,67$ | 5 | .. | .. |
| $\dfrac{800}{800}=1$ | 5 | .. | .. |
| $\dfrac{800}{1600}=0,5$ | 5 | .. | .. |
| $\dfrac{800}{2400}=0,33$ | 5 | .. | .. |
*********
