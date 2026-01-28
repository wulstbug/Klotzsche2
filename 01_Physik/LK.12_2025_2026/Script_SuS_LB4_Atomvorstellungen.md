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

<p style='margin-left:10%'>

@rangeQuiz2( $\lambda_{lang}$, 4050e-9, $\text{m}$ )

@rangeQuiz2( $\lambda_{kurz}$, 95.0e-9, $\text{m}$ )

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

*   **Langwelligste Linie ($\lambda_{lang}$):** Entspricht dem geringsten Energieunterschied $\Delta E_{min}$ im Rückfall, d.h., dem Übergang $5 \to 4$.
*   **Kurzwellige Linie ($\lambda_{kurz}$):** Entspricht dem größten Energieunterschied $\Delta E_{max}$ im Rückfall, d.h., dem Übergang $5 \to 1$.
*   Nutzen Sie $E = \frac{h \cdot c}{\lambda}$.

</details>

<details style="margin-left:10%;color:blue">

<summary> Lösung </summary>

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

$$\mathbf{\lambda_{lang} \approx 4,05 \cdot 10^{-6}\,\text{m}}\,\textrm{(infrarot)}$$

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

<div class="flex-child-2" style="min-width: 300px; margin-bottom: -10px">

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

__Forderung:__  <br> <br>

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

$ a = n \cdot \dfrac{\lambda}{2} $ mit $\lambda = \dfrac{h}{p} $ (_de Broglie_) <br> <br>

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

_Hinweis:_ <br> <br>

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

Wir lassen für dieses Model auch $\lambda = \dfrac{a}{2}$ zu <br> <br>

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

__Einsetzen (de Broglie):__ <br> <br>

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

$ a = \dfrac{n \cdot h}{2 \cdot p} \rightarrow p^2 = \dfrac{n^2 \cdot h^2}{4\cdot a^2} $ (I) <br> <br>

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

__Energie-Impuls-Relation:__  <br> <br>

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

$ E = \dfrac{1}{2}\cdot m \cdot v^2 = \dfrac{p^2}{2m} \rightarrow p^2 = E \cdot 2\cdot m$ (II)  <br> <br>

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

__Gleichsetzen (I)=(II):__  <br> <br> <br>

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

$\dfrac{n^2 \cdot h^2}{4\cdot a^2} = E \cdot 2\cdot m$  <br> <br>

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 150px; margin-bottom: -10px">

__Quantisierte Energiezustände $E_n$:__

</div>

<div class="flex-child-2" style="min-width: 150px; margin-bottom: -10px">

$ \boxed{E_n = \dfrac{h^2}{8\cdot m\cdot a^2}\cdot n^2 }$

</div>

</section>




</div>

<div class="flex-child-1" style="min-width: 200px; margin-bottom: -10px">

