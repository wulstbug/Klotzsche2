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

# LB 12 Atomvorstellungen

![Atomvorstellungen](https://www.leifiphysik.de/sites/default/files/images/c199eb074d2c47f51b2e099b66b655ca/0entwicklung-der-atomvorstellung-aristoteles.webp)

## 12. 1. Geschichte der Atommodelle


## 12. 2. Entstehung von Spektrallinien




### Übung: Spektrallinien

> 1. In der folgenden Abbildung ist für die _subjektive Methode_ das Linienspektrum einer $He$-Gasentladung dargestellt. Ermitteln Sie für die rote und die orange Spektrallinie die Wellenlänge in der Einheit nm. Ermitteln Sie ebenfalls die Energie der zugehörigen Photonen in der Einheit eV. Notieren Sie Ihre Ergebnisse im Hefter.

<p style='margin-left:10%'>

_Hinweise: Für den folgenden Versuch wurde das Interferenzmuster durch ein Gitter mit 600 vertikalen Spalten pro mm aufgenommen. Der Abstand des Gitters vom Schirm beträgt 39 cm. Der Schirm beginnt im Abstand von 5cm von der Spektrallampe._

![Spektrallinien-He](https://diversewolken.ddns.net/nextcloud/index.php/s/Z4oJjK2DTzYfCbs/download)

</p>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Orange Linie:__

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_o$,573,$\mathrm{nm}$)

@rangeQuiz2($E_{ph-o}$,2.165,$\mathrm{eV}$)

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Rote Linie:__

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_r$,651,$\mathrm{nm}$)

@rangeQuiz2($E_{ph-r}$,1.906,$\mathrm{eV}$)

</p>

</div>

</section>

> 2. Vergleichen Sie die von Ihnen ermittelten Werte mit den in der Formelsammlung angegebenen Spektrallinien für Helium. __Notieren Sie die Tabellenwerte.__

---

> 3. In der folgenden Abbildung ist für die _subjektive Methode_ das Linienspektrum einer $H$-Gasentladung dargestellt. Da sich über die Zeit andere Gase im Glaskörper gesammelt haben, ist hier neben den beiden hauptsächlich sichtbaren Linien (rot, hellblau) ein quasi-kontinuierliches Spektrum sichtbar, welches für diese Auswertung nicht beachtet werden soll. <br> Ermitteln Sie die sichtbaren Spektrallinien von Wasserstoff. Notieren Sie Ihre Ergebnisse im Hefter in Tabellenform. Berechnen Sie die zugehörige Photonenenergie in eV.

<p style='margin-left:10%'>

__Sichtbare Spektrallinien des Wasserstoff__

