<!--
author: Christian Golnik

language: de

link: https://gist.githubusercontent.com/andre-dietrich/3c69f68b2c4d80c8c6eb177229ae1ae8/raw/31cde15c4a7f3c2eda7d5ebdea440205f366acad/hideCircle.css

-->

# Feedback zu LIA-Classroom


> Hallo Andre

    .. ich hatte dir vor einer Weile ein Feedback zu LIAScript Classroom (LIA-CR) versprochen .. 

    Ich teste LIA nun in mittlerweile Gymnasialklassen (Stufe 8 und 10) und bin im großen und ganzen sehr begeistert. Ich habe vor kurzem begonnen, Classroom einzusetzen. Dazu ein kleines Feedback (Bitte als konstruktives Feedback auffassen und nicht als Kritik an der Sache).

## Vorbemerkung

Der m.E. nach Interessanteste Aspekt von LIA-CR sind die Quizzes und Surveys. In meinen Klassen spielt es für die Lernenden eine wichtige Rolle, dass sie bei interaktiven Elementen ein direktes Feedback bekommen, d.h. ob sie etwas richtig oder falsch gemacht haben. Das geht ganz wunderbar und hat m.E. nach einen echten Mehrwert (ist aber eigentlich immer noch kein CR-Feature, oder?). 

Ich zeige dir hier mal ein Beispiel und verlinke konkret die Seite die ich meinte:

??[bsp2](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche/master/Skripte/LIA/bsp2.md#1)

## Mein Eindruck

Ich sehe in LIA eine wirklich gute Möglichkeit für selbstständiges / selbstgesteuertes Lernen, d.h. die SuS     

 - bearbeiten in ihrem Tempo einen Lernblock

 - Lösen Aufgaben

 - Rechnen, Spielen usw. 
    
Das direkte Feedback, wer welche Aufgabe wie gut gemacht hat (was LIA-CR nach vielen Antworten bietet) hat meine Lernenden in meinen Beobachtungen überhaupt nicht interessiert. Konkret: Wird angezeigt, beim wievielten Trial andere die Aufgabe gelöst haben, wird das (falls es verstanden wird) <span style="color:orange">entweder ignoriert, oder es wird gelästert oder ich werde gefragt, ob das Histogramm auch abgeschrieben werden soll</span>. 

{{1}}
***************
> Zugegeben: Da müsste ich vielleicht noch eine bessere (technische) Vorbereitung bieten, my bad (die Zeit wird es zeigen).
***************

## Mein Lernziel

Ziel ist in meinem oben genannten Beispiel, dass die Lernenden 

> Die Aufgabe bereits erledigt haben und nur noch vergleichen 

oder 

> im Falle von Fehlern ihre Lösung vergleichen und gegeben falls korrigieren 

oder (_miau_)

> einfach nur abschreiben [worst case]. 

Leider hat m.E. das CR-Feedback mit den entsprechenden Trials in keinem der didaktischen Niveaus einen Nutzen. Es ist in diesem Fall, für die Lernenden eher hinderlich gewesen (ich meine das hier nur konkret auf meinen Fall bezogen).

## Ich als Lernbegleiter

Für mich als Lernbegleiter hingegen ist hier eine Sache sehr wichtig: 

> Ich weiß bzw. möchte gern wissen, _ohne bei jedem auf den Bildschirm zu schauen_, wieviele SuS eine bestimmte Aufgabe bereits erreicht haben (und ggf. richtig gelöst haben). 

In meinem konkret schulischen Fall, wo es um Wissensvermittlung ging und nicht um ein gemeinsames Auswerten von Meinungen / Stimmungen / Ideen, konnte die Power, die LIA-CR mitbringt nicht so richtig genutzt werden. 

_Ich hätte mir für mich, eher eine Feedback-Zusammenfassungs-Seite gewünscht (die ich auf dem Beamer hab), wo ich den Fortschritt innerhalb des Dokuments überblicken._

## Und sonst noch ..

Mir ist bewusst, das LIA-CR auch für andere Umgebungen konzipiert ist und da u.U. viel wirkungsvoller genutzt werden kann.

Technisch gesehen, hat LIA-CR absolut einwandfrei funktioniert, ich hatte keine Verbindungsprobleme oder andere Störungen. Als Tool hatte ich Gun genutzt.

# Weiter Wünsche / Vorschläge

Nun noch einige LIA-spezifische Fragen/Anmerkungen, die mir im Laufe meiner doch sehr intensiven Nutzung aufgefallen sind:

### 1. Hauptframe in zwei oder drei gleich breite Spalten teilen

Es passiert mir häufiger, dass ich den Bildschirm effektiver nutzen will und mir da die Hände gebunden sind. Beispielsweise wünsche ich mir in einigen Fällen, den Bildschirm geschickt in zwei (oder drei) horizontale Spalten teilen zu können und darin dann beliebig zu walten. Mir ist bewusst, dass dies prinzipiell mit Tabellen möglich ist (z.b. | .. | .. |), aber bei dieser Formatierung stoße ich immer wieder an grenzen, weil ich innerhalb einer Spalte komplexere Elemente (z.B. Latex-Code, Farbigen Text, eine Aufzählung) drin haben möchte und es mir noch nicht gelungen ist, dem LIA-Interpreter meine Wünsche adäquat zu codieren. Gibt es da eine andere Möglichkeit?

In folgendem Beispiel sieht man was ich meine. Ich hätte gern das Bild direkt neben der Lösung (ist mir nicht gelungen.)

??[bsp1](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche/master/Skripte/LIA/bsp1.md)

### 2. Farbiger Text 

Momentan nutze ich CSS als Umweg, gibt es eine einfachere Möglichkeit Text farbig zu gestalten? Mein Beispiel:

`<span style="color:red">Schnittpunkt bei $( -\frac{\pi}{2} | -4 ) $ </span>`

<span style="color:red">Schnittpunkt bei $( -\frac{\pi}{2} | -4 ) $ </span>



### 3. Einstellungen im Link

Zum Effektiven Teilen mit Lernenden würde ich gern im Link bereits einige Einstellungen mit übergeben z.B.:

Modus: "Präsentation" (in nightly "Navigation" - was ich beinahe immer verwende wegen der besser genutzten Bildschirmfläche).

Schriftgröße: Medium

### 4. Archivieren

Ich möchte meine Kurse gern archivieren und zwar nicht als .md - Datei, sondern als Kurs, als PDF-Datei. Plant ihr eine Möglichkeit die Webseite als PDF zu speichern? 

Z.B. im Textbuch Modus (Auch falls mal alles Offline ist?) 

<span style="color:orange">***<H5>Das wäre großartig!!</H5>***</span>

<span style="color:blue">***Oder gibt es einen Workaround?***</span>

# Danke fürs Lesen

_es ist spät geworden_


<iframe src="https://giphy.com/embed/A3556xyE9eMyE7ETv2" width="480" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>