![Potentialtopf](https://diversewolken.ddns.net/nextcloud/index.php/s/PcZ2GjQnrHyWpYs/download)

</div>

</section>

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


## 12. 6. Das Pauli-Prinzip

Das Pauli-Ausschlussprinzip (Wolfgang Pauli, 1925) ist ein fundamentales Konzept der Quantenphysik und besagt:

> Zwei Elektronen, Protonen, Neutronen (im allgemeinen Fermionen) können nicht gleichzeitig denselben quantenmechanischen Zustand (d.h. denselben Zustand mit identischen Quantnezahlen) einnehmen.

__Anders ausgedrückt:__ Damit sich auf einem Energieniveau zwei Elektronen befinden können müssen sie sich in einer anderen Quantenzahl (z.B. Nebenquantenzahl -> Orbitalform, Magnetquantenzahl -> Spin) unterscheiden.

__Orbitale beschreiben die Aufenthaltswahrscheinlichkeit der Elektronen:__

![Elektronen-Orbitale](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9b/AOs-3D-dots.png/960px-AOs-3D-dots.png)<!-- style="margin-left:5%;max-width:600px" -->

<details style='margin-left:10%'>

<summary> Einzelelektronenorbitale </summary>

![EInzelelektronenorbitale](https://diversewolken.ddns.net/nextcloud/index.php/s/f8RKwZRRXLaoQbe/download "Quelle: https://futurezone.at/science/grazer-physiker-messen-elektronen-orbitale-in-3d/156.749.407")

</details>

### Aufgabe Mehrelektronensystem -  Quantensprünge beim Helium-Ion ($He^+$)

![Helium+](https://diversewolken.ddns.net/nextcloud/index.php/s/btAyArjbMpwESFC/download)<!-- style="max-width:200px" --> Das Bohr’sche Atommodell lässt sich auf wasserstoffähnliche Ionen anwenden, indem die Kernladungszahl $Z$ berücksichtigt wird. Für die Energieniveaus gilt die Beziehung:

$E_n = R_y \cdot \frac{1}{n^2} \cdot Z^2$

     mit $R_y = -13,6\,\mathrm{eV}$ 
---

__Teilaufgabe: Berechnung der Emissionsfrequenz__

Ein Elektron eines $He^+$-Ions geht vom Energieniveau $E_4$ auf das Niveau $E_2$ über . Berechnen Sie die **Frequenz** $f$ des dabei emittierten Photons .

<p style='margin-left:10%'>

@rangeQuiz2( $f$ , 2.47e15, $\mathrm{Hz}$ )

</p>

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

1.  **Energieniveaus berechnen:** Nutzen Sie die Formel $E_n = -13,6 \, \text{eV} \cdot \frac{Z^2}{n^2}$ mit $Z=2$ .
    *   $E_4 = -13,6 \, \text{eV} \cdot \frac{4}{16} = -3,4 \, \text{eV}$
    *   $E_2 = -13,6 \, \text{eV} \cdot \frac{4}{4} = -13,6 \, \text{eV}$
2.  **Energiedifferenz bestimmen:** $\Delta E = E_4 - E_2$.
3.  **Frequenz berechnen:** Nutzen Sie den Zusammenhang $\Delta E = h \cdot f$, also $f = \frac{\Delta E}{h}$ .

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

Die Energiewerte für Helium ($Z=2$) betragen :
*   $E_4 \approx -5,45 \cdot 10^{-19} \, \text{J}$
*   $E_2 \approx -2,18 \cdot 10^{-18} \, \text{J}$

Die Energiedifferenz ergibt sich zu:
$\Delta E = E_4 - E_2 = 1,635 \cdot 10^{-18} \, \text{J}$

Daraus folgt für die Frequenz:
$f = \frac{\Delta E}{h} = \frac{1,635 \cdot 10^{-18} \, \text{J}}{6,626 \cdot 10^{-34} \, \text{Js}}$
$\mathbf{f \approx 2,47 \cdot 10^{15} \, Hz}$ [3]

</details>

---

__Teilaufgabe b) Berechnung der Ablöseenergie__

Das Elektron eines $He^+$-Ions befindet sich auf dem Energieniveau $E_2$. Geben Sie die Energie $E_{ab}$ an, die mindestens notwendig ist, um dieses Elektron abzulösen.

<p style='margin-left:10%'>

@rangeQuiz2( $E_{ab}$ , 2.18e-18, $\mathrm{J}$ )
</p>

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

Um ein Elektron „abzulösen“ (zu ionisieren), muss es von seinem aktuellen Energiezustand $E_n$ auf das Energieniveau $E_{\infty} = 0 \, \text{eV}$ (Ionisierungsgrenze) gehoben werden. Die dafür aufzubringende Energie entspricht dem Betrag der Bindungsenergie auf dem jeweiligen Niveau:
$\Delta E = E_{\infty} - E_n = |E_n|$

1.  **Berechnung des Energieniveaus:** Nutzen Sie die gegebene Formel für $n=2$ und $Z=2$. Beachten Sie, dass $R_y$ für den Grundzustand des Wasserstoffs ($n=1, Z=1$) etwa $13,6 \, \text{eV}$ bzw. $2,18 \cdot 10^{-18} \, \text{J}$ entspricht.
2.  **Umrechnung:** Stellen Sie sicher, dass das Ergebnis in der Einheit Joule ($\text{J}$) angegeben wird.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Gegeben: $n = 2$, $Z = 2$, $R_y \cdot h \approx 2,18 \cdot 10^{-18} \, \text{J}$

Die Energie auf dem Niveau $E_2$ berechnet sich wie folgt:
$E_2 = -2,18 \cdot 10^{-18} \, \text{J} \cdot \frac{2^2}{2^2} = -2,18 \cdot 10^{-18} \, \text{J}$

Da die Ablöseenergie die Differenz zur Ionisierungsgrenze ($0 \, \text{J}$) ist, gilt:
$E_{ab} = 0 \, \text{J} - (-2,18 \cdot 10^{-18} \, \text{J}) = \mathbf{2,18 \cdot 10^{-18} \, J}$

Die mindestens notwendige Energie zum Ablösen des Elektrons beträgt **$2,18 \cdot 10^{-18} \, \text{J}$** (was exakt $13,6 \, \text{eV}$ entspricht).

</details>


## 12. 7. Anregung von Atomen durch Elektronen und Photonen

> Führt man den Atom eines Gases Energie zu, so können sich die gebundenen Elektronen kurzzeitig in höhere Energieniveaus begeben. Der aufgenommene Energiebetrag muss dabei genau der Energiedifferenz $\Delta E$ zwischen Endniveau und Anfangsniveau entsprechen.

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Anregung durch beschleunigte Elektronen__

> Werden Elektronen beschleunigt ($E=U\cdot e$) so können diese bei einem elastischen Stoß mit einem Atom einen Teil ihrer Energie $E_{ab}$ an ein Elektron der Hülle abgeben. Dabei gilt:
>
> $$ \boxed{E_{ab} = \Delta E} $$

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Anregung durch Absorption von Photonen__

> Bestrahlt man ein Gas mit Photonen, so kann das Photon absorbiert werden und die Photonenenergie $E_{ph}$ wird auf ein Elektron der Hülle übertragen. Dabei gilt:
>
> $$\boxed{E_{ph} = \Delta E}$$

</div>

</section>

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Elektronenstoß](https://diversewolken.ddns.net/nextcloud/index.php/s/PJfWCXrBQq3SFrg/download)

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

![Photonenstoß](https://diversewolken.ddns.net/nextcloud/index.php/s/Xo6NiyFdojLzTy2/download)

</div>

</section>

### Abituraufgabe: Das Neon-Atom

Neon-Atome können durch Elektronenstöße angeregt werden. Dabei treten diskrete Energiezustände und charakteristische Emissionen auf.

---

__a) Energie eines Zwischenzustands__

Ein Neon-Atom (im Grundzustand) wechselwirkt mit einem freien Elektron und absorbiert dabei die Energie $E_{abs} = 18,6 \, \text{eV}$. Das angeregte Neon-Atom emittiert anschließend ein Photon (Quant) der Wellenlänge $\lambda = 640 \, \text{nm}$ (orangefarbenes Licht) und geht dabei in einen energetischen Zwischenzustand über.

Berechnen Sie die Energie $E_Z$ dieses Zwischenzustands bezüglich des Grundniveaus ($E_0 = 0 \, \text{eV}$).

<p style='margin-left:10%'>

@rangeQuiz2( $E_Z$ , 16.66, $\mathrm{eV}$ )

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

1. **Energie des emittierten Photons berechnen:** Nutzen Sie den Zusammenhang $E_{Ph} = \frac{h \cdot c}{\lambda}$. Mit der Näherung $h \cdot c \approx 1240 \, \text{eV} \cdot \text{nm}$ ergibt sich die Energie des Photons in Elektronenvolt.
2. **Energie des Zwischenzustands bestimmen:** Da das Atom von einem Niveau ($18,6 \, \text{eV}$) durch Abgabe eines Photons auf das Zwischenniveau $E_Z$ fällt, gilt: $E_Z = E_{abs} - E_{Ph}$.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Gegeben: $E_{abs} = 18,6 \, \text{eV}$, $\lambda = 640 \, \text{nm}$

$E_{Ph} = \frac{1240 \, \text{eV} \cdot \text{nm}}{640 \, \text{nm}} \approx 1,9375 \, \text{eV}$

$E_Z = 18,6 \, \text{eV} - 1,9375 \, \text{eV} = \mathbf{16,6625 \, eV}$

Der Zwischenzustand liegt energetisch etwa $16,66 \, \text{eV}$ über dem Grundniveau.

</details>

---

__b) Beobachtung leuchtender Bereiche__

Elektronen durchlaufen aus der Ruhe heraus eine Beschleunigungsspannung von $U = 22,6 \, \text{V}$ in einer mit Neongas gefüllten Röhre. Dabei werden in der Röhre zwei schmale, orangefarbig leuchtende Bereiche beobachtet.

Erklären Sie diese Beobachtung.

<details style="margin-left:10%;color:blue">

<summary>Lösungsweg</summary>

Betrachten Sie den Beschleunigungsvorgang der Elektronen. Diese nehmen kinetische Energie auf und geben sie bei Stößen mit Neon-Atomen ab, sobald sie die notwendige Anregungsenergie erreicht haben. Berücksichtigen Sie, dass die Elektronen nach einem unelastischen Stoß erneut beschleunigt werden können, sofern die Restspannung ausreicht.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

* **Erste Anregung:** Die Elektronen werden im elektrischen Feld beschleunigt. Sobald sie eine Energie von ca. $18,6 \, \text{eV}$ erreicht haben, regen sie bei einem Stoß ein Neon-Atom an. Beim Zurückfallen des Atoms in den Zwischenzustand wird orangefarbenes Licht emittiert (erster Leuchtbereich).
* **Zweite Anregung:** Nach dem Stoß haben die Elektronen fast ihre gesamte kinetische Energie verloren, werden aber durch die verbleibende Spannung erneut beschleunigt.
* **Zweiter Bereich:** Da die Gesamtspannung $22,6 \, \text{V}$ beträgt und für orangefarbenes Licht nur ca. $18,6 \, \text{eV}$ (Anregung) nötig sind, kann ein Elektron nach der ersten Anregung theoretisch erneut Energie aufnehmen. In der Praxis handelt es sich bei zwei getrennten Bereichen oft um die Visualisierung von Schichten, in denen die statistische Wahrscheinlichkeit für Anregungsstöße nach einer bestimmten Beschleunigungsstrecke maximal ist (ähnlich dem Franck-Hertz-Versuch).

</details>

---

__c) Entstehung von Laserstrahlung__