![Spektrallinien-H](https://diversewolken.ddns.net/nextcloud/index.php/s/9Y6d7636gEFARiH/download)

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Experimentell:__ $\lambda$ in nm

@rangeQuiz2($\lambda_r$,644,$\mathrm{nm}$)

@rangeQuiz2($\lambda_b$,484,$\mathrm{nm}$)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Tabellenwert__ 

@rangeQuiz2($\lambda_r$,656,$\mathrm{nm}$)

@rangeQuiz2($\lambda_b$,486,$\mathrm{nm}$)

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Tabellenwert:__ $E_{ph}$ in eV 

@rangeQuiz2($E_{ph-r}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($E_{ph-b}$,2.553,$\mathrm{eV}$)

</div>

</section>


</p>

---


12. 3. Spektrallinien am Wasserstoffatom


### Überprüfung von Zwischenergebnissen aus der Herleitung

<p style="color:blue">

Löse die folgenden Aufgaben. Übernimm die Lösungen in deinen Hefter. Sie sind Teil der Herleitung.

</p>

1. Erster Bohr'scher Radius.

<p style='margin-left:10%'>

@rangeQuiz2($r_1$,0.529e-10,$\mathrm{m}$)

</p>

2. Ionisierungs-Energie von Wasserstoff (_Rydberg-Energie_).

<p style='margin-left:10%'>

@rangeQuiz2($R_y$,13.6,$\mathrm{eV}$)

</p>

3. Ermitteln Sie dazu zunächst näherungsweise die für Grenzen des sichtbaren Spektrums (400-800 nm) die Photonenenergie in der Einheit eV.

<p style='margin-left:10%'>

__Untere Grenze (eV):__

@rangeQuiz2($E_{ph-u}$, 1.55 ,$\mathrm{eV}$)

__Obere Grenze (eV):__

@rangeQuiz2($E_{ph-o}$, 3.1 ,$\mathrm{eV}$)

</p>

4. Überprüfen sie nun mit Hilfe der Rydberg-Ritz-Formel, welche Energieübergänge am Wasserstoff-Atom Photonen im Bereich des sichtbaren Lichts emittieren. <br> Hier dargestellt sind die Nummern der Übergangs-Energieniveaus _von->nach_

<p style="margin-left:10%">

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

_Lymnan-Serie_

- [[ ]] 2->1
- [[ ]] 3->1
- [[ ]] 4->1
- [[ ]] 5->1
- [[ ]] 6->1

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

_Balmer-Serie_

- [[x]] 3->2
- [[x]] 4->2
- [[x]] 5->2
- [[x]] 6->2
- [[ ]] 7->2

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

_Paschen-Serie_

- [[ ]] 4->3
- [[ ]] 5->3
- [[ ]] 6->3
- [[ ]] 7->3
- [[ ]] 8->3

</div>

</section>

</p>

5. Ermittle nun die Übergäng für die beiden beobachteten sichtbaren Spektrallinien des Wasserstoff-Spektrums. Diese gehören zur _Balmer-Serie_. <br> __Notiere die Ergebnisse in deinem Hefter und ergänze die fehlenden Übergänge $_{\square->\square}$__

<p style='margin-left:10%'>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

@color(__Rot:__, red) <br>

@rangeQuiz2($E_{\square->\square}$,1.89,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{\square->\square}$,655,$\mathrm{nm}$)


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


@color(__Blau:__, blue) <br>

@rangeQuiz2($E_{\square->\square}$,2.553,$\mathrm{eV}$)

@rangeQuiz2($\lambda_{\square->\square}$,486,$\mathrm{nm}$)


</div>

</section>

</p>


## 12. 4. Zusammenfassung: Energieniveaus am Wasserstoffatom

__Grundannahmen:__

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

1. Das Elektron bewegt sich auf einer kreisförmigen Bahn um den Kern. Auf dieser Bahn ist das Elektron eine __Stehende Welle__ mit dem Umfang @color(gleich einem ganzzahligen Vielfachen der Wellenlänge, red): <br> $$ u = n \cdot \lambda $$ <br> u .. Umfang der Kreisbahn mit dem Radius r <br> n .. Natürliche Zahl <br> $ \lambda $ .. de-Broglie Wellenlänge



</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

2. Auf der Kreisbahn gilt @color(Radialkraft = elektrische Kraft, red) <br> $$ F_r = F_{el} $$ <br> $F_r$ .. Radialkraft der Kreisbewegung <br> $F_{el}$ .. elektrische Anziehungskraft zwischen Kern und Elektron

</div>

</section>

---

__Ergebnis (Bahnradien):__

<section class="flex-container">

<div class="flex-child-3" style="min-width: 400px; margin-bottom: -10px">

3. Setzt man für die Wellenlänge die Formel der de-Broglie Wellenlänge ein und eliminiert in den beiden Gleichungen die Geschwindigkeit des Elektrons, so ergibt sich für den n-ten Radius der Elektronenbahn an einem Wasserstoff-Atom. <br> $$ r_n = \dfrac{h^2\cdot \varepsilon_0}{\pi\cdot m_e \cdot e^2} \cdot n^2$$ <br> @color(Die Zahl $n$ wird __Hauptquantenzahl__ des Elektronenniveaus genannt. Die Niveaus erhalten Großbuchstaben K L M usw., red).

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Energieniveaus_1](https://diversewolken.ddns.net/nextcloud/index.php/s/64ZHS9DQsBwXjWt/download)<!--style="max-width:200px" -->

</div>

</section>



---

__Schlussfolgerung:__

<section class="flex-container">

<div class="flex-child-3" style="min-width: 400px; margin-bottom: -10px">


4. Für die Elektronen sind nur __bestimmte__ Bahnradien zulässig. Für die zugehörigen Energieniveaus ($E_n$ der n-ten Elektronenbahn) ergibt sich die Rydberg-Formel <br> $$E_n = R_y \cdot \dfrac{1}{n^2} $$ <br> $R_y = -13,6 \, \mathrm{eV}$ .. Rydberg-Konstante <br> <br> __Hinweis:__ Da das Elektron __gebunden__ ist, ist seine Energie kleiner als Null. Man muss dem Elektron Energie hinzufügen, damit es ein freies Elektron wird.

</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Energieniveaus_Schema](https://diversewolken.ddns.net/nextcloud/index.php/s/EwLKnmbiDaxngZw/download)<!--style="max-width:200px" -->

</div>

</section>


---

__Elektronenübergänge:__

5. Wechselt ein Elektron von einer **Elektronen-Bahn $m$ auf die Bahn $n$** 

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px; margin:5%">

<section class="flex-container">

so wird __Energie in Form eines Photons__ abgegeben, wenn

<div class="flex-child-3" style="min-width: 200px; margin-bottom: -10px">

$$m > n$$ <br> und die Energie des emittierten Photons beträgt <br> $$ E_{ph} = E_m - E_n $$ <br> $$ E_{ph} = R_y \cdot \Big( \frac{1}{m^2} - \frac{1}{n^2} \Big) $$ <br> __Hinweis:__ Da $R_y=-13,6\,\mathrm{eV}$ ist die Photonenenergie positiv, wenn $m>n$.

</div>

<div class="flex-child-1" style="min-width: 100px; margin-bottom: -10px; margin-left:5%">

![Energieniveaus_3](https://diversewolken.ddns.net/nextcloud/index.php/s/2ddwzeY98TGL5YJ/download)<!--style="max-width:150px" -->

</div>

</section>


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px; margin:5%">

<section class="flex-container">

muss dem __Elektron Energie zugefügt werden__, wenn 

<div class="flex-child-3" style="min-width: 200px; margin-left:5%">

$$m < n$$ $$ E_{zu} = E_m - E_n $$ <br> $$ E_{zu} = R_y \cdot \Big( \frac{1}{m^2} - \frac{1}{n^2} \Big) $$ <br> <br> Die zugeführte Energie ist $E_{zu}<0$.

</div>

<div class="flex-child-1" style="min-width: 100px">

![Energieniveaus_2](https://diversewolken.ddns.net/nextcloud/index.php/s/SbxPBHqsgLacLSK/download)<!--style="max-width:150px" -->

</div>

</section>


</div>

</section>


### Übungsaufgabe - Anregung von Wasserstoff

__Physik der Atomhülle: Anregung von Wasserstoff durch Elektronenstoß__

Elektronen werden aus der Ruhe heraus durch die Spannung $U=13,2\,\text{V}$ beschleunigt und treffen dann auf ein Gas aus Wasserstoffatomen. Durch Elektronenstoß werden die Wasserstoffatome aus dem Grundzustand ($n=1$) heraus angeregt. Jedes Elektron kann dabei höchstens einmal anregen. Nachdem die Elektronen das Gas verlassen haben, wird ihre kinetische Energie gemessen.

**(Grundlagenwerte für die Lösung:** Maximale zur Verfügung stehende Energie: $E_{max} = 13,2\,\text{eV}$. Wasserstoff-Energieniveaus: $E_n = \frac{-13,6\,\text{eV}}{n^2}$. Die maximal erreichbare Hauptquantenzahl ist $n=5$, da die Energie zur Anregung auf $n=6$ ($E_6 - E_1 = 13,222\,\text{eV}$) die Eingangsenergie von $13,2\,\text{eV}$ übersteigt.)

---

__Teilaufgabe a)__

Zeichnen Sie das Energieniveauschema des H-Atoms.

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Zeichnen Sie die ersten fünf Energieniveaus ($n=1$ bis $n=5$) des Wasserstoffatoms mit den entsprechenden Energiewerten in eV, wobei $E_1 = -13,6\,\text{eV}$ ist. Beachten Sie, dass der Abstand der Niveaus mit steigendem $n$ abnimmt.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Das Schema muss folgende Niveaus enthalten (Beispiele):

*   $n=1: E_1 = -13,60\,\text{eV}$

*   $n=2: E_2 = -3,40\,\text{eV}$

*   $n=3: E_3 = -1,51\,\text{eV}$

*   $n=4: E_4 = -0,85\,\text{eV}$

*   $n=5: E_5 = -0,54\,\text{eV}$

*   $n=\infty: E_\infty = 0\,\text{eV}$

</details>

---

Teilaufgabe b)

Welche Werte stellt man bei der Messung der kinetischen Energie der Elektronen fest (Begründung!)?

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Die Elektronen können nur diskrete Energiemengen abgeben, die den Anregungsenergien $\Delta E = E_n - E_1$ entsprechen.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die anfängliche kinetische Energie der Elektronen beträgt $E_{kin, Anfang} = 13,2\,\text{eV}$. Die Elektronen verlassen das Gas mit der Restenergie $E_{Rest} = E_{kin, Anfang} - \Delta E_{Anregung}$.

Messbare Werte sind:

1.  **$13,2\,\text{eV}$:** Wenn die Elektronen die H-Atome nicht anregen (elastischer Stoß oder kein Stoß).

2.  **$E_{Rest, 2} = 13,2\,\text{eV} - (E_2 - E_1) \approx 13,2\,\text{eV} - 10,20\,\text{eV} = 3,00\,\text{eV}$**.

3.  **$E_{Rest, 3} = 13,2\,\text{eV} - (E_3 - E_1) \approx 13,2\,\text{eV} - 12,09\,\text{eV} = 1,11\,\text{eV}$**.

4.  **$E_{Rest, 4} = 13,2\,\text{eV} - (E_4 - E_1) \approx 13,2\,\text{eV} - 12,75\,\text{eV} = 0,45\,\text{eV}$**.

5.  **$E_{Rest, 5} = 13,2\,\text{eV} - (E_5 - E_1) \approx 13,2\,\text{eV} - 13,06\,\text{eV} = 0,14\,\text{eV}$**.

Die gemessenen Werte sind diskret und ergeben sich aus der Differenz der Anfangsenergie und der zur Anregung benötigten Energiemenge.

</details>

---

__Teilaufgabe c)__

Warum emittiert das beschossene Gas elektromagnetische Strahlung?

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Die angeregten Atome sind instabil und fallen in Zustände geringerer Energie zurück.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die durch den Elektronenstoß in höhere Energieniveaus angeregten Wasserstoffatome sind instabil. Sie fallen spontan in tiefere, energieärmere Zustände zurück (Emissionsprozess). Bei jedem Rückfall wird die Energiedifferenz $\Delta E$ in Form eines Photons emittiert: $\Delta E = h \cdot f$.

</details>

---

__Teilaufgabe d)__

