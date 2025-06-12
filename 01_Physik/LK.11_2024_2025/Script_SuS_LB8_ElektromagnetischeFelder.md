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

.red {
    color: red;
}

.blue {
    color: blue;
}

.darkgreen {
    color: darkgreen;
}

.orange {
    color: orange;
}

.purple {
    color: purple;
}

@end

@color
<bdi style="color:@1">@0</bdi>
@end


@rangeQuiz2

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

@onload
window.LIA.settings.font_size = 2
@end

-->


# LB 8. - Elektromagnetische Felder

!?[CG-Physics-Generator](https://www.youtube.com/watch?v=34z97ULvmpM)

## Motivation - Kraftwerke zur Energieversorgung

![Waermekraftewerk](https://diversewolken.ddns.net/nextcloud/index.php/s/zq3twaoxKzLcwj7/download) ![Heizkrafttwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/8qx3ERQmPMgmeqX/download) ![Wasserkraftwerk](https://diversewolken.ddns.net/nextcloud/index.php/s/Xbf7QmBSmwzN4GK/download)

## 8.1. Elektromagnetische Induktion

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
>
> $\hspace{1cm}$ __Einheit:__ $\Big[ 1\,Wb = 1\,T\cdot m^2 = 1 V \cdot s \Big] $ (Wb _gesprochen_ Weber)
********

{{3}}
********
---

> __Induktionsspannung:__ Der Betrag der Induktionsspannung $U_{ind}$ ist definiert ergibt sich aus der Windungszahl der Spule $N$ multipliziert mit der @color(zeitlichen Änderung des magnetischen Flusses $\frac{\Delta\Phi}{\Delta t}$, red).
>
> $$ \boxed{U_{ind} = - N \cdot \dfrac{\red{\Delta \Phi}}{\Delta t}} $$
********

{{4}}
********
---

__Hinweis 1:__ Je größer die Windungszahl $N$ der Spule, desto größer ist die induzierte Spannung $U_{ind}$.

__Hinweis 2:__ Das Vorzeichen "-" gibt die _Richtung_ der induzierten Spannung an und wird durch das @color(Lenz'sche Gesetz, orange) beschrieben (_später_).

---
********

<p class="newspaper">
{{5}}
********
> __Induktion durch Änderung der Fläche A__
>
> $$ \boxed{U_{ind} = -N \cdot \red{B} \cdot \dfrac{\red{\Delta A}}{\Delta t}} $$
>
> mit $A = A_0 \cdot \cos\varphi$
>
>      $A_0$ .. Grundfläche der Spule/Leiterschleife
>
>      $\varphi$ .. Drehwinkel bzgl. der Feldlinien
>
> __Beispiel:__ @color(Generator, blue)
********

<p class="cb">
{{6}}
********

> __Induktion durch Änderung der Flussdichte B__ 
>
> $$ \boxed{U_{ind} = - N \cdot \red{A} \cdot \dfrac{\red{\Delta B}}{\Delta t}} $$
>
> __Beispiel:__ @color(Transformator, blue)
********
</p>

</p>

### 8.1.1. Das Generator-Prinzip

<p style="color:blue">

- [ ] Notiere das Tafelbild _1. Elektromagnetische Induktion_ in deinen Hefter

- [ ] Probiere die Aufgaben _Grundversuche Elektromagnetische Induktion_ und fülle die Lückentexte

- [ ] Schau dir kurz die Simulationen zum Generator an

- [ ] Übernimm den Absatz _Aufbau eines Generators_ in deinen Hefter

- [ ] Führe den Handversuch _Elektromagnetische Induktion_ durch

- [ ] Diskutiere mit der KI im Abschnitt _Elektromagnetische Induktion_

- [ ] Nutze den Bausatz Generator und baue ein Generatormodell auf, schließe ein Cassy-Spannungsmessgerät an und miss die induzierte Spannung

- [ ] Beantworte die Fragen zum Generator 2

</p>


#### Grundversuche Elektromagnetische Induktion

@color(Nutze die drei Simulationen um die zugehörigen Lückentexte auszufüllen., blue)

[LEIFI-Lückentexte](https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-induktion/versuche/drei-grundversuche-zur-elektromagnetischen-induktion-simulationen)

#### Simlationen zum Generator

>__Simulation Generator__
>
>    [FENDT-Simulation-Generator](https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-induktion/downloads/generator-simulation)


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

5. Schleifkontakte zur Spannungsabführung (Kommutator)

_Hinweis: Magnet und Spule (d.h. **Rotor** und **Stator**) können auch vertauscht sein. Dann ist Magnet beweglich und die Spule fest._

</p>

</p>

#### Handversuch - Spannung induzieren

__Materialien:__ 1m Kabel, Cassy-Messgerät, Magnet

1. Nutze ein 1m langes Kabel, wickle es zu einer einfachen Spule und schließe die Enden an das Cassy-Messgerät (Spannung messen) an.

     ![Generator_Bild1](https://diversewolken.ddns.net/nextcloud/index.php/s/bR2nasCZSpW432d/download)<!-- style="width:400px"-->

2. Wähle am Cassy-Messgerät den kleinsten (empfindlichsten) Messbereich

3. Bewege den Magneten in die Spule hinein und heraus und schau dir die induzierte Spannung an. Überprüfe auch das Vorzeichen beim Hinein-/Herausbewegen.

     ![Generator_Bild2](https://diversewolken.ddns.net/nextcloud/index.php/s/RZpQZJ5RPFTStH9/download)<!-- style="width:400px"-->

4. Lass dir von der Lehrkraft den Super-Stab-Magneten aushändigen und wiederhole den Versuch.

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
    5. Nenne und beschreibe die Kraft, die bei der Bewegung einer Leiterschleife oder Spule in einem Magnetfeld auf die Elektronen wirkt und somit die Spannung induziert.
    Alle Fragen sind im Fach Physik im Niveau Leistungskurs Klasse 11 zu beantworten. Schätze mir nach meiner 5. Antwort das Niveau meiner Antworten insgesamt ein.
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
- [[x]] $N_p=10000; N_s=200$

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

__Einstellungen:__

Nutze am Spannungsversorgungsgerät die Einstellung: __Wechselspannung, 6V__. Nutze am Cassy-Messgerät die Einstellung für die __Erfassung: Effektivwerte (AC+DC)__

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
| $\dfrac{2400}{800}=3$ | .. | .. | .. |
| $\dfrac{2400}{1600}=1,5$ | .. | .. | .. |
| $\dfrac{2400}{2400}=1$ | .. | .. | .. |
| $\dfrac{1600}{800}=2$ | .. | .. | .. |
| $\dfrac{1600}{1600}=1$ | .. | .. | .. |
| $\dfrac{1600}{2400}=0,67$ | .. | .. | .. |
| $\dfrac{800}{800}=1$ | .. | .. | .. |
| $\dfrac{800}{1600}=0,5$ | .. | .. | .. |
| $\dfrac{800}{2400}=0,33$ | .. | .. | .. |
*********


#### Begriffsklärung: Transformator

> __Idealer vs. realer Transformator__: Der ideale Transformator ist ein theoretisches Modell, bei dem einige Vereinfachungen (Idealisierungen) angenommen werden. <br> Zum Beispiel:
>
> - das magnetische Feld verläuft zu 100% im Inneren des Eisenkerns (d.h. die erzeugte magnetische Flussdichte in der Primärspule ist identisch mit der wirkenden magnetischen Flussdichte in der Sekundärspule)
>
> - der Draht der Wicklungen hat keinen elektrischen Widerstand (es entstehen keine Wärmeverluste)
>
> - innerhalb des Eisenkerns werden keine Wirbelströme induziert (keine Verluste, keine Hysterese)

> __Belasteter vs. unbelasteter Transformator__: Bei einem unbelasteten Trafo wird angenommen, dass im Sekundärstromkreis kein Verbraucher angeschlossen ist, d.h. es fließt kein Sekundärstrom. Die Gleichung 
>
> $$\dfrac{U_1}{U_2} = \dfrac{N_1}{N_2}$$
>
> gilt nur für einen __unbelasteten idealen Transformator__.


#### Demonstrationsexperiment A Freier Fall im Rohr

> Stabmagnet fällt einerseits durch ein metallisches Rohr (Aluminium) und andererseits durch ein Kunststoffrohr.

{{1}}
*********
---

@color(Zeichnen Sie eine Skizze des Versuchs. Beschreiben Sie jeweils Ihre Beobachtungen., blue)

---

__Skizze:__
*********

{{2}}
*********
---

__Beobachtung:__

<p class="newspaper">

__Metallrohr__

<p class="cb">

__Kunststoffrohr__

</p>

</p>

---
*********

{{3}}
*********
__Vorläufige Erklärung:__

> - das metallische Rohr wirkt wie eine Spule mit einer Windung
>
> - durch die Bewegung der magnetischen Kugel ändert sich _lokal_ der magnetische Fluss in der Röhre, es wird eine @color(Spannung induziert, red)
>
> - durch die induzierte Spannung @color(fließt _kreisförmig_ ein Strom und erzeugt ein Magnetfeld,red)
>
> - das @color(induzierte Magnetfeld, red) wechselwirkt mit dem Magnetfeld der Kugel und @color(bremst die Kugel, blue)
*********

### 8.1.3. Lenz'sche Regel - Richtung der Induktionsspannung

> Die induzierte Spannung ist immer @color(so gerichtet, red), dass sie ihrer Ursache @color(entgegen, red) wirkt.

> $$ \boxed{U_{ind} = \red{\textbf{-}}\, N \cdot \dfrac{\Delta\Phi}{\Delta t}} $$

__Beispiel:__ Fallende Kugel 

__Ursache für Induktion:__ Bewegung der Kugel im Rohr

__Anwendung der Lenz'schen Regel:__ Die induzierte Spanung (und daher das induzierte Magnetfeld) ist so gerichtet, dass es der Ursache (Bewegung) entgegen wirkt.

---

_Hinweise:_

- betrachten wir den @color(Betrag, red) (also den Wert) der induzierten Spannung, so genügt die Formel $N \cdot \dfrac{\Delta\Phi}{\Delta t}$

- betrachten wir die @color(Wirkung, red) der induzierten Spannung, so müssen wir die _Lenz'sche Regel_ beachten

#### Weitere Beispiele

@color(Beschreibe und erkläre die beiden Experimente in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen., blue)

#### B. Thomson'scher Ringversuch 

<p style="color:blue">
Aufgabe: Zeichne (Skizze), beschreibe (Beobachtung) und erkläre (Erklärung) das Experiment _Thomson'scher Ringversuch_ in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen.
</p>


__Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.__

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessernn.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Ich soll ein Experiment erst beschreiben und anschließend erklären. Bitte frage mich zunächst nach einer Beschreibung meiner Beobachtung. Unterstütze mich bei der Antwort, hilf mir nur, wenn ich darum bitte. Achte bei meiner Erklärung darauf, dass die Induktion einer Spannung richtig beschrieben wird und die Lenz'sche Regel korrekt erklärt wird. <br> Das Experiment ist der Thomson'sche Ringversuch. Man benutzt zwei Aluminiumringe: Der erste Ring ist vollständig, der zweite Ring hat einen Schlitz, sodass keine Ringströme fließen könnnen. Beide Ringe werden auf einen U-Kern mit Eisenjoch und einer Spule auf dem U-Kern gesteckt. An die Spule wird eine starke Wechselspannung angelegt. <br> Frage mich nun zunächst nach meiner Beobachtung des Experiments. Wenn ich eine zufriedenstellende Antwort gegeben haben, dann frage mich nach meiner Erklärung für das Experiment. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte oder zur nächsten Frage bzw. zur Einschätzung kommen möchte. <br> Alle Antworten sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir am Ende das Niveau meiner Antworten auf einer Skala von 1 bis 10 ein.</span>
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

### 8.1.4 Selbstinduktion an Spulen

> __Ändert__ sich das @color(__von einer Spule__, red) erzeugte Magnetfeld (__z.B. durch Ein- oder Ausschalten__), so wird in der Spule eine Spannung induziert. Man nennt diesen Effekt @color(__Selbstinduktion__, red). 

> __Schlussfolgerung:__ Beim Ein- bzw. Ausschalten wirkt die @color(__Selbstinduktion__,red) nach der __Lenz'schen Regel__ so, dass der Auf- bzw. Abbau des magnetischen Feldes __behindert__ wird.


#### Experiment zur Selbstinduktion

![Schaltkreis](https://diversewolken.ddns.net/nextcloud/index.php/s/Gn4s3bXyXQJNRq3/download)

<p style="color:blue">

__Aufgaben:__ 

1. Bauen Sie den Schaltkreis auf

2. Lassen Sie sich die Schaltung abnehmen

3. Überprüfen Sie das Aufleuchten der beiden Lampen, wenn der Schalter geschlossen wird

4. Beschreiben und erklären Sie ihre Beobachtung

5. Erklären Sie das Entstehen eines (Selbst-)Induktionsstroms

</p>

### 8.1.5 Induktivität einer Spule

![Herleitung1](https://diversewolken.ddns.net/nextcloud/index.php/s/fMG33JSBPQHNLTB/download)

![Herleitung2](https://diversewolken.ddns.net/nextcloud/index.php/s/4WBaq5AJgentTrc/download)

### 8.1.6 Energie im Magnetfeld einer Spule

Die im magnetischen Feld einer Spule gespeicherte Energie kann mit der Formel 

$$ \boxed{E_{mag} = \frac{1}{2} \cdot L \cdot I^2} $$

ermittelt werden.

#### Aufgabe 1

![Duden S. 376 / 41.](https://diversewolken.ddns.net/nextcloud/index.php/s/ZrJ9SJzw27kyGKQ/download)

<p style="margin-left:10%">

@rangeQuiz2($L$, 3.33e-3 ,H)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Ermitteln Sie zunächst die Induktivität der Spule.

Ermitteln Sie für die 5 Zeitabschnitte jeweils die Änderung der Stromstärke $\Delta I$ mit der Zeit $\Delta t$. Nutzen Sie das Gesetz zur Selbstinduktion, um die jeweilige Spannung zu ermitteln. Achten Sie auf das richtige Vorzeichen der Spannung.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

![Lsg_Duden_376_41](https://diversewolken.ddns.net/nextcloud/index.php/s/q47wj7KjJaNNf32/download)

<!--
     data-show
     data-title=""
     data-type="line"
     data-fontSize="16pt"
     data-xlabel="t in s"
     data-ylabel="U in mV"
-->
| t in s | U in mV | 
| :---: | :---: |
| 0 | 0 |
| 10 | 0 |
| 10 | 82.5 |
| 20 | 82.5 |
| 20 | 0 |
| 30 | 0 |
| 30 | -132 |
| 35 | -132 |
| 35 | 0 |
| 45 | 0 |

</details>

#### Aufgabe 2

2. An die Experimentierspule der Schule wird bei maximaler Windungszahl eine Spannung von 6V angelegt. Ermitteln Sie die im magnetischen Feld gespeicherte Energie.


<p style="margin-left:10%">

@rangeQuiz2($I$, 0.0896 , A)

@rangeQuiz2($E_{mag}$, 3.81e-4 , J)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Nutzen Sie für die Induktivität den aufgedruckten Wert. Nutzen Sie zur Ermittlung der Stromstärke den angegebenen Wert für den Ohmschen Widerstand der Spule.

</details>

<details style="margin-left:10%">

<summary> __Lösung__ </summary>

$L = 68 mH$

$R = 67 \Omega$

=> $I = \frac{U}{R} = 0,0896 A$

=> $E = \frac{1}{2} \cdot L \cdot I^2 = 0,381 mJ$

</details>

#### Aufgabe 3

![Metzler S. 261/3](https://diversewolken.ddns.net/nextcloud/index.php/s/KH9BGLMF8sk4Ts3/download)

<p style="margin-left:10%">

__Überprüfung a):__

@rangeQuiz2($\mu_r$, 884.6 , .)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Nutzen Sie die Formel für die Induktivität um mit den gegebenen Werten die magnetische Permeabilität zu ermitteln.

</details>

<details style="margin-left:10%">

<summary> __Lösung a__ </summary>

geg.: 

- $A = 20 cm^2 = 20 \cdot 10^{-4} m^2$

- $n = 600$

- $l = 0,4 m$

- $I = 6 A$

- $L = 2 H$

ges.:

- $\mu_r$

Lsg.:

Die Induktivität ergibt sich mit der Formel

$$ L = \mu_0 \mu_r \frac{N^2 \cdot A}{l}$$

und damit ergibt sich für $mu_r$

$$ \mu_r = 884,6 $$

</details>

#### Aufgabe 4

![Metzler S. 257 / 1a](https://diversewolken.ddns.net/nextcloud/index.php/s/AKTszCMAoy4mTMi/download)

<p style="margin-left:10%">

__Überprüfung a):__

@rangeQuiz2($\Delta B$, 0.003925 , T)

@rangeQuiz2($U_{ind}$, -23.55 , V)

</p>

<details style="margin-left:10%">

<summary> __Lösungshinweis__ </summary>

Ermitteln Sie zunächst die von der Feldspule erzeugte magnetische Flussdichte und ermitteln Sie aus der Änderung der Stromstärke, die Änderung $\Delta B$.

Nutzen Sie anschließend die Änderung $\Delta B$ im Zeitintervall $\Delta t$ um mit dem Induktionsgesetz die in der Induktionsspule induzierte Spannung zu ermitteln.

</details>

<details style="margin-left:10%">

<summary> __Lösung a__ </summary>

geg.: 

- $\Delta I = 0,25 A$

- $\Delta t = 7,5 \cdot 10^{-3} s$

- $N_F = 7500$

- $l_F = 0,6 m$

- $N_{ind} = 1500$

- $r_{ind} = 0,03 m$

ges.:

- $U_{ind}$

Lsg.:

Die Induktion wird hier von der Änderung des Magnetfeldes 
$\Delta B$ erzeugt.

$$ \Delta B = \mu_0 \cdot \frac{N_F \cdot \Delta I}{l_F} = 3,925 mT$$

Diese Änderung des Magnetfeldes wirkt in der Induktionsspule im Zeitintervall $\Delta t$. Nach dem Induktionsgesetz ergibt sich


$$ U_{ind} = - N_{ind} \cdot \frac{\Delta B}{\Delta t} = -23,55 V $$

</details>

#### Experimentelle Übungen

![Transformatoren](https://diversewolken.ddns.net/nextcloud/index.php/s/Bf5P3Abk5WQanWH/download)

{{1}}
********
1. Folgende Kombinationen funktionieren als Transformator

     [[x]] 1
     [[x]] 2
     [[x]] 3
     [[x]] 4
     [[x]] 5

********

{{2}}
********
2. Ermitteln Sie mit Hilfe einer Spannungsversorgung (6V~) und digitalen Messgeräten für jede der Kombinationen den Übertragungsfaktor n/n'. Notieren Sie Ihre Ergebnisse in einer Tabelle.

$$ \frac{n}{n'} = \dfrac{\frac{N_1}{N_2}}{\frac{U_1}{U_2}} $$
********


### 8.1.7 Ermittlung einer Induktionsspannung I

> Ist der zeitliche Verlauf $\Phi(t)$ gegeben, so lässt sich die Induktionsspannung daraus ermitteln.

__Beispiel 1: mit N=1__


<!--
     data-show
     data-title=""
     data-type="line"
     data-fontSize="16pt"
     data-xlabel="t in s"
     data-ylabel="Φ in Wb"
-->
| t in s | Φ in Wb | 
| :---: | :---: |
| 0 | 10 |
| 10 | 10 |
| 20 | 40 |
| 30 | 40 |
| 50 | 0 |
| 60 | 0 |
| 70 | 10 |

{{1}}
**************

<p class="newspaper3">

<p style="margin-left:5%">

__Abschnitt: 0-10 s__

{{2}}
**************
     $\Delta t = 10 s$ 

     $\Delta \Phi = 0 Wb$

     $U_{ind} = - \frac{\Delta \Phi}{\Delta t}$

     $U_{ind} = 0 V$
**************

</p>

<p class="cb">

<p style="margin-left:5%">

__Abschnitt: 10-20 s__

{{3}}
**************
     $\Delta t = 10 s$ 

     $\Delta \Phi = 30 Wb$

     $U_{ind} = - \frac{\Delta \Phi}{\Delta t}$

     $U_{ind} = -3 V$
**************

</p>

<p class="cb">

<p style="margin-left:5%">

__Abschnitt: 30-50 s__

{{4}}
**************
     $\Delta t = 20 s$ 

     $\Delta \Phi = -40 Wb$

     $U_{ind} = - \frac{\Delta \Phi}{\Delta t}$

     $U_{ind} = ..$
**************

</p>

</p>

</p>

</p>

{{5}}
**************
__Zeichne ein $U_{ind}(t)$-Diagramm für den dargestellten Zeitabschnitt.__

<details style="margin-left:5%">

<summary> Lösung </summary>

<!--
     data-show
     data-title=""
     data-type="line"
     data-fontSize="16pt"
     data-xlabel="t in s"
     data-ylabel="U in V"
-->
| t in s | U in V | 
| :---: | :---: |
| 0 | 0 |
| 10 | 0 |
| 10 | -3 |
| 20 | -3 |
| 20 | 0 |
| 30 | 0 |
| 30 | 2 |
| 50 | 2 |
| 50 | 0 |
| 60 | 0 |
| 60 | -1 |
| 70 | -1 |

</details>

**************

**************



### 8.1.7 Ermittlung einer Induktionsspannung II


![DurchsetzteFläche](https://diversewolken.ddns.net/nextcloud/index.php/s/7gtg9MopxsGg3SN/download)

Die induzierte Spannung ist für den Generator definiert als

> $U_{ind} = -N \cdot B \cdot \dfrac{\red{\mathrm{d} A}}{\red{\mathrm{d} t}}$

Die Ableitung der durchsetzten Fläche nach der Zeit ergibt:

> $\dfrac{\red{\mathrm{d} A}}{\red{\mathrm{d} t}} = \dfrac{\red{\mathrm{d}}}{\red{\mathrm{d} t}} A_0 \cdot cos(2\pi f \cdot t) = - A_0 \cdot 2\pi f \cdot sin(2\pi f \cdot t)$

An einem Generator ergibt sich die induzierte Spannung als Sinus-Funktion:

> $U_{ind}(t) = N \cdot B \cdot A_0 \cdot 2\pi f \cdot sin(2\pi f \cdot t)$
>
> ![Uind2](https://diversewolken.ddns.net/nextcloud/index.php/s/RDY5kJNYdkmL8b2/download)


## 8.2 Der Hall-Effekt


![Hall-Tafelbild](https://diversewolken.ddns.net/nextcloud/index.php/s/TxRstgAdGsEEgs9/download)

>In einer stromdurchflossenen Leiterplatte wird eine Hall-Spannung $U_H$ induziert, wenn ein Magnetfeld senkrecht zur Stromrichtung wirkt.
>
> $$ \boxed{U_H = R_H \dfrac{I}{d} B} $$
>
> mit
> 
> - $B$ .. magnetische Flussdichte
>
> - $R_H$ .. Hall-Konstante des Materials | Einheit: $\Big[ \dfrac{m^3}{C} \Big]$
>
> - $d$ .. Dicke der Leiterplatte
>
> - $I$ .. fließende Stromstärke

__Herleitung der Hall-Spannung__

<p style="margin-left:5%">

Wenn ein Strom $I$ durch einen Leiter fließt und dieser senkrecht zu einem Magnetfeld $B$ steht, wirken Lorentzkräfte $F_L$auf die bewegten Ladungsträger.

- Elektronen bewegen sich mit der Driftgeschwindigkeit $ v_d $
- Magnetfeld $ B $ steht senkrecht zur Bewegungsrichtung
- Lorentzkraft: $ F_L = q \cdot v_d \cdot B $

Diese Kraft führt zu einer Ladungstrennung im Leiter, was wiederum ein elektrisches Feld $ \vec{E}_H $ erzeugt.

**Im Gleichgewicht gilt:**

$ F_L = F_{el} $

$ \Rightarrow q \cdot v_d \cdot B = q \cdot E_H$

$ \Rightarrow E_H = v_d \cdot B$


Die Hall-Spannung $ U_H $ ergibt sich aus:

$ U_H = E_H \cdot d = v_d \cdot B \cdot d $

Die Driftgeschwindigkeit ergibt sich als $ v_d = \frac{ℓ}{t} $,wobei die Driftzeit $t$ mit der Stromstärke $I$ zu $t=\frac{Q}{I}$ und die fließende Ladung $Q$ mit $Q=N \cdot q$ ($N$..Anzahl der Ladungsträger) und $N=n \cdot V$ gilt ($n$..Dichte der Ladungsträger). Das Volumen $V$ der Leiterplatte ist $V = ℓ \cdot b \cdot h$. Sämtliche Formeln ineinander eingesetzt ergibt sich:

$ U_H = \dfrac{1}{n\cdot q} \dfrac{I}{d} B $

</p>


#### Multiple-Choice-Fragen

__Frage 1__
Welche Kraft bewirkt die Ladungstrennung im Hall-Effekt?

- [[ ]] Gravitationskraft
- [[x]] Lorentzkraft
- [[ ]] Reibungskraft
- [[ ]] Kernkraft

---

__Frage 2__
Was beschreibt die Hall-Spannung?

- [[ ]] Die Spannung, die durch Temperaturunterschiede entsteht
- [[x]] Die Spannung, die durch die Ablenkung von Ladungsträgern im Magnetfeld entsteht
- [[ ]] Die Spannung entlang der Stromrichtung
- [[ ]] Die Differenz zwischen magnetischer und elektrischer Energie

---

__Frage 3__
Welche Größen beeinflussen die Hall-Spannung direkt?

- [[x]] Stromstärke
- [[x]] Magnetfeldstärke
- [[ ]] Temperatur
- [[x]] Breite des Leiters

---

__Frage 4__
Was passiert mit der Hall-Spannung, wenn das Magnetfeld verdoppelt wird?

- [[x]] Sie verdoppelt sich
- [[ ]] Sie bleibt gleich
- [[ ]] Sie halbiert sich
- [[ ]] Sie wird null

---



__Frage 5__
Folgendes Material hat betragsmäßig die größte Hall-Konstante..

- [[ ]] Bismut
- [[x]] Germanium
- [[ ]] Gold
- [[ ]] Silber
- [[ ]] Zink

---


#### Aufgabe 1: Einfache Berechnung

Ein Silber-Leiter mit einer Breite von 2 cm, durch den ein Strom von 3 A fließt, befindet sich in einem Magnetfeld von 0,5 T.

Berechnen Sie den Betrag der Hall-Spannung.

@rangeQuiz2($U_H$, 6.675e-9 , V)


#### Aufgabe 2: Umformung und Analyse

Überprüfen Sie, auf welchen Wert die Hall-Spannung maximal steigen könnte, wenn man das Material Silber gegen ein anderes tauschen würde.

a) Tauschen mit

[[ Germanium ]]

b) Hall-Spannung steigt in diesem Fall auf

@rangeQuiz2($U_H$, 0.495 , V)


#### Aufgabe 3: Komplex – Materialvergleich

Zwei verschiedene Materialien A und B werden unter denselben Bedingungen (gleicher Strom, gleiches Magnetfeld, gleiche Geometrie) getestet. Die gemessene Hall-Spannung bei A beträgt $ U_H^A = 3 \cdot 10^{-6} \, \text{V} $, bei B $ U_H^B = 6 \cdot 10^{-6} \, \text{V} $. 

Wie verhalten sich die Ladungsträgerdichten $ n_A $ und $ n_B $ zueinander?

@rangeQuiz2($\dfrac{n_A}{n_B}$, 2 , . )

<details style="margin-left:5%">

<summary> Lösung </summary>

Die Hall-Spannung von A und B ergeben sich zu:

$U^A_H = \dfrac{1}{n_A\cdot q} \dfrac{I}{d} B$

$U^B_H = \dfrac{1}{n_B\cdot q} \dfrac{I}{d} B$

Das Verhältnis $\dfrac{n_A}{n_B}$ ist demnach

$\dfrac{n_A}{n_B} = \dfrac{U^B_H}{U^A_H} = \frac{2}{1}$

Material A hat also doppelt so viele Ladungsträger pro Volumen wie Material B.

</details>

#### Aufgabe 4: Abituraufgabe zum Hall-Effekt

Die Hall-Sonde ist ein wichtiger Sensor zum Ausmessen von Magnetfeldern.

a) Erklären Sie kurz, warum in einem quaderförmigen Silberplättchen zwischen den Anschlüssen 1 und 2 eine Hall-Spannung auftritt. ![Abi97_Bilda](https://diversewolken.ddns.net/nextcloud/index.php/s/eG2X7c9LnB3dJeg/download) 


<details style="margin-left:5%">

<summary> Antwort an KI </summary>

<span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: An einem quaderförmiges Silberplättchen fließt zwischen den Stirnflächen ein elektrischer Strom. Senkrecht zur Frontseite des Silberplättchens wirkt ein homogenes Magnetfeld. Erkläre das Auftreten der Hall-Spannung zwischen der oberen und der unteren Seite der Platte. <br> Bitte stelle mir diese Frage. Bitte warte auf meine Antwort und bewerte diese. Gib mir die Möglichkeit meine Antwort zu verbessern. Gib mir nicht die Lösung, sondern warte auf meine Aussagen. Mein Niveau ist Leistungs Physik Klasse 11. Bewerte meine Antwort jeweils auf einer Skala von 0 bis 10, wobei 10 das beste ist.</span>
    
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


</details>

---

b) Bei einer Hall-Sonde wird ein Silberplättchen der Dicke $d=12\,µm$ verwendet. Die Hall-Konstante von Silber beträgt bei Zimmertemperatur $R_H = 0,9\cdot10^{-10}\frac{m^3}{C}$. In einem Magnetfeld ergibt sich bei einem Sondenstrom von 10 A eine Hall-Spannung von $1,7\cdot10^{-5} V$. Berechnen Sie die Flussdichte B.

@rangeQuiz2($B$, 0.23 , T)

---

c) Berechnen Sie, wie viele Elektronen pro Silberatom im Mittel dem „freien Elektronengas“ zugeordnet werden können. Ein Silberatom hat eine Masse von 107,9 u und Silber hat eine Dichte von $10,5 \frac{t}{m^3}$.

@rangeQuiz2($N$, 1.2 , Elektronen pro Atom)

---

d)  Für eine Hall-Sonde aus dem Halbleiter Germanium mit der Dicke 1,0 mm wurden folgende Messreihen aufgenommen:

__für B = 10 mT__

| | | | | |
| I in mA	| 10	| 15	| 20	|25     |
| UH in mV	| 1,4	| 2,1	| 2,9	|3,7    |

__für B = 20 mT__

| | | | | |
|I in mA	|10	    |15	    |20	    |25     |
|UH in mV	|2,8	|4,3	|5,7	|7,3    |

__für B = 30 mT__

| | | | | |
|I in mA	|10	    |20	    |30	    |40     |
|UH in mV	|4,4	|8,8	|13,1	|17,5   |

Berechnen Sie für eine Messung die Hall-Konstante für Germanium.

@rangeQuiz2($R_H$, 0.015 , $\frac{m^3}{C}$)

<details style="margin-left:5%">

<summary> Lösung </summary>

![Lsg_Abi97_d.png](https://diversewolken.ddns.net/nextcloud/index.php/s/znQ6KkycyHSXqQe/download)

</details>

---

e) Berechnen Sie unter Verwendungen der Angaben und Ergebnisse aus den Aufgaben b) und d) das Verhältnis der Ladungsträgerdichten von Silber und Germanium $\frac{n_{Si}}{n_{Ge}}$. Schließen Sie daraus, welcher Stoff den elektrischen Strom besser leitet.

@rangeQuiz2($\dfrac{n_{Si}}{n_{Ge}}$, 1.7e8 , $.$)

<details style="margin-left:5%">

<summary> Lösung </summary>

![Lsg_Abi97_e.png](https://diversewolken.ddns.net/nextcloud/index.php/s/oj5FbWXJ6xL6LaL/download)

In Silber ist die Konzentration an freien Ladungsträgern um ein Vielfaches höher als in Germanium. Bei Zimmertemperatur leitet Silber wesentlich besser den elektrischen Strom als Germanium.

</details>

---

f) Überprüfen Sie anhand der Messdaten aus Aufgabe b, ob ein mathematischer Zusammenhang zwischen der Hall-Spannung und der Flussdichte nachgewiesen werden kann.

<details style="margin-left:5%">

<summary> Lösung </summary>

Für den Zusammenhang zwischen Hall-Spannung und Flussdichte müssen Werte gesucht werden, bei denen der Strom durch die Sonde gleich ist. Man kann also z.B. die Untersuchung für einen Strom von 10 mA oder für 20 mA vornehmen.

__für 10mA__

| | | | |
|$B$ in mT	    | 10	|20	 |   30  |
|$U_H$ in mV	| 1,4	|2,8 |   4,4 |
|$B/U_H$	    | 7,1	|7,1 |   6,8 |

__für 20 mA__

| | | | |
|$B$ in mT	    |10	    |20	    |30     |
|$U_H$ in mV	|2,9	|5,7	|8,8    |
|$B/U_H$	    |3,4	|3,5	|3,4    |

Für jede Stromstärke ergibt sich ein nachezu konstanter Wert $B/U_H$. Für eine konstante Stromstärke durch die Hallsonde ist die Hall-Spannung proportional zur Flussdichte.

</details>
