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
>
> $\hspace{1cm}$ __Einheit:__ $\Big[ 1\,Wb = 1\,T\cdot m^2 = 1 V \cdot s \Big] $ (Wb _gesprochen_ Weber)
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


### 1.2 Ermittlung einer Induktionsspannung I

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



### 1.2 Ermittlung einer Induktionsspannung II


![DurchsetzteFläche](https://diversewolken.ddns.net/nextcloud/index.php/s/7gtg9MopxsGg3SN/download)

Die induzierte Spannung ist für den Generator definiert als

> $U_{ind} = -N \cdot B \cdot \dfrac{\red{\mathrm{d} A}}{\red{\mathrm{d} t}}$

Die Ableitung der durchsetzten Fläche nach der Zeit ergibt:

> $\dfrac{\red{\mathrm{d} A}}{\red{\mathrm{d} t}} = \dfrac{\red{\mathrm{d}}}{\red{\mathrm{d} t}} A_0 \cdot cos(2\pi f \cdot t) = - A_0 \cdot 2\pi f \cdot sin(2\pi f \cdot t)$

An einem Generator ergibt sich die induzierte Spannung als Sinus-Funktion:

> $U_{ind}(t) = N \cdot B \cdot A_0 \cdot 2\pi f \cdot sin(2\pi f \cdot t)$
>
> ![Uind2](https://diversewolken.ddns.net/nextcloud/index.php/s/RDY5kJNYdkmL8b2/download)