Wie viele verschiedene Wellenlängen können nachgewiesen werden? Welche davon liegen im sichtbaren Bereich? Stellen Sie alle Übergänge im Energieniveauschema aus Teilaufgabe a dar!

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Die maximale Hauptquantenzahl ist $n_{max}=5$. Die Gesamtzahl der möglichen Übergänge von $n_{max}$ bis $n=1$ ist gegeben durch: $N = \sum_{k=1}^{n_{max}-1} k$.

Der sichtbare Bereich (Balmer-Serie) umfasst Übergänge, die auf das Niveau $n=2$ führen.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die maximale Anregung erfolgt bis zum Niveau $n_{max}=5$.

**Anzahl der Linien:**
Die Gesamtzahl der möglichen Emissionslinien ist die Summe aller möglichen Rückfälle:
$$ N = (5 \to 4) + (5 \to 3) + (5 \to 2) + (5 \to 1) $$
$$ + (4 \to 3) + (4 \to 2) + (4 \to 1) $$
$$ + (3 \to 2) + (3 \to 1) $$
$$ + (2 \to 1) $$
Insgesamt: $N = 4 + 3 + 2 + 1 = \mathbf{10}$ verschiedene Wellenlängen können maximal nachgewiesen werden.

**Sichtbarer Bereich (Balmer-Serie):**
Im sichtbaren Bereich liegen Übergänge, die auf das Niveau $n=2$ führen [3].
*   $5 \to 2$
*   $4 \to 2$ ($\text{H}\gamma$-Linie)
*   $3 \to 2$ ($\text{H}\beta$-Linie)
(Anmerkung: Die $\text{H}\alpha$-Linie ($3 \to 2$) und $\text{H}\beta$-Linie ($4 \to 2$) liegen im sichtbaren Bereich. Die $\text{H}\gamma$-Linie ($5 \to 2$) liegt im Violett/UV-Bereich, wird aber oft noch zum sichtbaren Bereich gezählt.)

