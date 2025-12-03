<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg 

logo: https://www.projektmagazin.de/sites/default/files/inline-images/4-seiten-einer-nachricht.JPG

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

mode: textbook

@onload
window.LIA.settings.font_size = 2
@end

@color
<bdi style="color:@1">@0</bdi>
@end

-->


# Axiome von P. Watzlawick und Vier-Ohren-Modell

### Quiz - Axiome nach Watzlawick

<iframe src="https://www.testedich.de/widget.php?quiz=67&id=1611253998&theme=nice-blue&lang=de&width=550&height=400" width="550" height="400" frameborder="0"></iframe>



## Vier-Ohren-Modell

!?[4-Ohren-Modell](https://www.youtube.com/watch?v=9VJn1cPbf1A)

### Beispielvideo - 4-Ohren

{{0-1}}
!?[4-Ohren](https://diversewolken.ddns.net/nextcloud/index.php/s/oosk3pMxeNoMSnL/download)

{{1-2}}
![Reaktion](https://diversewolken.ddns.net/nextcloud/index.php/s/kjQAmqN5DkjzEA9/download)

{{2}} 
> Sachohr: Sag es nicht, wenn du es nicht so meinst.

{{3}}
> Appelohr: Überleg dir genau, was du sagst.

{{4}}
> Beziehungsohr: Unsere Beziehung (sehr frisch), kann solche zweideutigen Bemerkungen nicht aushalten

{{5}}
> Selbsoffenbahrungsohr: Ich bin empfindlich, was pauschale Aussagen über Weiblichkeit/Männlichkeit betrifft

#### Quiz - 4 - Ohren-Modell

<iframe src="https://www.testedich.de/widget.php?quiz=73&id=1669667273&theme=blue-round&lang=de&width=550&height=400" width="550" height="400" frameborder="0"></iframe>

#### Quiz - 5 - Kommunikationsstörungen

Wahrnehmung, Interpretation oder Gefühl? Entscheide, auf welchen Vorgängen die Äußerungen beruhen.

1. Du bist desinteressiert.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [(x)] Interpretation
     [( )] Gefühl

2. Du warst 60 Minuten im Bad.

     <!-- data-solution-button="off" -->
     [(x)] Wahrnehmung
     [( )] Interpretation
     [( )] Gefühl

3. Ich habe dich gestern mit einem anderen Mädchen gesehen.

     <!-- data-solution-button="off" -->
     [(x)] Wahrnehmung
     [( )] Interpretation
     [( )] Gefühl

4. Ich bin heute schlecht drauf.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [( )] Interpretation
     [(x)] Gefühl

5. Er hat nichts gesagt.

     <!-- data-solution-button="off" -->
     [(x)] Wahrnehmung
     [( )] Interpretation
     [( )] Gefühl

6. Du liebst mich nicht mehr so sehr wie am ersten Tag.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [(x)] Interpretation
     [( )] Gefühl

7. Du kritisierst mich.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [(x)] Interpretation
     [( )] Gefühl

8. Deine Aussage verletzt mich.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [( )] Interpretation
     [(x)] Gefühl

9. Ich fühle mich hintergangen.

     <!-- data-solution-button="off" -->
     [( )] Wahrnehmung
     [( )] Interpretation
     [(x)] Gefühl


#### KI-Aufgabe: Kommunikationsmodelle

<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.
</p>

---

__Aufgabe:__<br> Beantworte die Aufträge der KI. Du kannst dein Ergebnis verbessern, oder zur nächsten Frage springen.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Grundlage der folgenden Kommunikation sind die beiden Kommunikationsmodelle 5-Axiome von Paul Watzlawick und das 4-Ohren-Modell nach Friedemann Schulz von Thun. Ich möchte dass du mir 5 Fragen aus diesen beiden Themengebieten stellst. Bitte achte darauf, dass die Antworten nicht zu lang sein müssen. Ich bin ein Einsteiger in diesem Thema. Gib mir nach jeder Frage ein Feedback und frage mich, ob ich meine Antwort verbessern möchte. Gib mir nicht die Lösung, aber unterstütze mich bei der Beantwortung. Nach der fünften Frage möchte ich, dass du meine Antworten auf einer Skala von 1 bis 10 einschätzt und mir ein Feedback gibst.</span>
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
