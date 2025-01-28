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

# SHILF IPADs und Cassy

1. [SHILF - IPads](#1.-ipads)

1. 1. [Zuordnung Geräte](#1.-1.-umgang-mit-den-geräten-und-zuordnung-von-lernenden
)

1. 2. [VorJederStunde](#1.-2.-vor-jeder-stunde)

1. 3. [Probleme?](#1.-3.-probleme-oder-wünsche)

1. 4. [Kurzfassung](#1.-4.-kurzfassung)

---

2. [Anleitung zur Verbindung von Cassy und Tablet](#2.-anleitung-zur-verbindung-von-cassy-und-tablet)

     [Einführungsvideo zu Mobile-Cassy 2](#einführungsvideo-zu-mobile-cassy-2)

2. 1. [Schüler-Experiment: U-I-Kennlinie mit Cassy - Manuelle Messwertaufnahme](#2.1-schülerexperiment:-u-i-kennlinie-mit-cassy-manuelle-messwertaufnahme)

2. 2. [Schülerexperiment: U-I-Kennlinie mit Cassy - Automatische Messwertaufnahme](#2.2-schülerexperiment:-u-i-kennlinie-mit-cassy-automatische-messwertaufnahme)

2. 3. [Schülerexperiment: Entladekurve Kondensator](#2.3-schülerexperiment:-entladekurve-kondensator)

2. 4. [Schülerexperiment: Messungen der magnetischen Flussdichte](#2.4-schülerexperiment:-messungen-der-magnetischen-flussdichte)


# 1. SHILF - IPads

Gliederung - 10min

- Umgang mit Geräten und Zuordnung von Lernenden
- Wie verteilt man Webseiten und Dokumente
- Apple-Classroom

## 1. 1. Umgang mit den Geräten und Zuordnung von Lernenden

Wir haben gute Erfahrungen damit gemacht, den SuS feste IPads, d.h. feste Nummern zuzuordnen 

=> Idee: Achtsamer Umgang

### Vorschläge zur Zuordnung

1. Registrierung von IPad-Nummer, Klasse und Schüler*in

oder

2. Feste Nummern auf den Tischen

oder

3. Liste schreiben

### Registrierung von IPad-Nummer, Klasse und Schüler*in

Auf jedem Lehrer-IPad ist ein Link auf dem Desktop. Hier können die SuS in der ersten Stunde ihr IPad zum Namen registrieren.

![Logo](https://diversewolken.ddns.net/nextcloud/index.php/s/daeDQDtLp6k3BHT/download)

Dieser Link muss __einmalig__ mit den Lernenden geteilt werden.

{{1}}
***********

Öffnet man diesen Link so sieht das so aus:

??[IPad-Reg](https://forms.microsoft.com/Pages/ResponsePage.aspx?id=OYkUKbuZEE6zqVVLeyuod-N98JNwJnhAr0ZoZo5y2cdUQlE5S05TRUdKSVJQVDJHM0w3UFdPMkdJSS4u)
***********

{{2}}
***********
Auf dem Lehrer IPad gibt es einen zweiten Link. Dort sind dann die eingetragenen SuS mit IPad Nummern zu sehen.

![SuS](https://diversewolken.ddns.net/nextcloud/index.php/s/meSGztTL8gAJFpZ/download)

***********

## 1. 2. Vor jeder Stunde

Zu Beginn jedes Unterrichtes sollte der Apple-Classroom auf dem Lehrer-IPad geöffnet werden.

![AppleClassroom](https://help.apple.com/assets/64FA4E962B9CCDCEC80ED904/64FA4E98620FE6D9040E4F44/de_DE/b841ccb47e8104c9630c378a2c1b225b.png)

Im Apple-Classroom können

- alle IPads eingesehen werden

- Links oder Dokumente per Airdrop verteilt werden

- Apps zugelassen oder gesperrt werden

- die Nutzung einzelner Apps eingesehen werden

__Screenshot:__

{{1}}
**********
![Screenshot](https://diversewolken.ddns.net/nextcloud/index.php/s/fnA8eNqrytmefom/download)
**********

{{2}}
**********
Jede Webseite und jedes Dokument (z.B. PDF-Datei) kann über Air-Drop an die gesamte Gruppe verteilt werden.

Teilen klicken und: 

| Teilen => | Airdrop |
| ![AppleTeilen](https://diversewolken.ddns.net/nextcloud/index.php/s/NF7YMnHZ8gNeY7c/download) | ![AirDrop](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/AirDrop_logo.svg/255px-AirDrop_logo.svg.png) |

**********

## 1. 3. Probleme oder Wünsche

Können auf dem Lehrer-IPad unter diesem Logo eingetragen werden.

![Wuensche](https://diversewolken.ddns.net/nextcloud/index.php/s/mkikXomFLTd7ffT/download)

Das sieht dann so aus:

??[WünscheProbleme](https://gykl-my.sharepoint.com/:w:/g/personal/golnik_ch_gykl_onmicrosoft_com/EVMmssf-S9BGlYR9cE-xbUUBM6UFTHikKFJ1H6RlrfgHvA?e=U3aBxd)

## 1. 4. Kurzfassung

| | | |
| Einmal | Registrieren | ![Logo](https://diversewolken.ddns.net/nextcloud/index.php/s/daeDQDtLp6k3BHT/download)<!--style="width: 100px"--> ![SuS](https://diversewolken.ddns.net/nextcloud/index.php/s/meSGztTL8gAJFpZ/download)<!--style="width: 100px"-->  |
| Vor der Stunde | Classroom starten | ![AppleClassroom](https://help.apple.com/assets/64FA4E962B9CCDCEC80ED904/64FA4E98620FE6D9040E4F44/de_DE/b841ccb47e8104c9630c378a2c1b225b.png)<!--style="width: 100px"--> |
| Während der Stunde | Teilen & Airdrop | ![AppleTeilen](https://diversewolken.ddns.net/nextcloud/index.php/s/NF7YMnHZ8gNeY7c/download)<!--style="width: 100px"--> ![AirDrop](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/AirDrop_logo.svg/255px-AirDrop_logo.svg.png)<!--style="width: 100px"--> |
| Probleme/Wünsche | Bitte eintragen | ![Problem](https://diversewolken.ddns.net/nextcloud/index.php/s/mkikXomFLTd7ffT/download)<!--style="width: 100px"--> | 
| Nach der Stunde | Klasse beenden | ![AppleClassroom](https://help.apple.com/assets/64FA4E962B9CCDCEC80ED904/64FA4E98620FE6D9040E4F44/de_DE/b841ccb47e8104c9630c378a2c1b225b.png)<!--style="width: 100px"--> |



# 2. Anleitung zur Verbindung von Cassy und Tablet

## Einführungsvideo zu Mobile-Cassy 2

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

__Grundlage:__ Jedes __Mobile Cassy 2__-Messgerät (im Folgenden mit _Cassy_ bezeichnet) kann mit Hilfe einer W-Lan Verbindung über das Tablet ferngestuert werden. Dabei können Messparameter eingestellt, Messungen gestartet und Messdaten abgespeichert werden. Hier wird das Tablet mit dem Cassy verbunden.

__Arbeitsablauf:__

- nach Einschalten von _Cassy_ baut das Gerät selbstständig eine W-Lan Verbinung auf

- wechseln Sie mit den Pfeilen auf dem roten runden Bedienfeld des Cassy zum Menu Einstellungen (oben rechts, Kreis mit Ausrufezeichen 

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/cbw8JJBd7AAetEz/download)<!-- style="max-width:300px; margin-left:20%"-->

- wählen Sie QR-Code anzeigen, wechseln Sie zu AP-Daten und scannen Sie den angezeigten QR-Code mit dem Tablet -> das Tablet wird sich mit dem Cassy verbinden

- wenn ihr Tablet mit dem _Cassy_-WLan verbunden ist, öffnen Sie einen neuen Tab im Safari-Webbrowser und öffnen Sie folgende Adresse [http://10.10.10.1](http://10.10.10.1)

![Cassy-WLan](https://diversewolken.ddns.net/nextcloud/index.php/s/zgynA6RKTTEaM4Y/download)<!-- style="max-width:80%; margin:5%"-->

- zu sehen ist die Live-Anzeige der aktiven Sensoren

## 2.1 Schülerexperiment: U-I-Kennlinie mit Cassy - Manuelle Messwertaufnahme

__Aufgabenstellung:__ Nimm mit die U-I-Kennlinie für einen ohmschen Widerstand ($R=512\Omega$) auf. Variiere die Spannung in Schritten von 1 V im Intervall 0 - 10 V.


<p style="color:blue">

__Durchführung:__ _(muss nicht notiert werden)_ 

1. Übernimm Überschrift und Aufgabenstellung auf eine neue Seite.

2. Übernimm den Schaltplan und die zugehörige Tabelle für die Messwerte.

3. Stelle das Cassy-Messgerät anhand der Erklärungen ein.

4. Variiere die Spannung an der Spannungsquelle von 0..10V in Schritten von 1 V. Notiere Spannung und Stromstärke an Cassy-Messgerät.

5. Zeichne eine U-I-Kennlinie: Zeichne dazu ein Diagramm (x-Achse: U in V | y-Achse: I in A).

6. Öffne die nächste Seite: @color(_1.7.2 Automatische Messwert-Erfassung mit Cassy_,darkgreen). Folge den Anweisungen und wiederhole die Messung mit einer Automatischen Messwert-Aufname.

</p>

<p class="newspaper">

__Schaltkreis:__

![Schaltkreis_Exp1](https://diversewolken.ddns.net/nextcloud/index.php/s/rAwYZqysffqknd6/download)

{{0-1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | |
| 1 | |
| 2 | |
| .. | |
| 9 | |
| 10 | |
************

{{1}}
************
__Messwerte-Tabelle:__

| U in V | I in A |
| :---: | :---: |
| 0 | 0,002 |
| 1 | 0,004 |
| 2 | 0,006 |
| 3 | 0,008 |
| ..| .. |
| 9 | 0,018 |
| 10 | 0,02 |
************

<p class="cb">

__Diagramm Kennlinie:__

{{0-1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/Z9at8rKH75N4Agt/download)
*************

{{1}}
*************
![VGl-Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/s/ztd7ScndfNAYNqM/download)
*************

<details  style="color:blue">

<summary>__Einstellen des Cassy-Messgerätes:__</summary>

_(muss nicht notiert werden)_

1. Schließe den blauen Anschluss (_I_) an den Minuspol der Spannungsquelle. Der schwarze Anschluss wird an den Widerstand angeschlossen.

2. Schalte das Cassy-Messgerät ein. Im oberen linken Bereich des Fensters sind die messbaren Größen dargestellt. Deaktiviere mit [Cursor-Rad + OK] die Spannung und aktiviere die Stromstärke.

![VGl-Cassy1](https://diversewolken.ddns.net/nextcloud/index.php/s/e7eaHcHB4YkGf95/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Klicke auf das Symbol für Stromstärke (I) und stelle für den (Mess-)Bereich [-0,03A .. 0,03A] ein. Wechsle zurück Anzeige der Stromstärke. Achte auf: __Nullpunkt links__.

![VGl-Cassy2](https://diversewolken.ddns.net/nextcloud/index.php/s/JiSJbjqy3SkS2CN/download)<!-- style="max-width:80%;margin-left:10%" -->

</details>

</p>

</p>

!?[Einführung-Mobile-Cassy2](https://www.youtube.com/watch?v=2gPGb_NdbqM)

## 2.2 Schülerexperiment: U-I-Kennlinie mit Cassy - Automatische Messwertaufnahme

In dieser Messreihe wird die Kennlinie vom Cassy-Messgerät automatisch aufgenommen.

1. Schalte die Spannungsquelle ab.

2. Verbinde mit einem weiteren Kabel den @color(roten Pol __U__, red) des Cassy-Gerätes mit einem Kontakt hinter dem Widerstand.

![VGl-Cassy3](https://diversewolken.ddns.net/nextcloud/index.php/s/LxJxpcGsAmAeJJt/download)<!-- style="max-width:80%;margin-left:10%" -->

3. Erweitere deine angezeigten Messwerte auf Spannung U und Stromstärke I. Achte auf __Bereich 0V .. 10V__ und __Nullpunkt links__.

![VGl-Cassy4](https://diversewolken.ddns.net/nextcloud/index.php/s/sXkCT7eGYWyrCYX/download)<!-- style="max-width:80%;margin-left:10%" -->

4. Wechsle zur Anzeige von Spannung und Stromstärke. Schalte die Spannungsquelle ein und vergleiche drei Messwertpaare der angezeigten Daten mit den Daten deiner Messwerttabelle (oben). <br> @color(Stimmen sie überein, red) nimmt Cassy nun korrekt Spannung und Stromstärke auf.

5. Stelle die Spannung an der Spannungsquelle auf 0 V.

6. Wähle nun oben rechts den __Diagramm Modus__. Stelle für die x-Achse die Spannung und für die y-Achse die Stromstärke ein. 

![VGl-Cassy5](https://diversewolken.ddns.net/nextcloud/index.php/s/4nJbMTEEjwz3SJd/download)<!-- style="max-width:80%;margin-left:10%" -->

7. Starte die automatische Messwerterfassung -> Wechsel auf Uhr oben links. 

![VGl-Cassy6](https://diversewolken.ddns.net/nextcloud/index.php/s/cHFbdz2ZQJGFTsE/download)<!-- style="max-width:80%;margin-left:10%" -->

8. Drehe die Spannung an der Spannungsquelle langsam von 0 V -> 10 V und beobache die dargestellten Messwerte. Vergleiche deine Darstellung mit dem hier gezeigten Erwartungsbild.

![VGl-Cassy7](https://diversewolken.ddns.net/nextcloud/index.php/s/f93rWiDbtDkR6Jj/download)<!-- style="max-width:80%;margin-left:10%" -->

9. @color(Dieses Diagramm und dein Messwertdiagramm sollten übereinstimmen., red)

## 2.3 Schülerexperiment: Entladekurve Kondensator

__Aufgabenstellung:__ Untersuche den Entladevorgang eines Kondesators mit Hilfe der elektronischen Messwerterfassung ***Mobile Cassy 2***.

__Teilaufgaben:__ (_können_ in selbst gewählter Reihenfolge bearbeitet werden)

- [ ] Inhalten eines Protokolls notieren

- [ ] Vorbetrachtungen zum Versuch vornehmen und notieren

- [ ] ***Mobile Cassy 2*** mit Tablet/Laptop verbinden

- [ ] Einstellen der Parameter am Cassy

- [ ] Schaltkreis zur Messung aufbauen @color(und von Lehrkraft abnehmen lassen, red)

- [ ] Messwerte aufzeichnen

- [ ] Daten auswerten und Ergebnisse analysieren

- [ ] Ergebnisse formulieren

### Vorbetrachtungen zum Versuch

<p class="newspaper">

__Schaltplan:__

![Kondensator_Ladekreis_2](https://diversewolken.ddns.net/nextcloud/index.php/s/JqJRbJpBMJXNwTq/download)

<p class="cb">

__Ladekreis__ 

Der Kondensator wird in dieser Schaltung direkt über die Spannungsquelle und ohne ohmschen Widerstand aufgeladen.

__Entladekreis:__

Wird der Entladekreis geschlossen, fließt die auf dem Kondensator gespeicherte Ladung $Q$ über den ohmschen Widerstand $R$ ab. Dabei wird mit der elektronischen Messwerterfassung _Cassy_ der Entladestrom $I$ in Abhängigkeit der Zeit $t$ aufgenommen. Die gesamte Messzeit wird mit $T$ bezeichnet (s.u.).

{{1}}
*****
__Ermittlung der Ladung $\,Q$:__

Die vom Kondensator abgeflossene Ladung $Q$ entspricht im @color(Zeit-Stromstärke-Diagramm, blue) der <bdi style="color:red"> __Fläche unter dem Graphen $I(t)$__</bdi>.
*****

{{1-2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/Q9MwZdw5ZxwfrcN/download)<!-- style="max-width:80%; margin:5%"-->
*****

{{2}}
*****
![I(t)_Graph](https://diversewolken.ddns.net/nextcloud/index.php/s/GSN44xxcqTH4HH6/download)<!-- style="max-width:80%; margin:5%"-->

Die Fläche unter dem $I(t)$ Graphen kann mit Hilfe des Cassy-Messgerätes ausgewertet werden.

*****

{{3}}
*****
__Ermittlung der Messdauer $T$ für Cassy:__

Für die Kombination aus Kondensator (Kapazität $C$) und ohmscher Widerstand (Widerstand $R$) kann eine Zeitkonstante $\tau$ ermittelt werden: 

$$ \boxed{\tau = R \cdot C} \Rightarrow \boxed{T = 4 \cdot \tau} $$

Als Messdauer $T$ für die elektronische Erfassung wird eine Zeit von @color($4\tau$,red) empfohlen. Nach dieser Zeit sind ca. $98,2\%$  der Gesamtladung Q abgeflossen.
*****

</p>

</p>

### Anleitung zur Verbindung von Cassy und Tablet/Laptop

__Grundlage:__ Jedes __Mobile Cassy 2__-Messgerät (im Folgenden mit _Cassy_ bezeichnet) kann mit Hilfe einer W-Lan Verbindung über das Tablet/Laptop ferngestuert werden. Dabei können Messparameter eingestellt, Messungen gestartet und Messdaten abgespeichert werden. Hier wird das Tablet/Laptop mit dem Cassy verbunden.

__Arbeitsablauf:__

- nach Einschalten von _Cassy_ baut das Gerät selbstständig ein W-Lan Netzwerk auf

<p class="newspaper">

__Tablet:__

- wechseln Sie auf dem Cassy zum Menu Einstellungen (oben rechts) 

- wählen Sie QR-Code anzeigen, wechseln Sie zu AP_Daten und scannen Sie den angezeigten QR-Code mit dem Tablet -> das Tablet wird sich mit dem Cassy verbinden

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/cbw8JJBd7AAetEz/download)<!-- style="max-width:300px; margin-left:20%"-->

- wenn ihr Tablet mit dem _Cassy_-WLan verbunden ist, öffnen Sie einen neuen Tab im Safari-Webbrowser und öffnen Sie folgende Adresse [http://10.10.10.1](http://10.10.10.1)

![Cassy-WLan](https://diversewolken.ddns.net/nextcloud/index.php/s/zgynA6RKTTEaM4Y/download)<!-- style="max-width:80%; margin:5%"-->

---

<p class="bc">

__Notebook:__

- wechseln Sie auf dem Cassy zum Menu Einstellungen (oben rechts) 

- überprüfen Sie den Name des Cassy-Gerätes: z.B. MC2-010

- suchen Sie in den Laptop-WLan-Einstellungen nach dem Netzwerk, welches den selben Namen wie ihr Cassy-Gerät hat und verbinden Sie sich damit

- wenn ihr Laptop mit dem _Cassy_-WLan verbunden ist, öffnen Sie einen neuen Tab Webbrowser (z.B. Firefox) und öffnen Sie folgende Adresse [http://10.10.10.1](http://10.10.10.1)

![Cassy-WLan](https://diversewolken.ddns.net/nextcloud/index.php/s/zgynA6RKTTEaM4Y/download)<!-- style="max-width:80%; margin:5%"-->

</p>

</p>

---

- zu sehen ist die Live-Anzeige des Spannungssensors <br>-> aktivieren Sie am Cassy die Stromstärkemessung und deaktivieren Sie die Spannungsmessung <br> -> Überprüfen Sie die Veränderung auf Ihrem Cassy

![Cassy-WLan2](https://diversewolken.ddns.net/nextcloud/index.php/s/8ZjcN5DZqk6frXw/download)<!-- style="max-width:80%; margin:5%"-->

### Einstellen der Messparameter am Cassy

__Grundlage:__ Hier werden die Messparameter eingestellt

__Arbeitsablauf:__

- wechseln Sie auf der linken Seite zu Einstellungen

- hier müssen Sie den Messbereich für die Stromstärke einstellen __0,03 A__ und den Nullpunkt (des Diagramms) auf __links__ setzen(_Hinweis: diese Einstellung kann auch im Cassy direkt vorgenommen werden_)

![Cassy-Einstellungen](https://diversewolken.ddns.net/nextcloud/index.php/s/KQLjMB5CoYRR34o/download)<!-- style="max-width:80%; margin:5%"-->

- wechseln Sie auf der linken Seite zu ***Diagramm*** und vergleichen Sie Ihre Anzeige

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/9APdepf3in8wQ86/download)<!-- style="max-width:80%; margin:5%"-->

### Aufbau der Messchaltung

$ \red{\boxed{\mathrm{Es\ muss\ keine\ Gewalt\ angewendet\ werden.}}}$

__Grundlage:__ Für diesen Versuch ist der Schaltplan in den Vorbetrachtungen des Versuchs gezeichnet. 

__Materialien:__ Sie erhalten einen Kondensator mit der Kapazität $4700 \mu F$ und einen ohmschen Widerstand mit $1000 \Omega$.

---

<H4>Schaltung: </H4>

__Ladekreis:__

- die Pole der Spannungsquelle werden über den Wechselschalter direkt an den Kondensator angeschlossen

<p style="margin-left:5%">

$ \red{\boxed{\mathrm{ACHTUNG:\ + Platte\ des\ Kondensators\ mit\ \oplus der\ Spannungs-Quelle\ verbinden}}}$

<details>

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_1](https://diversewolken.ddns.net/nextcloud/index.php/s/SMpRaWdBfXBPDSW/download)<!-- style="max-width:80%; margin:5%"-->

</details>

</p>

---

Entladekreis:

- der Widerstand wird in Reihe zum Kondensator angeschlossen

- in Reihe zum Widerstand folgt das _Cassy_

- achten Sie beim Anschluss des _Cassy_, dass der blaue Anschluss in Richtung $\ominus$-Pol der Spannungsquelle und der schwarze Anschluss in Richtung des $\oplus$-Pols der Spannungsquelle zeigt

<details style="margin-left:5%">

<summary> Überprüfen Sie die Schaltung </summary>

![Schaltungsaufbau_2](https://diversewolken.ddns.net/nextcloud/index.php/s/m2KAErdZKRTMFi5/download)<!-- style="max-width:80%; margin:5%"-->

</details>

- lassen Sie sich die Schaltung von der Lehrkraft abnehmen

### Aufnahme der Entladekurve

$ \red{\boxed{\mathrm{Die Schaltung\ muss\ abgenommen\ worden\ sein.}}}$

__Grundlage:__ Hier wird der Kondensator zunächst geladen. Dann wird die automatische Messung mit dem _Cassy_ gestartet und die Entladekurve wird aufgezeichnet.

- legen Sie den Wechselschalter in die Ladeposition

- schalten Sie die Spannungsquelle ein und wählen eine Spannung von 10 V

- starten Sie anschließend die Messung auf dem _Cassy_ indem Sie oben auf __"Messzeit nicht vorgegeben"__ klicken, legen Sie anschließend den Schalter um

![Cassy-Diagramm_1](https://diversewolken.ddns.net/nextcloud/index.php/s/dDiiE3cYDgGqM3W/download)<!-- style="max-width:80%; margin:5%"-->

- stoppen Sie die Messung nach etwa $T=4\tau$ (4 charaktieristischen Zeiteinheiten)

- achten Sie darauf, dass die eigentliche Entladung erst beginnt, wenn Sie den Schalter umlegen


### Auswertung einer Messung

__Grundlage:__ Hier werden die Messdaten ausgewertet.

__Ermittlung der geflossenen Ladung:__

- wählen Sie unter Auswertungen (unterhalb des Diagramms) den Menupunkt _"Fläche zur x-Achse"_

- angezeigt wird die geflossene Ladung in der Einheit $A\cdot s = C$ 

- notieren Sie den Messwert

![Cassy_-_Auswertung_1](https://diversewolken.ddns.net/nextcloud/index.php/s/BXHx8eeCy8oXBSD/download)<!-- style="max-width:80%; margin:5%"-->

__Diagramm zeichnen aus einzelnen Messwerten:__

- wechseln Sie auf der linken Seit zum Reiter __Tabelle__

- notieren Sie in einer Messwerttabelle __t in s__ und __I in A__ und übernehmen Sie 10 charakteristische Messwerte

- zeichnen Sie anschließend den I(t)-Graph für Ihre Messwerte in das Protokoll


## 2.4 Schülerexperiment: Messungen der magnetischen Flussdichte

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
>      - wähle als Messbereich -10 - 10 mT

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