</details>

---

__Teilaufgabe e)__

Berechnen Sie die Wellenlänge der lang- ($\lambda_{lang}$) und kurzwelligen ($\lambda_{kurz}$) Linie!

@rangeQuiz2( $\lambda_{lang}$, 4050e-9, $\text{m}$ )

@rangeQuiz2( $\lambda_{kurz}$, 95.0e-9, $\text{m}$ )

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

*   **Langwelligste Linie ($\lambda_{lang}$):** Entspricht dem geringsten Energieunterschied $\Delta E_{min}$ im Rückfall, d.h., dem Übergang $5 \to 4$.
*   **Kurzwellige Linie ($\lambda_{kurz}$):** Entspricht dem größten Energieunterschied $\Delta E_{max}$ im Rückfall, d.h., dem Übergang $5 \to 1$.
*   Nutzen Sie $E = \frac{h \cdot c}{\lambda}$.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

**I. Kurzwellige Linie (Größte Energie $\Delta E_{max}$):**
Dies ist der Rückfall vom höchsten erreichten Niveau ($n=5$) zum Grundzustand ($n=1$).
$$ \Delta E_{max} = E_5 - E_1 = (-0,544\,\text{eV}) - (-13,6\,\text{eV}) = 13,056\,\text{eV} $$
Umrechnung der Wellenlänge (unter Verwendung des Kurzwertes $h \cdot c \approx 1240\,\text{eV} \cdot \text{nm}$):
$$ \lambda_{kurz} = \frac{1240\,\text{eV} \cdot \text{nm}}{13,056\,\text{eV}} \approx 95,0\,\text{nm} $$
$$\mathbf{\lambda_{kurz} \approx 9,50 \cdot 10^{-8}\,\text{m}}$$

