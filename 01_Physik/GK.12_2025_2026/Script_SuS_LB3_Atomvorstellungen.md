<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp

@style
.lia-effect__circle {
    display: none !important;
}
.flex-container {
    display: flex;
    flex-wrap: wrap; /* Allows the items to wrap as needed */
    align-items: stretch;
    gap: 40px;
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
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
    input <= 0.03
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

@rangeQuiz20
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
    input = Math.abs(eval(input)-@1)/Math.abs(@1)
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
    input = Math.abs(eval(input)-@1)
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

# LB 8 Atomvorstellungen

![Atomvorstellungen](https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp)


## 8. 1. Die Geschichte der Atommodelle


## 8. 2. Das Bohr'sche Atommodell

![TB_1](https://diversewolken.ddns.net/nextcloud/index.php/s/apsmjmxb3B2abe7/download)

---

![TB_2](https://diversewolken.ddns.net/nextcloud/index.php/s/apsmjmxb3B2abe7/download)

### Aufgaben zu den Atmomodellen (Multiple-Choice)

❓ Frage 1: Grundannahme des bohr’schen Atommodells

Welche zentrale Annahme macht das bohr’sche Atommodell über die Elektronenbewegung?

- [[ ]] Elektronen bewegen sich frei im Atomkern
- [[X]] Elektronen bewegen sich auf festen, quantisierten Kreisbahnen
- [[ ]] Elektronen verlieren kontinuierlich Energie beim Umlauf
- [[ ]] Elektronen befinden sich in einer Elektronenwolke ohne feste Bahnen
- [[ ]] Elektronen können jede beliebige Bahnenergie annehmen

---

❓ Frage 2: Energieniveaus im bohr’schen Atommodell

Warum geben Atome nach dem bohr’schen Modell nur bestimmte Spektrallinien ab?

- [[ ]] Weil Elektronen ihre Masse verändern
- [[ ]] Weil Protonen Energie abstrahlen
- [[X]] Weil Elektronen nur zwischen diskreten Energieniveaus wechseln können
- [[ ]] Weil die Umlaufgeschwindigkeit der Elektronen konstant ist
- [[ ]] Weil der Atomkern instabil ist

---

❓ Frage 3: Gültigkeitsbereich des bohr’schen Atommodells

Für welche Atome liefert das bohr’sche Atommodell gute Ergebnisse?

- [[X]] Für wasserstoffähnliche Atome mit nur einem Elektron
- [[ ]] Für alle Atome unabhängig von ihrer Größe
- [[ ]] Nur für schwere Atome wie Uran
- [[ ]] Ausschließlich für Moleküle
- [[ ]] Für Festkörper und Metalle

❓ Frage 4: Energieabgabe im bohr’schen Atommodell

Wann wird nach dem bohr’schen Atommodell Strahlung emittiert?

- [[ ]] Wenn sich ein Elektron auf einer stabilen Bahn bewegt
- [[ ]] Wenn ein Elektron den Atomkern berührt
- [[X]] Wenn ein Elektron von einem höheren auf ein niedrigeres Energieniveau wechselt
- [[ ]] Wenn ein Elektron seine Umlaufgeschwindigkeit erhöht
- [[ ]] Wenn sich zwei Elektronen abstoßen

❓ Frage 5: Kritik am bohr’schen Atommodell

Welche der folgenden Aussagen beschreibt eine bekannte Schwäche des bohr’schen Atommodells?

- [[ ]] Es erklärt das Wasserstoffspektrum korrekt
- [[ ]] Es führt quantisierte Energieniveaus ein
- [[X]] Es kann die Spektren von Mehrelektronenatomen nicht korrekt erklären
- [[ ]] Es berücksichtigt den Atomkern
- [[ ]] Es erklärt die Stabilität von Elektronenbahnen

### Aufgaben zum Wasserstoffatom (Berechnungen)

1. Zeichnen Sie ein Energieniveau-Schema des Wasserstoffatoms mit dem Grundzustand und den ersten 5 angeregten Zuständen. Notieren Sie an jedem Niveau die Bindungsenergie. Kennzeichnen Sie den Übergang n=3 -> n=2.

---

2. Die Emissionen, die im sichtbaren Bereich liegen sind beim Wasserstoff Übergänge auf die zweite Schale. Ermitteln Sie die Energie und die Wellenlänge der Übergänge von n=3 -> n=2. Notieren Sie die Farbe des emittierten Lichts.

<p style='margin-left:10%'>

@rangeQuiz2($E_{3->2}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{3->2}$,655e-9,$\mathrm{m}$)

<!-- data-solution-button="off" -->
[[ infrarot | rot | gelb | grün | blau | violett | ultraviolett ]]

</p>

---

3. Geben Sie für ein Wasserstoffatom die Ionisierungsenergie an. <br> _Hinweis: Die Ionisierungsenergie ist die Energie, die aufgewendet werden muss, damit das Elektron des Wasserstoffs nicht mehr gebunden ist._

<p style='margin-left:10%'>

@rangeQuiz2($E_{ion}$,13.6,$\mathrm{eV}$)

</p>

