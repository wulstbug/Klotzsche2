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


## 1. Elektromagnetische Induktion

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

#### Aufbau Transformator

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

#### Demonstrationsexperiment A Freier Fall im Rohr

### 1.3. Lenz'sche Regel - Richtung der Induktionsspannung

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


#### C. Magnetisches Pendel (Induktionsbremse)

<p style="color:blue">
Aufgabe: Zeichne (Skizze), beschreibe (Beobachtung) und erkläre (Erklärung) das Experiment magnetisches Pendel in deinem Hefter. Nutze die KI um deine Beobachtungen und Erklärungen zu überprüfen.
</p>

__Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.__

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessernn.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Ich soll ein Experiment erst beschreiben und anschließend erklären. Bitte frage mich zunächst nach einer Beschreibung meiner Beobachtung. Unterstütze mich bei der Antwort, hilf mir nur, wenn ich darum bitte. Achte bei meiner Erklärung darauf, dass die Induktion einer Spannung richtig beschrieben wird und die Lenz'sche Regel korrekt erklärt wird. <br> Ein Aluminiumrad hängt frei auf einer Achse und kann sich drehen. Am unteren Ende des Aluminiumrades sind zwei Polschuhe eines Elektromagneten (Spule mit U-Kern) rechts und links des Rades angebracht. Liegt am Elektromagneten keine Spannung an und das Rad wird angestoßen, so dreht es sich weiter bis es nach einiger Zeit aufgrund der Reibung zum stehen kommt. Wird an den Elektromagneten eine Gleichspannung angelegt, so bremst das Rad ab. Je größer die Spannung, desto schneller wird das Rad gebremst. <br> Frage mich nun zunächst nach meiner Beobachtung des Experiments. Wenn ich eine zufriedenstellende Antwort gegeben haben, dann frage mich nach meiner Erklärung für das Experiment. Frage mich nach jeder meiner Antworten, ob ich meine Antwort verbessern möchte oder zur nächsten Frage bzw. zur Einschätzung kommen möchte. <br> Alle Antworten sind im Fach Physik im Niveau Grundkurs Klasse 11 zu beantworten. Schätze mir am Ende das Niveau meiner Antworten auf einer Skala von 1 bis 10 ein.</span>
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


### 1.4. Experiment: Realer Transformator

### 1.5 Ermittlung der Induktionsspannung I

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



### 1.5 Ermittlung der Induktionsspannung II