**II. Langwelligste Linie (Kleinste Energie $\Delta E_{min}$):**
Dies ist der Rückfall zwischen den beiden höchsten angeregten Niveaus: $n=5 \to n=4$.
$$ \Delta E_{min} = E_5 - E_4 = (-0,544\,\text{eV}) - (-0,85\,\text{eV}) = 0,306\,\text{eV} $$
Umrechnung der Wellenlänge:
$$ \lambda_{lang} = \frac{1240\,\text{eV} \cdot \text{nm}}{0,306\,\text{eV}} \approx 4052\,\text{nm} $$
$$\mathbf{\lambda_{lang} \approx 4,05 \cdot 10^{-6}\,\text{m}}$$ (Liegt im infraroten Bereich)

</details>

---

__Teilaufgabe f)__

Was beobachtet man, wenn man das Gas mit Photonen der Energie $13,2\,\text{eV}$ beschießt?

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Prüfen Sie, ob Photonen der Energie $13,2\,\text{eV}$ in der Lage sind, eine Anregung aus dem Grundzustand zu bewirken. Beachten Sie, dass Photonen ihre Energie nur vollständig abgeben können.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Die Photonen haben eine Energie von $13,2\,\text{eV}$.
Da Photonen ihre gesamte Energie in einem Stoß abgeben müssen, muss diese Energie exakt einer der diskreten Anregungsenergien $\Delta E = E_n - E_1$ entsprechen, oder die Ionisierungsenergie überschreiten.

*   Die höchste Anregungsenergie bis $n=5$ beträgt $13,06\,\text{eV}$.
*   Die Ionisierungsenergie beträgt $13,6\,\text{eV}$.

Da die $13,2\,\text{eV}$ Photonenenergie **keinem** der diskreten Übergänge von $n=1$ in einen höheren Zustand **exakt** entspricht und die Ionisierungsenergie unterschreitet, können die Photonen **keine** Energie an die H-Atome abgeben.

**Beobachtung:** Es würde **keine** zusätzliche elektromagnetische Strahlung emittiert und es würde **keine** messbare Schwächung der durchgelassenen Photonenstrahlung festgestellt. Das Gas erscheint "transparent" für diese Photonen.
</details>


## 12. 5. Modell eindimensionaler Potentialtopf

