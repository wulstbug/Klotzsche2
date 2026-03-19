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

# LB VIII Atomvorstellungen

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

## 8. 3. Das Wasserstoffatom

![TB_1](https://diversewolken.ddns.net/nextcloud/index.php/s/7DwNPsGoEy62fNL/download)


{{1}}
************
__Zusammenfassung bis hierher:__
************

{{2}}
************
> - an einen Atomkern gebundene Elektronen können nur bestimmte (d.h. diskrete) Energieniveaus besetzen -> @color(Orbitale im quantenmechanischen Atommodell, red)
************

{{3}}
************
> - wechselt ein Elektron ein Energiniveau, so ist das mit einem __quantenhaften__ Energieaustausch mit der Umgebung verbunden -> @color(Emission und Absorption von Photonen, red)
************

## 8. 4. Orbitale des quantenmechanischen Atommodells

{{1}}
**********
__Aufenthaltswahrscheinlichkeit statt feste Kreisbahn:__

> Das quantenmechanische Atommodell beschreibt den Aufenthaltsort der Elektronen nicht als Kreisbahn (wie im bohrschen Atommodell), sondern als eine @color(Wahrscheinlichkeitsverteilung, red) im Raum um den Atomkern. -> [Video 1](https://youtu.be/behQ3O97DXw?t=446)
**********

{{2}}
**********
__Bemerkungen:__

- bei einer Messung ist der Ort des Elektrons __nicht vorhersagbar (nicht determiniert)__

- die Bohrsche Kreisbahn ist bei einem Wasserstoffatom der __wahrscheinlichste Abstand vom Kern__
**********


{{3}}
**********
> Die räumliche Wahrscheinlichkeitsverteilung nennt man @color(Orbital, red). Je nach Quantenzahl haben diese Orbitale unterschiedliche Formen. <br> [Simulation](https://www.leifiphysik.de/atomphysik/quantenmech-atommodell/versuche/wellenfunktionen-orbitale-des-wasserstoffatoms-simulation-von-paul-falstadt) & [Video 2](https://www.youtube.com/watch?v=2e31oqxlkJg)
**********

{{4}}
**********
__Bemerkungen:__

- das einfachste Orbital (K-Schale) ist kugelförmig

- je größer die Hauptquantenzahl n (K->L->M), desto weiter weg ist der wahrscheinlichste Aufenthaltsort des Elektrons

- [Orbitale](https://commons.wikimedia.org/wiki/Hydrogen_orbitals_3D_real) können z.B. kugelförmig, hantelförmig oder dounutförmig sein
**********

{{5}}
**********
<p style="margin-left:10%">
![Ausschnitt-Atomorbitale](https://diversewolken.ddns.net/nextcloud/s/2fDBpE4c7sQx6Et/download "n-Hauptquantenzahl, m-Nebenquantenzahl ")
</p>
**********


## 8. 5. Quantenhafte Absorption und Emission von Energie

> Wenn Elektronen das Energieniveau wechseln, kann Energie aufgenommen oder abgegeben werden.
>
> @color(__Der Energiebetrag entspricht dabei der Differenz der Energieniveaus.__, red)

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Absorption von Energie__

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Emission eines Photons__

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

---

Elektron wird auf eine höhere Bahn gehoben. Es muss Energie hinzugefügt werden.

---

![Absorption](https://diversewolken.ddns.net/nextcloud/s/BQ2Z5Apxa9TyqR4/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

---

Elektron springt auf eine niedrigere Bahn. Es wird Energie in Form eines Photons abgegen.

---

![Emission](https://diversewolken.ddns.net/nextcloud/s/wRYRWkGLbYcMqqA/download)

</div>

</section>

### Übungsaufgaben zu Orbitalen und Energieaustausch

<details>

<summary> 1. __Aussagen zu Atomorbitalen__ </summary>

1. 1. Welche Aussage beschreibt ein **Orbital** im quantenmechanischen Atommodell am besten?

<p style="margin-left:10%">

- [( )] Ein Orbital ist die feste Kreisbahn, auf der das Elektron um den Kern fliegt.
- [(X)] Ein Orbital ist ein Raumbereich, in dem sich ein Elektron mit hoher Wahrscheinlichkeit aufhält.
- [( )] Ein Orbital ist der Ort, an dem das Elektron immer exakt gefunden wird.
- [( )] Ein Orbital ist eine messbare Bahnkurve, die man mit einem Mikroskop sehen kann.
- [( )] Ein Orbital ist nur eine Zeichnung ohne physikalische Bedeutung.
- [( )] Ein Orbital ist identisch mit der Schale (z.B. „2. Schale“), mehr gibt es da nicht.

</p>

---

1. 2. Was bedeutet „Aufenthaltswahrscheinlichkeit“ bei Elektronen?

<p style="margin-left:10%">

- [( )] Sie sagt, wie schnell das Elektron unterwegs ist.
- [( )] Sie sagt, wie warm das Elektron ist.
- [(X)] Sie gibt an, wie wahrscheinlich es ist, ein Elektron in einem bestimmten Raumbereich zu finden.
- [( )] Sie gibt an, wie wahrscheinlich es ist, dass der Atomkern verschwindet.
- [( )] Sie ist die Wahrscheinlichkeit, dass das Elektron auf einer festen Bahn bleibt.
- [( )] Sie ist eine Zufallszahl ohne Bezug zu Messungen.

</p>

---

1. 3. Warum zeichnet man im quantenmechanischen Atommodell **keine festen Elektronenbahnen** wie im Bohr-Modell?

<p style="margin-left:10%">

- [( )] Weil Elektronen zu klein sind, um Bahnen zu haben.
- [(X)] Weil Ort und Impuls nicht gleichzeitig beliebig genau bestimmbar sind (Unschärferelation).
- [( )] Weil der Atomkern das Elektron „nicht reinlässt“.
- [( )] Weil Elektronen immer im Kreis fliegen.
- [( )] Weil die Elektronen ständig zwischen den Bahnen hin und her sprichen.

</p>

---

1. 4. Je größer die Hauptquantenzahl n, ..

<p style="margin-left:10%">

- [( )] desto geringer ist die Ausdehnung des Atomkerns.
- [( )] desto größer ist die Ausdehnung des Atomkerns.
- [( )] desto näher am Kern ist der wahrscheinlichste Fundort (bei einer Messung) des Elektrons.
- [(X)] desto weiter vom Kern entfernt ist der wahrscheinlichste Fundort (bei einer Messung) des Elektrons.

</p>

</details>


---

<details>

<summary> __2. Aussagen zu Absorption und Emission von Energie bei einem Atom__ </summary>

2. 1. Absorption: Wann passiert sie? <br> Wann wird bei einem Elektronenübergang **Energie absorbiert**?

<p style='margin-left:10%'>

- [( )] Wenn ein Elektron von einem höheren auf ein niedrigeres Energieniveau wechselt.
- [(X)] Wenn ein Elektron von einem niedrigeren auf ein höheres Energieniveau wechselt.
- [( )] Wenn ein Elektron im gleichen Energieniveau bleibt.
- [( )] Wenn ein Elektron den Atomkern berührt.
- [( )] Immer, egal in welche Richtung der Übergang geht.
- [( )] Nur wenn das Elektron vorher schon leuchtet.

</p>

---

2. 2. Emission: Was wird frei? Was passiert bei einem Übergang von einem **höheren** auf ein **niedrigeres** Energieniveau?


<p style='margin-left:10%'>

- [( )] Das Atom absorbiert ein Photon.
- [(X)] Das Atom emittiert Energie, oft als Photon (Licht).
- [( )] Das Elektron gewinnt Energie und springt nach außen.
- [( )] Es passiert nichts: Energieniveaus sind nur Theorie.
- [( )] Die Protonenzahl ändert sich.
- [( )] Das Elektron wird zu einem Proton (ist doch alles elektrisch).

</p>

---


2. 3. Zusammenhang Energie – Lichtfarbe <br> Welche Aussage ist richtig?



<p style='margin-left:10%'>

- [( )] Je größer die Energiedifferenz ΔE, desto kleiner die Photonenenergie.
- [( )] Die Farbe hängt nur von der Anzahl der Elektronen ab.
- [( )] Alle Übergänge haben die gleiche Photonenergie, so lange die Änderung der Quantenzahl gleich ist (z.B. $\Delta n=1$)
- [( )] Ein Photon kann nur bei Absorption entstehen, nicht bei Emission.
- [(X)] Je größer die Energiedifferenz ΔE, desto energiereicher (z.B. „blauer“) ist das emittierte/absorbierte Photon.
- [( )] Die Photonenenergie ist unabhängig vom Übergang.

</p>

</details>

---

<details>

<summary> __3. Berechnungen zur Emission und Absorption von Energie__ </summary>

3. 1. Die Emissionen, die beim Wasserstoffatom im sichtbaren Bereich liegen, sind Übergänge auf die zweite Schale. Ermitteln Sie die Energie und die Wellenlänge der Übergänge von n=3 -> n=2. Notieren Sie die Farbe des emittierten Lichts.

<p style='margin-left:10%'>

@rangeQuiz2($E_{3->2}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{3->2}$,655e-9,$\mathrm{m}$)

<!-- data-solution-button="off" -->
[[ infrarot | rot | gelb | grün | blau | violett | ultraviolett ]]

</p>

---

3. 2. Ein Photon der Wellenlänge 102,64 nm wird von einem Wasserstoffatom absorbiert. Ermitteln Sie, welche Bahnen des Wasserstoff-Atoms an diesem Übergang beteiligt sind.

<p style='margin-left:10%'>

von n= [[ 1 ]] auf n=[[ 3 ]]

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Ermitteln Sie die Photonenergie in der Einheit eV. Nutzen Sie die Formel für die Energieniveaus am Wasserstoffatom und überprüfen Sie, welchem Übergang die Photonenenergie entspricht.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Das Elektron springt auf die dritte Bahn.

</details>


</details>

---


## 8. 6. LASER - Prinzip und Funktionsweise

> __Eigenschaften von Laserlicht (im @color(Wellen-, red) und @color(Teilchenbild, blue)):__
>
> - __intensiv__ - @color(Lichtwelle hat hohe Amplitude, red) olor(viele Photonen, blue)
>
> - __monochromatisch__ - @color(nur eine Wellenlänge, red) | @color(nur eine Energie, blue)
>
> - __kohärent__ - @color(Phasenbeziehung konstant -> Wellenberg auf Wellenberg/Wellental auf Wellental, red) <br> ![Kohaerenz](https://diversewolken.ddns.net/nextcloud/s/KzCZZR9iPqDGYKq/download)

---

>__Emission von Photonen:__
>
> Vorraussetzung, dass ein Photon von einem Atom emittiert werden kann sind:

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

> Ein Elektron des Atoms befindet sich in einem angeregten Zustand (z.B. durch Absorption eines Photons)
>
> ![Absorption](https://diversewolken.ddns.net/nextcloud/s/pfZky8257jAsgWc/download)


</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">


> __Spontane__ Abregung des Elektrons (fällt auf ein niedrigeres Niveau), führt __nicht__ zum Laser <br> <br>
>
> ![SpontaneEmission](https://diversewolken.ddns.net/nextcloud/s/Prt82L92MdGN9tT/download)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">


> __Stimulierte Emission:__ Ein Photon (Ph1), mit der gleichen Energie wie die Bandlücke, regt das angeregte Elektron ab (Sprung auf niedrigeres Niveau) zur Emission eines zweiten Photons Ph2
>
> ![StimulierteEmission](https://diversewolken.ddns.net/nextcloud/s/JX66oNPLPAqdFnH/download)


</div>

</section>




---

>__Eigenschaften der Photonen Ph1 & Ph2 bei stimulierter Emission:__
>
> 1. Photon Ph2 hat die selbe Wellenlänge/Energie, wie Ph1 -> @color(__monochromatisches Licht__, red)
> 
> 2. Phase (Wellenberg/Wellental) von Ph1 und Ph2 sind gleich -> @color(__kohärentes Licht__, red)



>__Vorraussetzung fürs Lasen:__
>
> Lasen: kontinuierliche Lichtabgabe mit hoher Intensität
>
> __Besetzungsinversion:__ Es befinden sich mehr Atome in einem angeregten Zustand
>
> __Metastabiler/Triplet Zustand:__ Die angeregten Elektronen verbleiben sehr __lange in ihrem Zustand__, @color(ohne spontan zu emittieren, blue)




<details style='color:blue;margin-left:10%'>

<summary> Beispiel: He-Ne Laser </summary>

![He-Ne-Laser-Schema](https://diversewolken.ddns.net/nextcloud/s/B8g9KP7fYCsC7Zn/download)

</details>