Ein Energieniveau des Neons ist metastabil und somit geeignet, um Laserlicht zu erzeugen.

Erläutern Sie das physikalische Prinzip der Entstehung von Laserstrahlung.

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

Ein Laser (Light Amplification by Stimulated Emission of Radiation) benötigt drei grundlegende Komponenten/Vorgänge: Besetzungsinversion, ein metastabiles Niveau und die stimulierte Emission.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

1. **Pumpen:** Durch Energiezufuhr (z. B. Elektronenstoß) werden Atome in einen angeregten Zustand versetzt.
2. **Metastabiler Zustand:** Die Atome verweilen in diesem Zustand länger als üblich (hohe Verweildauer) .
3. **Besetzungsinversion:** Es befinden sich mehr Atome im angeregten (metastabilen) Zustand als im energetisch tieferen Zustand.
4. **Stimulierte Emission:** Ein vorbeifliegendes Photon passender Energie löst bei einem angeregten Atom den Übergang in einen tieferen Zustand aus. Dabei wird ein zweites Photon emittiert, das in Frequenz, Phase, Richtung und Polarisation identisch mit dem ersten ist.
5. **Resonator:** Spiegel am Ende des Mediums reflektieren die Photonen, wodurch eine lawinenartige Verstärkung durch weitere stimulierte Emissionen erfolgt.

</details>


## 12. 8. Fluoreszenz und Phosphoreszenz

__Oberbegriff: Lumineszenz__ bezeichnet allgemein jede Lichtemission eines Stoffes, die nicht durch hohe Temperatur (also nicht durch Glühen) verursacht wird. Die Lichtabgabe entsteht durch elektronische Anregungs- und Relaxationsprozesse.

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Fluoreszenz__

**Definition:**  
Ein Stoff emittiert nach Anregung durch Licht @color(**sofort wieder Licht wieder**, red). <br> Die Lichtemission endet praktisch unmittelbar, sobald die Anregung abgeschaltet wird.