[Link zum Erklärvideo](https://youtu.be/pWYo7qxzTaM)

> Ein eindimensionaler Potentialtopf ist ein gutes Modellsystem, um die Quantisierung von Energiezuständen quantenmechanischer Teilchen zu untersuchen.
>
> Wir betrachten einen Potentialtopf der Breite $a$, in dem sich ein quantenmechanisches Teilchen (z.B. ein Elektron) aufhält. Außerhalb des Topf hat das Teilchen die Aufenthaltswahrscheinlichkeit 0.
>
> Wir fordern (wie beim Wasserstoff-Modell), dass das Teilchen stabil nur als stehende Welle im Potentialtopf existieren kann.
>
> Gesucht sind die möglichen Energiezustände $E_n$ für das Teilchen.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

__Forderung:__  <br> <br>

_Hinweis:_ <br> <br>

__Einsetzen (de Broglie):__ <br> <br>

__Energie-Impuls-Relation:__  <br> <br>

__Gleichsetzen (I)=(II):__  <br> <br> <br>

__Quantisierte Energiezustände $E_n$:__

</div>

<div class="flex-child-2" style="min-width: 200px; margin-bottom: -10px">

$ a = n \cdot \frac{\lambda}{2} $ mit $\lambda = \frac{h}{p} $ (_de Broglie_) <br> <br>

Wir lassen für dieses Model auch $\lambda = \frac{a}{2}$ zu <br> <br>

$ a = \frac{n \cdot h}{2 \cdot p} \rightarrow p^2 = \frac{n^2 \cdot h^2}{4\cdot a^2} $ (I) <br> <br>

$ E = \frac{1}{2}\cdot m \cdot v^2 = \frac{p^2}{2m} \rightarrow p^2 = E \cdot 2\cdot m$ (II)  <br> <br>

$\frac{n^2 \cdot h^2}{4\cdot a^2} = E \cdot 2\cdot m$  <br> <br>

$ \boxed{E_n = \frac{h^2}{8\cdot m\cdot a^2}\cdot n^2 }$

</div>

<div class="flex-child-2" style="min-width: 200px; margin-bottom: -10px">

![Potentialtopf](https://diversewolken.ddns.net/nextcloud/index.php/s/PcZ2GjQnrHyWpYs/download)

</div>

</section>

### Aufgaben zum Potentialtopf


### Aufgaben zum Potentialtopf

1. In einem eindimensionalen Potentialtopf der Breite $5\cdot10^{-10}\,\mathrm{m}$ befindet sich ein Elektron.

1. 1. Ermitteln Sie die Wellenlänge und die Energie des Zustandes mit der Quantenzahl $n=1$ in J und eV.

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_1$,1e-9,$\mathrm{m}$)

@rangeQuiz2($E_1$,2.41e-19,$\mathrm{J}$)

@rangeQuiz2($E_1$,1.504,$\mathrm{eV}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Nutze die Formel für den Potentialtopf. Die erste Wellenlänge entspricht $2a$.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$E_1 = \frac{h^2}{8\cdot m_e \cdot a^2} = 2,41\,\mathrm{J}$

</details>

---

1. 2. Ein Elektron sei auf dem Energieniveau mit der Quantenzahl $n=3$. Ermitteln sie die Wellenlängen der Photonen in Einheit nm, die es beim Übergang auf die Niveaus $n=1$ und $n=2$ aussenden würde. Entscheiden Sie jeweils, ob es sich um infrarotes, sichtbares oder ultraviolettes Licht handelt.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<p style='margin-left:10%'>

@rangeQuiz2($\lambda_{3->1}$,103e,$\mathrm{nm}$)

@rangeQuiz2($\lambda_{3->2}$,275,$\mathrm{nm}$)

</p>

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

<!-- data-solution-button="off" -->
- [[ infrarot | sichtbar | (ultraviolett) ]] $\lambda_{3->1}$
- [[ infrarot | sichtbar | (ultraviolett) ]]  $\lambda_{3->2}$


</div>

</section>


<details style='color:blue;margin-left:10%'>

<summary> Lösunghinweis </summary>

Das Energieniveau $E_3$ ist das neufache des Grundniveaus, $E_2$ ist das vierfache. Sichtbares Licht ist im Bereich ($1,5-3,1 \,\mathrm{eV}$ | $800-400 \,\mathrm{nm}$)

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösung </summary>

$E_3 = 3^2 \cdot E_1 = 2,17\cdot10^{-18}\,\mathrm{J}$

$E_2 = 2^2 \cdot E_1 = 9.64\cdot10^{-18}\,\mathrm{J}$

$\lambda_{3->1} = \frac{h\cdot c}{(E_3-E1)} = 1,03\cdot10^{-7}\,\mathrm{m} = 103\,\mathrm{m}$

$\lambda_{3->1} = \frac{h\cdot c}{(E_3-E2)} = 2,75\cdot10^{-7}\,\mathrm{m} = 275\,\mathrm{m}$

</details>