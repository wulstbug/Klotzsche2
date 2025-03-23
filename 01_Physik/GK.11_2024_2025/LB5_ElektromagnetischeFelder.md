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

> __Induktion:__ Eine Spannung wird induziert, wenn sich der @color(magnetische Fluss $\Phi$,red) einer Leiterschleife oder Spule @color(ändert, red).

---

> __Definition:__ Der @color(magnetische Fluss $\Phi$, red) ist definiert als
>
> $$ \boxed{\red{\Phi = B \cdot A}} $$
>
> $\hspace{1cm}$ B .. magnetische Flussdichte
>
> $\hspace{1cm}$ A .. vom Magnetfeld durchsetzte Fläche

---

> __Induktionsspannung:__ Der Betrag der Induktionsspannung $U_{ind}$ ist definiert ergibt sich aus der Windungszahl der Spule $N$ multipliziert mit der @color(zeitlichen Änderung des magnetischen Flusses $\frac{\Delta\Phi}{\Delta t}$, red).
>
> $$ \boxed{U_{ind} = N \cdot \dfrac{\red{\Delta \Phi}}{\Delta t}} $$

---

__1. Schlussfolgerung:__ Je größer die Windungszahl $N$ der Spule, desto größer ist die induzierte Spannung $U_{ind}$.

---

<p class="newspaper">

> __Induktion durch Änderung der Fläche A__
>
> $$ \boxed{U_{ind} = N \cdot \red{B} \cdot \dfrac{\red{\Delta A}}{\Delta t}} $$
>
> __Beispiel:__ @color(Generator, blue)

<p class="cb">

> __Induktion durch Änderung der Flussdichte B__ 
>
> $$ \boxed{U_{ind} = N \cdot \red{A} \cdot \dfrac{\red{\Delta B}}{\Delta t}} $$
>
> __Beispiel:__ @color(Transformator, blue)

</p>

</p>

### Grundversuche Elektromagnetische Induktion

@color(Nutze die drei Simulationen um die zugehörigen Lückentexte auszufüllen., blue)

[LEIFI-Lückentexte](https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-induktion/versuche/drei-grundversuche-zur-elektromagnetischen-induktion-simulationen)

### Unterhalte dich mit der KI über die Induktion am Generator und am Transformator.

Login: phy-@color(xx,red)@gykl.ipads
Passwort: phy-@color(xx,red)

??[OpenWebUI](https://subtle-corgi-firmly.ngrok-free.app)

<p style="color:blue">
Kopiere einen Prompt in das Feld der KI. Beantworte dann die gestellte Aufgabe. Verbessere deine Antwort, bis die KI deine Antwort akzeptiert. <br> Wiederhole es mit der zweiten Aufgabe.
</p>

---
1. __Transformator:__ Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Transformators.
<div class="container" style="margin-left:10%">
    <span class="text-box" id="textToCopy1">Ich habe folgende Aufgabe bekommen: Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Transformators. Ich gebe dir meine Antwort im folgenden Prompt. Bitte bewerte meine Antwort auf seine Richtigkeit. Nutze als Formelzeichen für die Spannung U.</span>
</div>
<script input="button" style="margin-left:10%">
        const text = document.getElementById("textToCopy1").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Kopieren"
</script>

---

2. __Generator:__ Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Generators.
<div class="container" style="margin-left:10%">
    <span class="text-box" id="textToCopy2">Ich habe folgende Aufgabe bekommen: Erkäre die Anwendung des Induktionsgesetzes am Beispiel eines Generators. Ich gebe dir meine Antwort im folgenden Prompt. Bitte bewerte meine Antwort auf seine Richtigkeit. Nutze als Formelzeichen für die Spannung U.</span>
</div>
<script input="button" style="margin-left:10%">
        const text = document.getElementById("textToCopy2").innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert("Text wurde in die Zwischenablage kopiert!");
        }).catch(err => {
            console.error("Fehler beim Kopieren: ", err);
        });
        "Kopieren"
</script>

---