</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Phosphoreszenz__

**Definition:**  
Ein Stoff emittiert nach Anregung durch Licht zeitlich @color(**zeitlich verzögert**, red). Es erfolgt und auch nach dem Ende der Anregung noch anhält (Nachleuchten).


</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


**Physikalischer Ablauf:**

- Ein Photon regt ein Elektron vom **Grundzustand** in einen **angeregten Singulett-Zustand** an

- Das Elektron fällt innerhalb von etwa **10⁻⁹ bis 10⁻⁸ Sekunden** in den Grundzustand zurück.

- das angeregte Photon emittiert ein Elektron

_Hinweis: Ein Teil der emittierten Energie wird als Wärme abgegen. Daher besitzt das emittierte Licht eine geringere Energie als das anregende Licht._


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

**Physikalischer Ablauf:**

- Ein Elektron wird zunächst in einen angeregten **Singulett-Zustand** gehoben, wechselt aber in einen Triplett-Zustand

- Der Übergang zurück in den Grundzustand ist **quantemmechanisch verboten bzw. stark gehemmt**

- Die Rückkehr erfolgt langsam, wodurch die Lichtemission von **Sekunden bis Stunden** andauern kann.


</div>

</section>

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

**Beispiele:**

- Textmarker
- Schwarzlichteffekt von Leuchtstoffröhren
- Sicherheitsmerkmale auf Geldscheinen

</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


**Beispiele:**

- Nachleuchtende Notausgangsschilder

- Leuchtfarbe auf Uhren

- Dekorative Leuchtsterne

</div>

</section>

---

__Infografik:__

![Fluoreszenz_Phosphoreszenz](https://diversewolken.ddns.net/nextcloud/index.php/s/HWj7ATcTNNff2SY/download)

[Was-sind-Singlett-Triplett-Zustände-Frag-die-KI](http://10.102.1.3:3001/?q=Erl%C3%A4utere%20mir,%20was%20ein%20Signlett-%20und%20ein%20Triplettzustand%20ist.%20Der%20Kontext%20ist%20Fluoreszenz%20und%20Phosphoreszenz.%20Auf%20Grundlegendem%20Niveau)

### Aufgabe zu Fluoreszenz und Phosphoreszenz

Ein gewöhnlicher angeregter Zustand (Fluoreszenz) hat eine Lebensdauer von etwa $\Delta t=10^{−8}\mathrm{s}$. Ein metastabiler Zustand (Phosphoreszenz) kann dagegen viele Sekunden überdauern. <br>
Berechnen Sie die minimale Energieunschärfe $\Delta E$ (in eV) für einen Zustand mit einer Lebensdauer von $\Delta t=1,0\cdot10^{−8}\mathrm{s}$.

<p style='margin-left:10%'>

@rangeQuiz2( $\Delta E$ , 3.29e-8, $\mathrm{eV}$ )

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungsvorschlag </summary>

Setzen Sie die Heiißenberg'sche Unschärferelation als Gleichung an und ermitteln sie $\Delta E$.

$$ \Delta E \cdot \Delta t≥ \frac{h}{4\pi}$$

</details>

## 12. 9. LASER - Light emission by stimulated radiation

__Nutze Duden S. 488__

> Informiere dich über die Begriff __spontane und induzierte Emission__. Was ist ein metastabiler Zustand? Notiere dir Stichpunkte dazu.

__Nutze Duden S. 488 oder Metzler S. 442__

> Informiere dich über die grundlegende Funktionsweise eines Lasers. Notiere eine qualitative Übersicht über die beteiligten Energieniveaus. Notiere wichtige Eigenschaften des Laserlichts.
>
> Wiederhole die Begriffe kohärenz und lineare Polarisation.

### Erläuterung des LASER - Prinzips


Ein Energieniveau des Neons ist metastabil und somit geeignet, um Laserlicht zu erzeugen.

Erläutern Sie das physikalische Prinzip der Entstehung von Laserstrahlung.

<details style="margin-left:10%;color:blue">
<summary>Lösungsweg</summary>

Ein Laser (Light Amplification by Stimulated Emission of Radiation) benötigt drei grundlegende Komponenten/Vorgänge: Besetzungsinversion, ein metastabiles Niveau und die stimulierte Emission.

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

1. **Pumpen:** Durch Energiezufuhr (z. B. Elektronenstoß) werden Atome in einen angeregten Zustand versetzt.
2. **Metastabiler Zustand:** Die Atome verweilen in diesem Zustand länger als üblich (hohe Verweildauer) .
3. **Besetzungsinversion:** Es befinden sich mehr Atome im angeregten (metastabilen) Zustand als im energetisch tieferen Zustand.
4. **Stimulierte Emission:** Ein vorbeifliegendes Photon passender Energie löst bei einem angeregten Atom den Übergang in einen tieferen Zustand aus. Dabei wird ein zweites Photon emittiert, das in Frequenz, Phase, Richtung und Polarisation identisch mit dem ersten ist.
5. **Resonator:** Spiegel am Ende des Mediums reflektieren die Photonen, wodurch eine lawinenartige Verstärkung durch weitere stimulierte Emissionen erfolgt.

</details>


<details style='color:blue;margin-left:10%'>

<summary> __Besetzungsinversion:__ </summary>

Mehr Atome befinden sich im angeregten (metastabilen) Zustand als im Grundzustand. <br> Es erfolgt eine zufällige spontane Emission eines Photons. Dieses Photon sorgt für die induzierte (stimulierte) Emission weiterer Photonen, wenn es auf angeregte Atome im metastabilen Zustand trifft.

</details>


### Übungsaufgabe Franck-Hertz und LASER

1. Übungsaufgabe: Energieaustausch in der Atomhülle

<p style="margin-left:10%">

![ArgonEnergieen](https://diversewolken.ddns.net/nextcloud/index.php/s/K3WPC7xNNsfXGZZ/download)Angeregte Zustände von Argon-Ionen lassen sich zur Erzeugung von Laserlicht verwenden. Das Laserlicht entsteht beim Übergang der Argon-Ionen vom Zustand **4p** in den Zustand **4s**. Um das obere Laserniveau 4p zu erreichen, ist zusätzlich zur Ionisierung eine Anregung des Ions durch Elektronenstoß erforderlich .

</p>

---

1. 1. Anregung durch Elektronenstoß

<p style="margin-left:10%">

Ein Elektron der Geschwindigkeit $v = 4,2 \cdot 10^6 \text{ m/s}$ verliert bei der Ionisation von Argonatomen $30 \%$ seiner Geschwindigkeit. Untersuchen Sie durch Rechnung, ob dieses Elektron anschließend noch in der Lage ist, ein Argon-Ion in das obere Laserniveau 4p anzuregen (erforderliche Energie: $\Delta E = 20 \text{ eV}$) .

@rangeQuiz2($ E_{kin} $, 24.0,$ \mathrm{eV} $)

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

1. Berechnen Sie die Restgeschwindigkeit $v'$ des Elektrons nach dem Verlust von $30 \%$ ($v' = 0,7 \cdot v$) .
2. Berechnen Sie die kinetische Energie mit $E_{kin} = \frac{1}{2} \cdot m \cdot v'^2$ .
3. Nutzen Sie für die Masse des Elektrons $m \approx 9,11 \cdot 10^{-31} \text{ kg}$ und rechnen Sie das Ergebnis von Joule in Elektronenvolt um ($1 \text{ eV} \approx 1,60 \cdot 10^{-19} \text{ J}$) .

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

$v' = 0,7 \cdot v = 0,7 \cdot 4,2 \cdot 10^6 \text{ m/s} = 2,9 \cdot 10^6 \text{ m/s}$ .

$E_{kin} = \frac{1}{2} \cdot 9,11 \cdot 10^{-31} \text{ kg} \cdot (2,9 \cdot 10^6 \text{ m/s})^2 = 3,8 \cdot 10^{-18} \text{ J} \approx 24 \text{ eV}$ .

**Ergebnis:** Da die kinetische Energie mit $24 \text{ eV}$ größer als die benötigten $20 \text{ eV}$ ist, ist eine Anregung möglich .

</details>

---

1. 2. Wellenlänge des Laserlichts

<p style="margin-left:10%">

Berechnen Sie die Wellenlänge $\lambda$ des Laserlichts, das beim Übergang vom 4p-Zustand in den 4s-Zustand emittiert wird .

@rangeQuiz2($ \lambda $, 497.0, $\mathrm{nm} $)

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

1. Bestimmen Sie die Energiedifferenz $\Delta E = E_{4p} - E_{4s}$ .
2. Nutzen Sie die Formel $\Delta E = \frac{h \cdot c}{\lambda}$ und stellen Sie diese nach $\lambda$ um .
3. Konstanten: $h \approx 6,63 \cdot 10^{-34} \text{ Js}$; $c \approx 2,99 \cdot 10^8 \text{ m/s}$ .

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

$\Delta E = 36,0 \text{ eV} - 33,5 \text{ eV} = 2,5 \text{ eV}$ .

$\lambda = \frac{h \cdot c}{\Delta E} \Rightarrow \lambda = \frac{6,63 \cdot 10^{-34} \text{ Js} \cdot 2,99 \cdot 10^8 \text{ m/s}}{2,5 \text{ eV} \cdot 1,60 \cdot 10^{-19} \text{ As}} = 4,97 \cdot 10^{-7} \text{ m} = 497 \text{ nm}$ .

</details>

---

1. 3. Wirkungsgrad des Lasers

<p style="margin-left:10%">

Vom unteren Laserniveau 4s fallen die Argon-Ionen in kürzester Zeit in den Grundzustand $Ar^+$ zurück. Berechnen Sie den Wirkungsgrad $\eta$ für den Laserprozess (Verhältnis von Laserenergie zu Anregungsenergie). Die anfängliche Ionisierungsarbeit soll unberücksichtigt bleiben .

@rangeQuiz2($ \eta $, 12.5, $\mathrm{\%} $)

<details style="margin-left:10%;color:blue">
<summary>Lösungshinweis</summary>

Der Wirkungsgrad ergibt sich aus dem Verhältnis der genutzten Energie (emittiertes Laserphoton) zur aufgewendeten Anregungsenergie: $\eta = \frac{\Delta E_{Laser}}{\Delta E_{Anregung}}$ .

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

$\eta = \frac{2,5 \text{ eV}}{20 \text{ eV}} = 12,5 \%$ .

</details>

</p>

---

2. Abituraufgabe: Der Franck-Hertz-Versuch

<p style="margin-left:10%">

Im Jahr 1925 wurden die deutschen Physiker **James FRANCK** (1882 - 1964) und **Gustav HERTZ** (1887 - 1975) für ihre experimentellen Forschungen auf dem Gebiet der Atomphysik mit dem Nobelpreis ausgezeichnet .

</p>


---

2. 1. Versuchsaufbau und Durchführung

<p style="margin-left:10%">

Skizzieren Sie den Versuchsaufbau (inkl. Messgeräte) zum Elektronenstoß-Versuch im FRANCK-HERTZ-Rohr, beschriften Sie die wesentlichen Teile und beschreiben Sie knapp die Versuchsdurchführung.

</p>

<details style="margin-left:10%;color:blue">
<summary>Lösungshinweis</summary>

Der Aufbau besteht aus einer evakuierten Röhre mit Quecksilberdampf, einer Glühkathode, einem Gitter und einer Auffängerelektrode .

</details>

<details style="margin-left:10%;color:blue">
<summary>Lösung</summary>

**Versuchsaufbau:**
*   **Kathode:** Emittiert Elektronen durch thermische Emission (Glühwendel) .
*   **Gitter:** Zwischen Kathode und Gitter liegt die regelbare Beschleunigungsspannung $U$ .
*   **Auffänger:** Zwischen Gitter und Auffänger liegt eine Gegenspannung $U_{geg} \approx 1 \text{ V}$ .
*   **Messgeräte:** Voltmeter für $U$ und ein empfindlicher Strommesser (Pikoamperemeter) für den Auffängerstrom $I$ .

![Lsg_Aufbau](https://diversewolken.ddns.net/nextcloud/index.php/s/zQQQZ5bRndr2Y8Y/download)

**Versuchsdurchführung:**
Die Röhre wird im Ofen aufgeheizt, um den nötigen Dampfdruck zu erzeugen . Die Beschleunigungsspannung $U$ wird kontinuierlich von $0 \text{ V}$ bis ca. $30 \text{ V}$ gesteigert . Nur Elektronen, deren kinetische Energie groß genug ist, um das Gegenfeld zu überwinden ($E_{kin} > 1 \text{ eV}$), erreichen den Auffänger und tragen zum Strom $I$ bei .

</details>

---

2. 2. Das $U-I$-Diagramm


<p style="margin-left:10%">

Fertigen Sie eine Skizze des charakteristischen $U-I$-Diagramms an. Zeichnen Sie darin auch den ungefähren Verlauf der Kennlinie ein, die man erwarten würde, wenn zwischen Elektronen und Quecksilberatomen nur elastische Stöße auftreten könnten. Begründen Sie den unterschiedlichen Kurvenverlauf .


</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Betrachten Sie das periodische Abfallen des Stroms bei Erreichen der Anregungsenergie von Quecksilber ($4,9 \text{ eV}$) .

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

**Skizze:**
Die Kurve zeigt einen grundsätzlich steigenden Verlauf mit periodischen Minima bei $U_1 \approx 4,9 \text{ V}$, $U_2 \approx 9,8 \text{ V}$, $U_3 \approx 14,7 \text{ V}$ . Die theoretische Kurve für rein elastische Stöße wäre eine glatt ansteigende Kurve ohne Minima.

![](https://diversewolken.ddns.net/nextcloud/index.php/s/TQatCWceiADmczM/download)

**Begründung:**
*   **Elastische Stöße:** Aufgrund des hohen Massenunterschieds zwischen Elektron und Hg-Atom verlieren die Elektronen dabei kaum Energie und erreichen trotz Stößen den Auffänger .
*   **Inelastische Stöße:** Sobald Elektronen kurz vor dem Gitter eine Energie von $4,9 \text{ eV}$ erreichen, können sie ein Hg-Atom anregen . Sie geben dabei ihre kinetische Energie fast vollständig ab, können das Gegenfeld nicht mehr überwinden und der Strom $I$ fällt ab . Bei höheren Spannungen ist dieser Vorgang mehrfach möglich (Bereich IV) .

</details>


---

2. 3. Notwendigkeit der Heizung


<p style="margin-left:10%">

Bei Zimmertemperatur ist in der Röhre Quecksilber in flüssigem Zustand zu sehen. Erklären Sie kurz, warum zur Aufnahme der Messkurve die Röhre beheizt werden muss .

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Denken Sie an die Stoßwahrscheinlichkeit zwischen Elektronen und Atomen .

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Flüssiges Quecksilber besitzt bei Zimmertemperatur einen zu geringen Dampfdruck . Die Heizung ist notwendig, damit genügend Quecksilbergas vorhanden ist, sodass eine hohe Stoßwahrscheinlichkeit für die Elektronen mit den Gasatomen besteht . Zudem verhindert es mögliche Kurzschlüsse durch flüssiges Quecksilber zwischen den Elektroden .

</details>



---

2. 4. Wellenlängenberechnung


<p style="margin-left:10%">

Nach Anregung der Quecksilberatome auf ein Niveau von $4,9 \text{ eV}$ über dem Grundzustand geht die Mehrzahl direkt wieder in den Grundzustand über. Berechnen Sie die Wellenlänge der damit verbundenen Strahlung. Nennen Sie den dazugehörigen Wellenlängenbereich .

@rangeQuiz2( $\lambda$ , 253.0, $\mathrm{nm}$ )

[[ Terahertz | Infrarot | Sichtbar | (Ultraviolett) | Röntgen | Gammastrahlung ]]

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Nutzen Sie die Beziehung $\Delta E = h \cdot \frac{c}{\lambda}$ mit $\Delta E = 4,9 \text{ eV}$ .

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Gegeben: $\Delta E = 4,9 \text{ eV}$

$\lambda = \frac{h \cdot c}{\Delta E} = \frac{4,14 \cdot 10^{-15} \text{ eV s} \cdot 3,0 \cdot 10^8 \text{ m/s}}{4,9 \text{ eV}}$ 
$\lambda \approx 2,53 \cdot 10^{-7} \text{ m} = \mathbf{253 \text{ nm}}$ 

**Wellenlängenbereich:**
Die Wellenlänge von $253 \text{ nm}$ liegt im **ultravioletten Bereich** (UV-Licht) .

</details>


## 12. 10. Röntgen-Strahlung

> Röntgenstrahlung kann zur nichtinvasiven Diagnose von Knochfrakturen oder Fehlstellungen genutzt werden.

----

__Die Entstehung von Röntgenstrahlung__

---

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


[__Versuchsaufbau:__](https://www.leifiphysik.de/atomphysik/roentgen-strahlung/grundwissen/erzeugung-von-roentgen-strahlung)


![Röntgenröhre](https://diversewolken.ddns.net/nextcloud/index.php/s/yacB5mkMdHWHJQb/download)


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">

__Foto:__

![Foto](https://www.leifiphysik.de/sites/default/files/images/0b24932ebb31555c9eb7c5fdc10898c7/992Erzeugung_von_R%C3%96NTGEN-Strahlung_moderne_roehren.webp)


</div>

</section>

> Ein Metallblock (z.B. aus Wolfram) wird mit hochenergetischen Elektronen beschossen.

---

__Wechselwirkung der Elektronen mit der Anode:__

- In der Anode der Röntgenröhre werden die auftreffenden schnellen Elektronen stark abgebremst. Dabei entsteht die @color(Bremsstrahlung, red) -> @color(kontinuierliches Spektrum, red).

- Die Elektronen werden im Anodenmaterial je nach Abstand zu einem Kern unterschiedlich stark beschleunigt, entsprechend enthält das Spektrum der Bremsstrahlung alle Photonenenergien bis zum Höchstwert

- Schlagen die einfallenden Elektronen Hülleelektronen des Anodenmaterials aus ihren Energieniveaus, so werden @color(charakteristische Linien, blue) emittiert @color(diskretes Spektrum, blue) (Mindestbeschleunigungsspannung erforderlich)

---

[__Entstehung-Charakteristischer-Röntgenstrahlung:__](https://www.leifiphysik.de/atomphysik/roentgen-strahlung/grundwissen/charakteristische-strahlung)

<section class="flex-container">

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


![Spektrum](https://diversewolken.ddns.net/nextcloud/index.php/s/Pyyy4ZsB9MDes2s/download)


</div>

<div class="flex-child-1" style="min-width: 300px; margin-bottom: -10px">


_Hinweise:_ 

- Bezeichnung der charakteristischen Röntgenlinien: 

  - Großbuchstabe -> Schale auf die das Strahlung emittierende Elektron fällt
  - Griechische Buchstabe -> Abstand des beteiligten Energieniveaus ($\alpha=1$, $\beta=2$ ...)
  - $K_\alpha$: Elektron springt von der L-Schale ($\alpha$-> nächster Nachbar) auf die K-Schale



</div>

</section>

### Aufgaben zu Röntgenstrahlung

1. In der folgenden Tabelle sind charakteristische $K_\alpha$-Linien verschiedener Metalle dargestellt. Ermitteln Sie das Anodenmaterial des dargestellten charakteristischen Röntgenspektrums.

![Tablle_KAlpha](https://diversewolken.ddns.net/nextcloud/index.php/s/FWezyfiMqYRsNgb/download)

![RöntgenspektrumSpektrum](https://diversewolken.ddns.net/nextcloud/index.php/s/H3ANfieM5MM4WEE/download)

[[ Mo ]]

---

2. Ermitteln Sie die Beschleunigungsspannung für den roten Graphen.

<p style='margin-left:10%'>

@rangeQuiz2($U$,23e3,$\mathrm{V}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Um Photonen der unteren Grenze des Wellenlängenspektrums zu erzeugen, müssen die Elektronen ihre gesamte kinetische Energie abgeben.

</details>

---

3. Ermitteln Sie den Abstand der Energieniveaus M und L für das verwendete Kathodenmaterial.

<p style='margin-left:10%'>

@rangeQuiz2($\Delta E_{M-L}$,2465,$\mathrm{eV}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Überprüfen Sie die zu den gegebenen charakteristischen Röntgenlinien gehörenden Energieniveaus.

Überlegen Sie, wie Sie daraus die Energiedifferenz $\Delta E_{M-L}$ ermitteln können.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis 2 </summary>

Die $K_\alpha$-Linie resultiert aus dem Übergang L->K. Die $K_\beta$-Linie aus M->K. 

Die gesuchte Energiedifferenz entspricht der Differenz der beiden Photonenenergien.

</details>

---

4. [Abitur-BY-2019](https://www.leifiphysik.de/atomphysik/roentgen-strahlung/aufgabe/metallhydrid-speicher-abitur-2019-ph12-2-a2)


### Aufgaben zu Röntgenstrahlung

1. In der folgenden Tabelle sind charakteristische $K_\alpha$-Linien verschiedener Metalle dargestellt. Ermitteln Sie das Anodenmaterial des dargestellten charakteristischen Röntgenspektrums.

<p style='margin-left:10%;margin-right:10%'>

![Tablle_KAlpha](https://diversewolken.ddns.net/nextcloud/index.php/s/FWezyfiMqYRsNgb/download)

![RöntgenspektrumSpektrum](https://diversewolken.ddns.net/nextcloud/index.php/s/H3ANfieM5MM4WEE/download)

[[ Mo ]]

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Ermitteln Sie die Wellenlänge der $K_\alpha$-Linie. Vergleichen Sie diese Wellenlänge mit den Angaben in oberer Tabelle und schließen Sie auf das Anodenmaterial.

</details>

---

2. Ermitteln Sie die Beschleunigungsspannung für den roten Graphen.

<p style='margin-left:10%'>

@rangeQuiz2($U$,23e3,$\mathrm{V}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Um Photonen der unteren Grenze des Wellenlängenspektrums zu erzeugen, müssen die Elektronen ihre gesamte kinetische Energie abgeben.

</details>

---

3. Ermitteln Sie den Abstand der Energieniveaus M und L für das verwendete Kathodenmaterial.

<p style='margin-left:10%'>

@rangeQuiz2($\Delta E_{M-L}$,2465,$\mathrm{eV}$)

</p>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis </summary>

Überprüfen Sie die zu den gegebenen charakteristischen Röntgenlinien gehörenden Energieniveaus.

Überlegen Sie, wie Sie daraus die Energiedifferenz $\Delta E_{M-L}$ ermitteln können.

</details>

<details style='color:blue;margin-left:10%'>

<summary> Lösungshinweis 2 </summary>

Die $K_\alpha$-Linie resultiert aus dem Übergang L->K. Die $K_\beta$-Linie aus M->K. 

Die gesuchte Energiedifferenz entspricht der Differenz der beiden Photonenenergien.

</details>

---

4. Aufgabe: Physikalische Grundlagen der Röntgenstrahlung

     > In einer Röntgenröhre werden Elektronen aus einer Glühkathode emittiert und durch eine hohe Spannung $U$ in Richtung einer Anode beschleunigt. Beim Aufprall auf das Anodenmaterial entsteht Röntgenstrahlung, deren Spektrum aus einem kontinuierlichen Teil (Bremsstrahlung) und charakteristischen Linien besteht.

---

4. 1. Kurzwellige Grenzwellenlänge

     In einer spezifischen Versuchsanordnung werden die Elektronen mit einer Spannung von $U = 48 \text{ kV}$ beschleunigt. Ein Elektron überträgt beim Aufprall seine gesamte kinetische Energie auf ein einzelnes Photon.

     Berechnen Sie die minimale Wellenlänge $\lambda_{\min}$ (kurzwellige Grenze) der emittierten Bremsstrahlung.

<p style='margin-left:10%'>

@rangeQuiz2( $\lambda_{\min}$ , 25.8e-12, $\mathrm{m}$ )

</p>

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

1. **Energiebilanz aufstellen:** Die kinetische Energie des Elektrons $E_{kin} = e \cdot U$ entspricht der maximalen Energie des Photons $E_{Ph} = h \cdot f_{\max} = h \cdot \frac{c}{\lambda_{\min}}$ [8], [5].
2. **Formel umstellen:** $\lambda_{\min} = \frac{h \cdot c}{e \cdot U}$.
3. **Konstanten nutzen:** Verwenden Sie $h \approx 6,626 \cdot 10^{-34} \text{ Js}$, $c \approx 2,998 \cdot 10^8 \text{ m/s}$ und $e \approx 1,602 \cdot 10^{-19} \text{ C}$.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

$\lambda_{\min} = \frac{6,626 \cdot 10^{-34} \text{ Js} \cdot 2,998 \cdot 10^8 \text{ m/s}}{1,602 \cdot 10^{-19} \text{ C} \cdot 48000 \text{ V}}$

$\lambda_{\min} \approx 2,58 \cdot 10^{-11} \text{ m} = \mathbf{25,8 \text{ pm}}$

Die kurzwellige Grenze liegt bei ca. $25,8 \text{ Pikometern}$.

</details>

---

4. 2. Entstehung der Strahlung

     Erläutern Sie den physikalischen Prozess, der zur Entstehung des kontinuierlichen Röntgenspektrums führt.

<details style="margin-left:10%;color:blue">

<summary>Lösungshinweis</summary>

Betrachten Sie die Wechselwirkung der beschleunigten Elektronen mit den Atomkernen des Anodenmaterials. Denken Sie an den Begriff der "Abbremsung" geladener Teilchen.

</details>

<details style="margin-left:10%;color:blue">

<summary>Lösung</summary>

Das kontinuierliche Spektrum entsteht durch die **Abbremsung** der Elektronen im elektrischen Feld der Atomkerne der Anode. Dabei wird kinetische Energie in Strahlungsenergie (Photonen) umgewandelt. Da die Elektronen in unterschiedlichen Abständen an den Kernen vorbeifliegen, geben sie unterschiedlich große Energiebeträge ab, was zu einer kontinuierlichen Verteilung der Wellenlängen führt. Die Grenze $\lambda_{\min}$ wird erreicht, wenn ein Elektron seine gesamte Energie in einem einzigen Stoßprozess abgibt.

</details>

---

### IQB - Aufgabe Potentialtopf

<iframe src="https://diversewolken.ddns.net/nextcloud/index.php/s/9MGqQZjBXk6HDY2/download"
        width="100%" 
        height="600px">
</iframe>

<details style='color:blue'>

<summary> Erwartungsbild </summary>

<iframe src="https://diversewolken.ddns.net/nextcloud/index.php/s/nbAFWZNwTCjNN3w/download"
        width="100%" 
        height="600px">
</iframe>

</details>

### Abituraufgabe zu Röntgenstrahlung

5. [Abitur-BY-2019](https://www.leifiphysik.de/atomphysik/roentgen-strahlung/aufgabe/metallhydrid-speicher-abitur-2019-ph12-2-a2)