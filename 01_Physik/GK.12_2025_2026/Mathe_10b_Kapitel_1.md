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
}

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
}
@end

mode: Presentation

@onload
window.LIA.settings.font_size = 2
@end

-->

# Mathe Runde 10 

# 1. Wachstumsvorgänge und Zerfallsprozesse

{{1}}
********************************************
**Ziel**: Wir beschreiben einen Vorgang <span style="color:darkblue">***mit Worten***</span> bei dem sich eine Eigenschaft (d.h. eine Zahl ändert).

Beispiele:
********************************************

{{2-5}}
********************************************
Anzahl von Tieren (z.B. Hasen):

![Hasen](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/pZAF7cHJXw29ktS?file=/&fileId=103172&x=1920&y=1080&a=true&etag=e9bc3b99b3a2fdcd48d95aab5b0513eb)

********************************************
{{3-5}}
Weitere Beispiele für Wachstumsvorgänge:

{{4-5}}
********************************************
Bitte LB S. 50/51 aufschlagen

![weitere Beispiele](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/2CAwForfryw9CXf?file=/&fileId=103214&x=1920&y=1200&a=true&etag=590dfa04136a199804d84613eac62562)

********************************************

{{5}}
- Anzahl von Tieren in einer Population. 
- Anzahl der Bakterien in einer Nährlösung
- Anzahl der zefallenen radioaktiven Atome in einem Brennstab

{{6}}
********************************************
Aus Beschreibung entwickeln wir eine Menge von Datenpunkten, z.B. als Tabellendarstellung

Vereinfachtes Beispiel der Bakterienvermehrung:

_jedes Bakterium vermehrt sich pro Generationsschritt ***genau ein mal***, keine Zelle stirbt_

********************************************

{{7-8}}
********************************************
| Generation   | Anzahl     |
| :---------:   | :---------: |
| 1            | 1          |
| 2            | 2          |
********************************************


{{8}}
********************************************
| Generationsschritt   | Anzahl     |
| :---------:   | :---------: |
| 1            | 1          |
| 2            | 2          |
| 3            | 4          |
| 4            | 8          |
| 5            | 16          |
| 6            | 32          |
| 7            | 64          |


********************************************

{{9}}
Wir beobachten hier ein <span style="color:red">***exponentielles Wachstum***</span>.

{{10}}
********************************************
<span style="color:darkblue">
__LB. S 52:__ Untersuche den Forschungsauftrag 2 in Gruppenarbeit (2 Personen) 

1. Notiere den Sachverhalt
2. Erstelle Datenpunkte
3. Stelle deine Ergebnisse graphisch dar
4. Stelle eine Vermutung über die Art des Wachstumsprozesses auf.
</span>
********************************************

## Lösungen zu LB S.52

<H3>Durchmesser des Ölteppichs</H3>

Die ***beobachtete Größe*** ist hier der Durchmesser des Ölteppichs.

{{1-2}}
********************************************
| Anzahl der Tage   | Durchmesser in m   | Zuwachs pro Tag in m|
| :---------        | :---------         | :---------         |
| 0           | 8               | -           |
| 1           | 10               | -           |
| 2           | 12               | -           |
| 3           | 14               | -           |
| 4           | 16               | -           |
| 5           | 18               | -           |
********************************************

{{2}}
********************************************
| Anzahl der Tage   | Durchmesser in m   | Zuwachs pro Tag in m|
| :---------        | :---------         | :---------         |
| 0           | 8               | 2           |
| 1           | 10               | 2           |
| 2           | 12               | 2           |
| 3           | 14               | 2           |
| 4           | 16               | 2           |
| 5           | 18               | 2           |
********************************************

{{3}}
![Loesungen LB S.52 Forschungsauftrag 2 Diagramm](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/XpJzFSF9K3b6nSr?file=/&fileId=104875&x=1920&y=1200&a=true&etag=f2060e5f84359e2c3a2093dcc77be8d7)

{{4}}
Der Zuwachs, beschreibt die Änderung der beobachteten Größe. Bei einem <span style="color:red">***linearen Wachstum***</span> wird der Zuwachs <span style="color:red">***Wachstumsrate***</span> genannt und  diese ist <span style="color:red">***konstant***</span>.

$$ \hspace{2cm} $$

{{5}}
*******************************************
<H3>Flächinhalt A des Ölteppichs</H3>


Formel für Flächeninhalt A eines Kreises mit dem Durchmesser d lautet  

$$ \hspace{2cm} $$

*******************************************

{{6}}
$$ A = \frac{\pi}{4}\cdot d^2 $$  

{{7-8}}
********************************
| Anzahl der Tage t  | Fläche A in m²   | - |
| :--------- | :--------- | :--------- |
| 0     | 50.3     | -     |
| 1     | 78.5     | -     |
| 2     | 113.1     | -     |
| 3     | 153.9     | -     |
| 4     | 201.1     | -     |
| 5     | 254.5     | -     |
*******************************

{{8}}
*******************************
| Anzahl der Tage t  | Fläche A in m²   | Zuwachs   |
| :--------- | :--------- | :--------- |
| 0     | 50.3      | -        |
| 1     | 78.5      | 28.2     |
| 2     | 113.1     | 34.6     |
| 3     | 153.9     | 40.8     |
| 4     | 201.1     | 47.2     |
| 5     | 254.5     | 53.4     |
*******************************

{{9}}
![Loesungen LB S.52 Forschungsauftrag 2 Daten2](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/2XrsfDiH6JwXNxq?file=/&fileId=104879&x=1920&y=1200&a=true&etag=8e3304799d8471ce4eb922e04421555a)

{{10}}
**********************************
Wir beobachten hier ein <span style="color:red">***quadratisches Wachstum***</span>. 

Die explizite Berechnungsvorschrift ist eine quadratische Funktion:

$$ A(t) = \pi \cdot (4 + t)^2 $$
$$ A(t) = \pi\cdot t^2 + 8 \cdot \pi \cdot t + 16\cdot \pi $$

Der Zuwachs ist <span style="color:red">***nicht konstant***</span>.
**********************************

## zurück zum Beispiel Bakterien

![Bakterien](http://yesofcorsa.com/wp-content/uploads/2020/02/Bacteria-In-A-Petri-Dish-Wallpaper-Download-1024x682.jpg)

{{1}}
********************************************
<span style="color:red;font-size:25px">
<!--
    data-title="Wachstum Bakterien"
    data-xlabel="G-Schritt n"
    data-ylabel="Anzahl B"
-->
| Generationsschritt n  | Anzahl B    | Zuwachs |
| :---------:   | :---------: |  :---------:  |
| 0            | 1          |   0   |
| 1            | 2          |   1   |
| 2            | 4          |   2   |
| 3            | 8          |   4   |
| 4            | 16          |  8   |
| 5            | 32          |  16  |
| 6            | 64          |  32  |
</span>
********************************************


{{2}}
Auch bei einem exponentiellen Wachstum ist der Zuwachs <span style="color:red">***nicht konstant***</span>.

{{3}}
<H4>Explizite Berechnungsvorschrift</H4>

{{4}}
$$ B(n) = 2^n $$

## Arten von Wachstum

Wir definieren: 

- Die Zeiteinheiten, in denen wir ein Wachstum beobachten bezeichnen wir allgmein mit __n__. 

    _Hinweis: z.B. Anzahl an Tagen oder Generationsschritte_

- Der Wert der beobachteten Größe B nach n Zeitschritten wird mit $$ B(n) $$ bezeichnet.

    _Hinweis: z.B. Durchmesser des Ölflecks oder die Anzahl an Bakterien_

{{1}}
****************************************
<H4>Lineares Wachstum</H4>

- Die Differenz $$ d = B(n) - B(n-1) $$ beschreibt den Zuwachs im n-ten Zeitschritt und wird <span style="color:red">***Wachstumsrate***</span> genannt.

    <span style="color:red">***Bei einem ***linearen Wachstum*** ist die Wachstumsrate d konstant.***</span>

    Die explizite Berechnung lautet $$ B(n) = n \cdot d + B(0) $$

    _Hinweis: Ölfleck -> B(n) = 2n + 8_ 
****************************************

{{2}}
****************************************
<H4>Exponentielles Wachstum</H4>

    Bei einem exponentiellen Wachstum ist der Quotient $$ q = \frac{B(n)}{B(n-1)} $$ konstant. Der Quotient q wird <span style="color:red">***Wachstumsfaktor***</span> genannt.

    Die explizite Berechnung lautet $$ B(n) = B(0) \cdot q^n $$. 

    _Hinweis: Bakterienanzahl -> $B(n) = 1 \cdot 2^n$ _
****************************************

$$ .. $$

{{3}}
<H3 style="color:blue">LB S. 56 Aufgabe 1</H3>

{{4}}
![LB51_A1](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/n3wywxxgY5E2wa2?file=/&fileId=105205&x=1920&y=1200&a=true&etag=8eb050b23e6b6725b6c5cd83d7dde3e4)

## Rekursive Darstellung (Erklärung)

{{0-25}}
<H4> ...bisher hatten wir <span style="color:red">***explizite***</span> Berechungsvorschriften für B(n)</H4>

{{1-25}}
Diese Vorschrift heißt <span style="color:red">***explizite Vorschrift***</span>, weil man für B(n) für ein beliebiges n <span style="color:red">direkt</span> berechnen kann.

{{2-25}}
| <H4>Lineares Wachstum</H4> | <H4>Exponentielle Wachstum</H4> |
| :---------    | :--------- |
| {3-25}{Die <span style="color:red">***explizite Berechnung***</span> für ein ***lineares Wachstum*** lautet $$ B(n) = n \cdot d + B(0) $$ <br> __(Beispiel Ölfleck)__  }  |  {4-25}{Die <span style="color:red">***explizite Berechnung***</span> für ein ***exponentielle Wachstum*** lautet $$ B(n) = B(0) \cdot q^n \hspace{2cm} \textbf{mit} \hspace{0.5cm} q = \frac{B(n)}{B(n-1)} $$ <br> __(Beispiel Bakterien)__ } |


{{5}}
****************************
Die <span style="color:orange">***rekursive Darstellung***</span> eines Wachstumsprozesses beruht darauf, dass man die beobachtete Größe B(n) immer aus deren vorherigem Wert B(n-1) bestimmt.
****************************

{{6-23}} 
************************
<H5> Neues Beispiel: Gnupopulation </H5>

    ![Gnupopulation](Wachstum_03_04_Rekusiv/img/gnus.jpg)<!--onerror="this.src='https://upload.wikimedia.org/wikipedia/commons/thumb/6/66/Blue_wildebeest_at_Etosha_National_Park.jpg/1920px-Blue_wildebeest_at_Etosha_National_Park.jpg'"-->

<H5> Anfangspopulation: B(0) = 30000 </H5>

************************

{{7-23}} 
| 1. Prognose   | {8}{2.Prognose}  |
| :---------    | :--------- |
| Nach jedem Zeitschritt n, kommen 3000 neue Gnus dazu.    | {8}{Nach jedem Zeitschritt kommen 10% neue Gnus dazu.} |

{{9-23}}
| n          |  $B_1(n)$      | $B_2(n)$ |
| :---------    | :--------- | :-------------- |
| 0     | 30000           | 30000 |
| 1     | {10}{33000}     | {12-13}{30.000 ∙ 1,1} {13}{33000} |
| 2     | {11}{36000}     | {14-15}{33.000 ∙ 1,1} {15}{36300}    |
| 3     | {11}{39000}     | {16}{39930}     |
| 4     | {11}{42000}     | {16}{43923}     |

{{17-24}}
***********************
<H4>Rekursive Darstellung der Gnupopulation</H4>

| 1. Prognose                | 2.Prognose                   |
| $B_1(n)$ = {18}{$B_1(n-1)+3000$}   | $B_2(n)$ = {19}{$B_2(n-1) ∙ 1,1$}    |
| {20}{lineares Wachstum}    | {21}{exponentielles Wachstum}|
| {22}{$B(n) = B(n-1) + d$}    | {23}{$B(n) = B(n-1) ∙ q$}      |

***********************

{{24}}
| <H4>Lineares Wachstum</H4>    | <H4>exponentielles Wachstum</H4>|
| :---------    | :--------- |
| $B(n) = B(n-1) + d$           | $B(n) = B(n-1) ∙ q $    |

{{25}}bitte notieren

## Rekursive Darstellung (Tafelbild)

Die <span style="color:orange">***rekursive Darstellung***</span> eines Wachstumsprozesses beruht darauf, dass man die beobachtete Größe B(n) immer aus deren vorherigem Wert B(n-1) bestimmt.


| <H4>Lineares Wachstum</H4>    | <H4>exponentielles Wachstum</H4>|
| :---------    | :--------- |
| $B(n) = B(n-1) + d$           | $B(n) = B(n-1) ∙ q $      |
| d .. Wachstumsrate            | q .. Wachstumsfaktor      |

{{1}}
<H2><span style="color:blue">***Wähle 4 Aufgaben aus: LB S.56 A 2/4a+b/6/7/10/11/12 und löse sie.***</span></H2>

{{2}}
<H2><span style="color:orange">***Lösungen können eingesehen werden.***</span></H2>

## Lösungen LB S.56

<H2><span style="color:blue">***Wähle 4 Aufgaben aus: LB S.56 A 2/4a+b/6/7/10/11/12 und löse sie.***</span></H2>

| 2: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/Xgn6Ki8gH7Sxm3r)   | 4: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/nTk6ZSem4ftEsXn) | 6: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/5zcfe4tjpwr9kQ7)  |
| 10: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/5SNmKQXkHYCnJXf)     | 11: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/qT7kpixHfYyMk9s)    | 12: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/bGnejwKEX5AW3ow)     |

## Aufgabe zum Wachstum

Milou hat auf seinem Sparkonto einen Betrag von 1500€. Seine Eltern überweisen ihm monatlich einen Betrag von 500€ zu seiner Verfügung. Milou muss von diesem Geld alle Einkäufe selbst erledigen. 

Er gibt jeden Monat 20% des Geldes, das nach der Überweisung seiner Eltern auf seinem Konto ist, für sein Leben aus.

1. Nenne die Größe B(n) welche in dieser Aufgabe beobachtet wird. Notiere B(0).

   {1}{<span style="color:orange">***  Vermögen / Kontostand , B(0) = 1500€.***</span>}

2. Entscheide, ob sich der Geldbetrag auf Milou's Konto vergrößert oder verkleinert. Begründe deine Antwort kurz.

   {2}{<span style="color:orange">***Sein Vermögen wächst. Nach der Überweisung hat er 2000€. Davon gibt er 400€ aus, d.h. B(1) = 1600€. B(2) = 1680€ ...***</span>}

3. Erstelle eine Tabelle mit n , B(n)  für 6 Monate.

   {{3}}
   **************************
   <span style="color:orange">
   <!--data-title="Kontostand"		data-xlabel="Monate n" 	data-ylabel="Kontostand in €"-->
   | n | B(n) |
   |---|------|
   | 0 | 1500 |
   | 1 | 1600 |
   | 2 | 1680 |
   | 3 | 1744 |
   | 4 | 1795.2 |
   | 5 | 1836.16 |
   | 6 | 1868.928 |
   </span>
   **************************

4. Entscheide, ob es sich bei der Beobachtung um ein lineares Wachstum, ein exponentielles Wachstum oder keins von beidem handelt. Begründe deine Antwort kurz.

   {{4}}
   ***********************
   <span style="color:orange">
   Hier liegt weder ein lineares noch ein exponentielles Wachstum vor. 
   <br> <br>
   Test lineares Wachstum: Der Zuwachs (Wachstumsrate d=B(n)-B(n-1)) ist nicht konstant: 1600€-1500€=**100€**, 1680€-1600€=**80€**, ..**64€**...
   <br> <br>
   Test exponentielles Wachstum: Der Wachstumsfaktor $q = \frac{B(n)}{B(n-1)}$ ist nicht konstant: $\frac{1600}{1500}=1,0\bar{6}$ , $\frac{1680}{1600}=1,05 $, $\frac{1744}{1680}=1,04 $  
   </span> <br>
   ***********************

5. Notiere eine explizite oder eine Rekursive Berechnungsformel für B(n). 

   *Hinweis: Falls dir diese Aufgabe schwer fällt, erstelle eine Formel für B(1) und dann eine Formel für B(2). Vielleicht kannst du jetzt B(n) allgemein ausdrücken.*

   {{5}}
   ********************************
   <span style="color:orange">
   $$ B(n) = \big( B(n-1) + 500 \big) \cdot 0,8 $$
   </span> <br>
   ********************************

6. Ermittle den Prozentsatz (nach der Überweisung), den er ausgeben dürfte, damit sein Vermögen konstant bleibt.

   {{6}}
   ********************************
   <span style="color:orange">
   Wenn das Vermögen konstant bleiben sollte, dann muss folgende Gleichung gelten: <br>

   $$ 1500 = ( 1500 + 500) \cdot x $$

   damit ist $$ x = \frac{1500}{2000} = 0,75 \,(75\%) $$
   </span> <br>
   ********************************

7.  Stelle eine Vermutung darüber an, ob sich das Vermögen von Milou 

   a) stetig verkleinert 

   b) beliebig anwächst 

   c) ob es eine Grenze erreicht. 

   Begründe deine Vermutung.

   {{7}}
   ***************************
   <span style="color:orange">
   c) ist die richtige Antwort. Berechnet man das Wachstum weiter, so scheint sich der Kontostand 2000€ anzunähern. Man kann diese Vermutung untermauern: <br> <br>

   a) Hätte Milou zu Beginn 2000€, so würde sein Kontostand konstant bleiben, weil 

   $ B(1) = (2000€+500€) \cdot 0,8 = 2000€ $. <br> <br>

   b) Milou hat weniger als 2000€ und der Kontostand wächst, aber der Zuwachs wird immer kleiner. <br> <br>

   c) Hätte Milou mehr als 2000€ würde der Kontostand langsam sinken.

   z.B. mit $ B(0) = 2100€: \hspace{1cm} B(1) = (2100€+500€)*0,8 = 2080€ $  
   </span> <br> <br>
   ***************************

{{8}}
> Merke: Hat die Wachstumsfolge eine obere Grenze, welche B(n) selbst für beliebig große Werte n nicht überschreitet, so nennt man das Wachstum <span style="color:red">***begrenztes Wachtstum***</span>, im Gegensatz zum <span style="color:red">***unbegrenzten Wachstum***</span> (linear, exponentiell)

## Vorteile der expliziten bzw. rekursiven Darstellung

| explizite Darstellung | rekursive Darstellung |
| :--------: | :-----: | 
| Bsp.: $ B(n)=B(0)\cdot q^n $ | Bsp.: $B(n) = (B(n-1)+c)\cdot q $ |
| Nur ein Wert B(n) und q (oder d) muss bekannt sein, um einen beliebigen Wert zu berechnen. | Komplizierte Vorgänge lassen sich mathematisch darstellen. |

## Eigenschaften der Exponentialfunktion

Allgemeine Form: 

> $$ f(x) = c \cdot a^x $$ mit <br> __a .. Wachstumsfaktor__ (bisher q) <br> __c .. Anfangswert (Wert an Stelle x=0)__

<span style="color:red">_Aufgabe:_ Untersuche mit folgender Applikation den Einfluss der Parameter c und a auf die Exponentialfunktion. Notiere dir Ergebnisse aus deiner Beobachtung.</span>

| | |
| <iframe src="https://www.geogebra.org/classic/euthm47e?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe> | [qr-code](https://www.geogebra.org/classic/euthm47e) |

__Einfluss des Wachstumsfaktors a:__

   Wenn a>1, so ist die Funktion {0-1}{_monoton steigend/monoton fallend/konstant_} {1}{<span style="color:orange">monoton steigend</span>}

   Wenn a=1, so ist die Funktion .. {2}{<span style="color:orange">konstant gleich c</span>}

   Wenn 0<a<1, so ist die Funktion .. {3}{<span style="color:orange">monoton fallend</span>}

   Spiegelt man die Funktion $f(x) = a^x$ an der y-Achse so erhält man die Funktion {0-3}{$f(x) = $}{4}{<span style="color:orange">$ f(x) = (\frac{1}{a})^x $</span>}

   Ist a>0, so hat die Funktion {0-5}{_keine / genau eine / unendlich viele_ Nullstellen.}{5}{<span style="color:orange">_keine Nullstellen_, der Wertebereich sind die positiven reelen Zahlen.</span>}

{{6}}
********************
__Einfluss des Anfangswertes c (wir betrachten nur c>0):__

    Die Exponentialfunktion schneidet die y-Achse im Punkt ( <span style="color:orange">{7}{0} \| {7}{c}</span> ).

    {8}{Der Parameter c wirkt als <span style="color:orange">***Streckungsfaktor***</span> der Exponentialfunktion entlang der y-Achse.}

********************

## Aufgaben zur Exponentialfunktion LB S.61

<span style="color:blue"><H3>Wir lösen gemeinsam: LB S. 60  1 a,b,c</H3></span>

<span style="color:orange">
   {1}{a) $ a=3,\ monoton\ steigend\hspace{1cm} $ <br> }
   {2}{b) $ a=0,25,\ monoton\ fallend \hspace{1cm} $ <br> }
   {3}{c) $ a=\sqrt{6},\ monoton\ steigend $ }
</span>

<span style="color:blue"><H3>Löse allein die Aufgaben LB S. 61 2 a/d/g,3, 5 und 6.</H3></span>

{{4}}
***************************
| Lösungen | |
| 2: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/JqTFF53bM8TbD3E?file=/&fileId=113875&x=1680&y=1050&a=true&etag=0feb710847735480d35a9e2283a49ee3) | 3: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/kHAg4qrHwqPEZYA?file=/&fileId=113876&x=1680&y=1050&a=true&etag=783f0a1c9fbdbb3f2a906dd9dfcc1d2f) |
| 5: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/EqbeEkAHkAP7Qtm?file=/&fileId=113877&x=1680&y=1050&a=true&etag=3fdfa9ddf2f82a5272b11e2819c70d98) | 6: [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/7WDYfSnwM4JfwSc?file=/&fileId=113878&x=1680&y=1050&a=true&etag=2b7bba4c14e1cbe7775d4d2580af871f) |
***************************

## Verallgemeinte Form der Exponentialfunktion
> $$ f(x) = c \cdot a^{(x+d)} + b$$<br>{1}{<br>b.. Verschiebung entlang der y-Achse um den Wert b}<br>{2}{d .. Verschiebung entlang der x-Achse um den Wert <span style="color:red">***-d***</span><br>}

<iframe src="https://www.geogebra.org/classroom/bewvggex?embed" width="100%" height="800" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>


## Umkehrung der Exponentialfunktion - Der Logarithmus

{{2}}
**********************
> Der <span style="color:orange">***Logarithmus von b zur Basis a (a>0, b>0, a≠1)***</span> ist diejenige Zahl x, mit der man a potentieren muss, um b zu erhalten. Man schreibt kurz<br>
>  $$ x = log_a(b) \textbf{\hspace{0.5cm}ist\ identisch\ zu \hspace{0.5cm}}b = a^x $$
**********************

Beispiel der Bakterien:

> $ B(n) = 2^n $

__Aufgabe:__ Bestimme die Anzahl n von Zeitschritten, nach denen die Anzahl der Bakterien 3.000.000 überschritten hat.

{3}{__Frage:__ Für welches x gilt:  $2^x=3.000.000$}

{4-5}{__Rechnung:__ $ x = log_2(3.000.000)  $} 

{5}{__Rechnung:__ $ x = log_2(3.000.000)  \approx 21,5 $ }

{6}{__Antwort:__ Nach n=22 Zeitschritten hat B(n) den Wert 3.000.000 überschritten.}

<br>
{{1-7}}
<div style='position: relative; padding-bottom: 56.25%; padding-top: 35px; height: 0; overflow: hidden;'><iframe sandbox='allow-scripts allow-same-origin allow-presentation' allowfullscreen='true' allowtransparency='true' frameborder='0' height='315' src='https://www.mentimeter.com/app/presentation/alcop55mvko8ijuddbj2restzfk9oojp/embed' style='position: absolute; top: 0; left: 0; width: 100%; height: 100%;' width='420'></iframe></div>

{{7}}
> <span style="color:darkblue">***Bitte abschreiben.***</span>

## Veranschaulichung des Logarithmus

> $ log_2(3.000.000) $

{0-1}{![Log1](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/Q2Y3i4Ays9YkqMo?file=/&fileId=114730&x=1920&y=1080&a=true&etag=c97733986b2b7ae468ce893dff59dc70)}
{1-2}{![Log2](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/iPeHfDNYaQT6Rg4?file=/&fileId=114731&x=1920&y=1080&a=true&etag=8a9fdcab8a6be19456a04ac782a5d1c0)}
{2-3}{![Log3](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/xqQ8jwxyLP5WzBk?file=/&fileId=114732&x=1920&y=1080&a=true&etag=9616854ba452643ab129efe6dc684e6e)}

## Logarithmus am GTR

> $ log_2(3.000.000) $

{0-1}{![Log1](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/zyqDNiBq6sDFt67?file=/&fileId=114817&x=1680&y=1050&a=true&etag=4a5029ae14176f1afc7edc8c3d78c9a9)}
{1-2}{![Log2](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/J23XDc9jHKGKLGB?file=/&fileId=114819&x=1680&y=1050&a=true&etag=6c3dd2802de67edb6ef678159d70c83b)}
{2-3}{![Log3](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_shanetring/publicpreview/xB668wQiwS3DXPK?file=/&fileId=114820&x=1680&y=1050&a=true&etag=9f1d6074f48a86d96dd3496a9e9df9e9)}

## Aufgaben

<div style="float: right; height: 100px; position: relative; width: 200px; overflow: hidden; top: -80px;"> <div style="overflow: hidden;"> </div> <div> <iframe width="200" height="90" src="https://webuhr.de/embed/timer/#countdown=00:10:00&showbuttons=0&theme=0&ampm=0&sound=xylophone" frameborder="0" allowfullscreen></iframe> </div> </div>

<H4>Für den Merkteil</H4>

1. Zeichne ein Diagramm __(15x15cm)__ in deinen Hefter. Die Werte auf beiden Achsen laufen von <span style="color:orange">***-5 bis 10***</span>.
2. Zeichne den Graph der Funktion <span style="color:darkgreen">**$f(x) = 2^x$**</span> dieses Diagramm. 
3. Zeichne den Graph der Funktion <span style="color:darkred">**$g(x)=log_2(x)$**</span> in das gleiche Koordinatensystem.
4. Überprüfe, wie man _geometrisch_ <span style="color:darkgreen">**f(x)**</span> in <span style="color:darkred">**g(x)**</span> überführen könnte (und umgekehrt).
{{1-2}}
![exp_log](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/yrKXmsmJkpdnSTp?file=/&fileId=114898&x=1920&y=1080&a=true&etag=ca98d36f59db33e532227c64c30709fd)<!--onerror="this.src='ExpFkt_03_04/Exp_Log.png'"-->

{{2-3}}
![exp_log_x](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/REkrygiWjHokEFZ?file=/&fileId=114952&x=1920&y=1080&a=true&etag=01de47f4fde79a3d5e338f7fc7463f55)<!--onerror="this.src='ExpFkt_03_04/Exp_Log_x.png'"-->

<H4>Für den Übungsteil</H4>

5. Löse LB S. 67 

   - 1 a/c/d
   - 2 a/d/h
   - 3 a/b/d/e (__versuche diese Aufgabe ohne GTR__)

{{3}}
**********************

__Lösungen__
| 1 | 2 | 3 |
| [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/2EDk8jTEzHntdRN) | [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/ioQWEQLeKz7d7qG) | [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/DFW3JqRdkFXLDoq) |

**********************

# Periodische Funktionen / Periodische Prozesse

<H2> Was ist bei diesen Beispielen der prinzipielle Unterschied?</H2>

| bisher   | neu  |
| :--------- | :--------- |
| ![money](https://media.giphy.com/media/lNUVjWo9IlRQsnApcw/giphy.gif)  | ![sun](https://media.giphy.com/media/4xe9oTRkO5lmw/giphy.gif) |
| ![bacteria](https://media.giphy.com/media/3osxYeymtCD76SeQjC/giphy.gif)  | ![ticktack](https://media.giphy.com/media/Qz4RaxcOh4qndWOG5N/giphy.gif) |

## Definition periodischer Vorgänge

> Definition: Wir beobachten eine Größe $B$. Der Wert von B zum Zeitpunkt t wird mit $B(t)$ bezeichnet. Wir nennen B eine <span style="color:orange">***periodische Größe***</span>, wenn sich die Werte von B nach einer bestimmten Zeit T wiederholen.
Es soll gelten:

> $$ B(t) = B(t+T) $$ <br> _In Worten: Der Wert von B zum Zeitpunkt t ist genauso groß, wie der Wert von B zum Zeitpunkt t+T._

> <span style="color:red">***T heißt Periodendauer ***</span> von B


{{1}}
**************************
<span style="color:blue">***LB. S. 12 oben***</span>
![EKG](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/kaw3n4oDnTR7RPS?file=/&fileId=116011&x=1920&y=1080&a=true&etag=51c4767e5e3187b8d0cd1cdab006fabf)<!--onerror="this.src='/Periodisch_01_02/EKG.png'"-->
**************************

{{2}}
**************************
<span style="color:blue">***Aufgaben LB S.13 A 1/2***</span>
**************************

{{3}}
**************************
<H3>Finde periodische Prozesse im Alltag. Notiere diesen auf dem orangen Zettel. Notiere auf der Rückseite die Periodenlänge T.</H3>
**************************

## Drehungen und Winkel

Für periodische Vorgänge wie <span style="color:darkblue">***Drehbewegungen***</span> spielt die Winkelbestimmung eine entscheidende Rolle. 

https://www.geogebra.org/classic/ehzzrkk3

{{1}}
***************************
> Wir definieren eine neue Winkeleinheit, das <span style="color:red">***Bogenmaß (auch Radiant genannt)***</span>. Unter dem <span style="color:orange">***Bogenmaß $arc(\alpha)$***</span> versteht man die zu einem im Gradmaß (°) gegebenem Winkel $\alpha$ gehörende <span style="color:red">***Bogenlänge***</span> im Einheitskreis.
***************************

{{2}}
***************************
> Mathematisch exaktes Beispiel: arc(180°) = $\pi$ oder arc(360°) = $2\pi$
***************************

{{3}} 
***************************
> <H4>Wir notieren Winkel in Kurzform: $\alpha = \pi = 180^\circ$ <br> Die Einheit $^\circ$ gibt an, dass wir uns im Gradmaß befinden. <span style="color:red">Steht keine Einheit dabei, gilt das Bogenmaß.</span></H4>

> Umrechnung Gradmaß <-> Bogenmaß: Die Umrechnung kann mit Dreisatz erledigt werden: $2\pi$ ≙ $ 360\circ$ -> wieviel entspricht x Grad?. <br>

- Beispiel Gradmaß->Bogenmaß: $ 140^\circ = \dfrac{2\pi}{360^\circ} \cdot 140^\circ \approx 2,44$
**************************

{{4}} 
***************************
<span style="color:blue">***<H3>Löse im LB S. 15 A 2a und 3a (jeweils 3 Beispiele) </H3>***</span>
__Lösungen__
| 2a | 3a | Am Handy |
| [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/igHGdpRwc7mXd5J?file=/&fileId=117629&x=1920&y=1080&a=true&etag=17138b0af9918f46bad6e2ed44de6e4b) | [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/ozJKY5JykqjYGmf?file=/&fileId=117631&x=1920&y=1080&a=true&etag=0cd81f267ef2fce2d3f6dbd053e689d4) | [qr-code](https://learningapps.org/watch?v=pctrak7fj23) | <iframe src="https://learningapps.org/watch?v=pctrak7fj23" style="border:0px;width:750px;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe> |
***************************

## Die Sinusfunktion

https://www.geogebra.org/classic/ehzzrkk3

{{1}}
![Einheitskreis](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/PiGKRwcNpY9M28A?file=/&fileId=116084&x=1920&y=1080&a=true&etag=3cc573a1d9c016d0925854b58a4e9c30)<!--onerror="this.src='D:\Nextcloud\Documents\Klotzsche\02_Mathe\Kl.10_2023_2024\Periodisch_01_02\Einheitskreis.png'"-->

{{2}}
> Die Funktion mit der Gleichung $ y = f(x) = sin(x) $ heißt __Sinusfunktion__. Sie hat den Definitionsbereich der reellen Zahlen.

{{3}}
> Die Sinusfunktion ist __periodisch mit einer Periodenlänge $2\pi$__ 

## Symmetrie der Sinusfunktion

https://www.geogebra.org/classic/mqanep2j

{{1}}
> Symmetrie: Es gilt: <br> $$ sin(x) = sin(\pi-x) $$ <br> $$ sin(\pi+x) = -sin(x) $$ <br> {4-5}{<span style="color:blue">***finde eine weitere Symmetrie***</span>}

{{2}}
$$ sin(-x)=-sin(x ) $$

## Feedback zum Unterricht

??[Feedback](https://www.mentimeter.com/app/presentation/alcfb7tugn5et752it2i572xj1s8dqmp/c7v79a5mk7zg)

## Parameter der Sinus-Funktion
L
> Parameter beeinflussen Form und Position der Sinusfunktion im Koordinatensystem (vgl. mit Parametern der Exponentialfunktion). Eine Darstellung kann lauten:
> <span style="color:orange">$$f(x) = a \cdot sin(b\cdot x + c) + d$$</span>

{{1}}L
********************
<span style="color:Orange"><H5>Ergebnis: Einfluss des Parameters</H5></span>

> | Veränderung | Auswirkung |
> | a | .. |
> | b | .. |
> | c | .. |
> | d | .. |
********************

{{2}}
********************
<span style="color:orange"><H5>Aufgabe: Wähle eine der zwei folgenden Aufgaben und bearbeite diese in einer kleinen Gruppe (max. 2-4 Personen).</H5></span>

<span style="color:blue">
__1. Visualisierung der Parameter mit Geogebra. [PDF](https://diversewolken.ddns.net/nextcloud/index.php/s/jK8wtWnakZR8BPA)__ <br>
</span> 


Nutze einen PC und gehe zu https://ogy.de/golnik -> Mathe 10b 2023-2024-> Gruppenpuzzle für Sinusfunktion<br>       

a. Teilt die vier Arbeitsaufträge auf und bearbeitet sie parallel (10min). <br>       

b. Erklärt euch im Anschluss den Einfluss eures Parameters anhand der Geogebra Konstruktion (je 5 min). <br>       

c. Mach dir zum Einfluss jedes Parameters eine kurze Skizze im Hefter. <br>

<span style="color:blue">
__2. Visualisierung der Parameter mit dem Lehrbuch.<br>__
</span>
a) Nutze das Lehrbuch S. 28-31 (Abschnitte 1-4). Teilt die Abschnitte unter euch auf. Lies deinen Abschnitt und mache dir im Hefter Notizen zum Einfluss des von dir untersuchten Parameters. <br> 
b) Erkläre mit dem Lehrbuch und deinem Hefter deinem Gruppenmitglied den Einfluss deines Parameters.<br>
c) Mach dir Notizen zu den Informationen deiner Begleiter.
********************


<span style="color:blue"><H5> 3. Löse das Quiz bei Geogebra. </H5> </span>
<details>
   <summary> SinusQuiz </summary>
   https://ogy.de/10b1810
   [qr-code](https://www.geogebra.org/classroom/ddjf3ung)
</details>

## Übungen Sinusfunktion für die KA [OHNE GTR]

<div style="float: right; height: 80px; position: absolute; width: 200px; overflow: hidden; top: 0px; right: 50px"> <div style="overflow: hidden;"> </div> <div> <iframe width="200" height="80" src="https://webuhr.de/embed/timer/#countdown=00:12:00&showbuttons=0&theme=0&ampm=0&sound=xylophone" frameborder="0" allowfullscreen></iframe> </div> </div>

<div style="position: absolute;top:100px;right:50px">
   <details>
      <summary> Aufgabe und Lösung </summary>
      https://ogy.de/10bSinus

      [qr-code](https://liascript.github.io/nightly/?https://api.allorigins.win/raw?url=https://diversewolken.ddns.net/nextcloud/index.php/s/yCxBKy7q4DqFZna/download#1)
   </details>
</div>

> <H4>Gegeben seien die beiden Funktionen: <br> <br>
$     f(x) = 3 \cdot sin(2x) - 1 \hspace{0.5cm} $ und <span style="color:red">$\hspace{0.5cm}$ $^*$</span> $ g(x) = 2 \cdot sin(\frac{3}{4}(x+\pi)) + 2 $ </H4>
 
1) Bestimme für f(x):

| | |
| a) Den Wertebereich | b) Die Periodenlänge | c) Die Extremstellen (innerhalb der ersten Periode) |

2) Zeichne f(x) mit mindestens einer Periode. <br>
   
   _Hinweis: Hier müssen die Extremstellen, die Periodenlänge und der vertikale Offset stimmen. <br> Nutze für f(x) in x-Richtung den Maßstab: 1cm ≙ $\pi/4$_

3) Gib die Funktionsgleichungen zu folgenden drei Funktionen an.

![3_SinusFunktionen](https://diversewolken.ddns.net/nextcloud/index.php/apps/files_sharing/publicpreview/So3FGoQ4ELgAa6k?file=/&fileId=118877&x=1920&y=1200&a=true&etag=8a595db044d9bc3787aca4c6a3d5906f)<!--onerror="this.src='D:\Nextcloud\Documents\Klotzsche\02_Mathe\Kl.10_2023_2024\Uebungen_01_02\3_SinusFunktionen.png'"-->

4*) Löse Aufgabe 1) und 2) für g(x).

## Sinus, Kosinus und Tangens am Einheitskreis

https://www.geogebra.org/classic/zhbbxgvr

## Sinus, Cosinus  und Tangens am Einheitskreis

{{0-1}}
****************
![Einheitskreis_SinusCosinusTangens.png](https://diversewolken.ddns.net/nextcloud/index.php/s/tG4MgQf2Nifkyf8/download)
****************

{{1}}
****************

| | |
| ![Einheitskreis_SinusCosinusTangens.png](https://diversewolken.ddns.net/nextcloud/index.php/s/tG4MgQf2Nifkyf8/download) | ![SinusCosinusDiagramm.png](https://diversewolken.ddns.net/nextcloud/index.php/s/YxMx7rfSSJ9Ctjz/download) |

$\hspace{1cm} cos(\alpha) = sin(\alpha + \dfrac{\pi}{2}) $

****************



{{2}}
****************
<span style="color:blue"><H4>LB. S.38 7</H4></span>

![LB38_7.png](https://diversewolken.ddns.net/nextcloud/index.php/s/ZK5q4DjwAZgWGF5/download)

{{3}}
****************
<span style="color:orange">
$\hspace{1cm}$ (1) mit f(x) und k(x)
</span>
****************

{{4}}
****************
<span style="color:orange">
$\hspace{1cm}$ (2) mit g(x) und h(x)
</span>
****************

{{5}}
****************
<span style="color:orange">
$\hspace{1cm}$ (3) mit i(x) und j(x)
</span>
****************

<span style="color:blue"><H4>Gemeinsamkeiten von Sinus und Kosinus</H4></span>
****************

## Gemeinsamkeiten von Sinus und Kosinus

$\hspace{1cm}$ Periodenlänge ist $2\pi$

$\hspace{1cm}$ Wertebereich $W = \{ y\in\R: -1 \leq y \leq 1 \}$ und Definitionsbereich $D = \R$

$\hspace{1cm} cos(\alpha) = sin(\alpha + \dfrac{\pi}{2}) $

$\hspace{1cm} cos(\dfrac{\pi}{4}) = sin(\dfrac{\pi}{4}) $

$\hspace{1cm}$ Verallgemeinerung der Wirkung von Parametern gilt bei sin und cos.

$\hspace{1cm}$ Amplitude identisch.

## Beautiful Geometry - Numberphile

!?[SineCosine](https://www.youtube.com/watch?v=snHKEpCv0Hk)

# Trigonometrie

??[EinheitskreisUndDreieck](https://www.geogebra.org/classic/bkttaybn)

## Trigonometrie am rechtwinkligen Dreieck

![Trigonometrie](https://diversewolken.ddns.net/nextcloud/index.php/s/raJ7dTnWoPRfFHX/download)

> <H4>Definitionen:</H4> <br>
> __Hypothenuse__: Dem rechten Winkel gegenüberliegende Seite des Dreiecks <br>
> __Gegenkathete (z.B. von $\alpha$)__: Dem Winkel ($\alpha$) gegenüber liegende Seite.<br>
> __Ankathete (z.B. von $\alpha$)__: Schenkel des Winkels ($\alpha$), der nicht die Hypothenuse ist.<br>

{{1}}
*****************
<span style="color:red"><H3>Achte bei Berechnungen auf die GTR Einstellung. 360° oder 2π.</H3></span>
*****************

{2}{<span style="color:blue">***Löse nun die Aufgaben auf dem [Arbeitsblatt Trigonometrie 1](https://diversewolken.ddns.net/nextcloud/index.php/s/s28LQERHxN2cL7X/download)***</span>}

## Winkelberechnung am rechtwinkligen Dreieck (Umkehrung Sinus Kosinus)

> Sind einen rechtwinkligen Dreieck zwei der drei Seitenlängen gegeben, können sämtliche Winkel berechnet werden. Hier wird die Umkehrung des Sinus- bzw. Kosinusfunktion genutzt.

>> Mathematisch werden diese Umkehrungen <span style="color:red">***arcsin***</span> (_Arcussinus_) und <span style="color:red">***arccos***</span> (_Arcuscosinus_) genannt.<br>
>> Am GTR ist die Bezeichnung <span style="color:red">***$sin^{-1}$***</span> oder <span style="color:red">***$cos^{-1}$***</span>.

<H4> Beispiel </H4>
| | |
| ![Umkehrung.png](https://diversewolken.ddns.net/nextcloud/index.php/s/Tj2P3EPbkxiYNKX/download) | geg.: c = 3cm , b = 4cm <br> ges.: $\alpha$ <br> Lsg.: <br> {1}{$\hspace{0.5cm}cos(\alpha) = \dfrac{c}{b}$} <br> <br> {2}{<span style="color:red">$\hspace{0.5cm}\alpha = cos^{-1}\big( \dfrac{c}{b}\big)$ </span>} {3}{$=41,4^\circ$} |


## Anwendungsaufgaben einfache Trigonometrie

### 8. Messtechnik - Sechskant

__Durchmesser eines Werkstücks berechnen__

Aus einem Drehteil soll ein Sechskant gefräst werden. Berechne den Durchmesser des Drehteils (schwarze runde Form), aus dem der Sechskant (blaue Form) für eine Schlüsselweite (orange Linie) von 20 mm gefertigt werden kann?

Geg.: Schlüsselweite = 20 mm
Ges.:	Durchmesser D des Drehteils

![A1.png](https://diversewolken.ddns.net/nextcloud/index.php/s/4BFW3SLYQjJdcrk/download)

Sechskant:<br> ![sechskant.png](https://diversewolken.ddns.net/nextcloud/index.php/s/C9QsrZyRHt7CsRL/download)

#### Lösungshinweis 8.
Ein Sechskant hat 6 gleichlange Seiten; Teilung des Sechskants 360°/ 6 = 60°. Ein Sechskant kann also in sechs gleichseitige Dreiecke zerlegt werden.

#### Lösung 8.

Lösung
Ein Sechskant kann in sechs gleichseitige Dreiecke zerlegt werden. Daher gilt: α = 60°. Daraus folgt auch, dass β = 30°. 

Weiterhin gilt s/2 = 10 mm. 

Ansatz:

$\hspace{1cm} cos(\beta) 	= \dfrac{s/2}{c}$

Einsetzen der bekannten Größen, Lösen nach c:

| | |
|$\hspace{1cm} cos (30°)	= \dfrac{10 mm}{c}$ <br> $\hspace{1cm} c	= \dfrac{10 mm}{cos (30°)}$ <br> $\hspace{1cm} c 	= 11,5 mm$ <br> | ![L1.png](https://diversewolken.ddns.net/nextcloud/index.php/s/r29cB5Ro6Rj3mDD/download)  | 

Daraus folgt, dass der Durchmesser des Drehstücks D = 23 mm beträgt.

### 9. *Gehäuse einer Hydraulikpumpe  berechnen

![A2.png](https://diversewolken.ddns.net/nextcloud/index.php/s/tZME7pRmRxXScEG/download) An dem Ventilgehäuse einer Hydraulikpumpe befinden sich zehn __M6__-Gewinde. Für die Fertigung wird die Lage dieser Gewinde mit den Maßen 30mm; 40mm, 60° bestimmt. <br> Um die Position der oberen und unteren Gewinde schneller und einfacher nach der Fertigung überprüfen (messen) zu können, benötigt man das Maß L. <br> <br>
<span style="color:blue">_Hinweise: In der nebenstehenden technischen Zeichnung sind sämtliche Abstandsangaben in der Einheit mm und die Winkel in ° angegeben._</span> <br> <br>
Aufgabe: Bestimme das Maß L.

#### Lösungshinweis 9.

![H8.png](https://diversewolken.ddns.net/nextcloud/index.php/s/WaQCiHrbyr3oTee/download)


#### Lösung 9.
![H8.png](https://diversewolken.ddns.net/nextcloud/index.php/s/WaQCiHrbyr3oTee/download) Winkelfunktion:<br>
cos(30°) = B/20		B = cos(30°) * 20 = 17,321 mm <br>
sin(30°) = A/20		A = sin(30°) * 20 = 10 mm <br> <br>
Satz des Pythagoras: <br> <br>
(L/2)² = (15 + B)² + A² <br>
(L/2)² = (15 + 17,321)² + 10² = 1144,647 mm <br>
L/2 = √1144,647 = 33,833 mm <br>
__L = 33,833 mm * 2 = 67,67 mm__

### 10. **Bohrungen an einer Adapterplatte berechnen

Bohrungsmaße für Adapterplatte einer hydraulischen Antriebseinheit berechnen

Diese Adapterplatte wird an einer hydraulischen Antriebseinheit eingesetzt. Die zwei schrägen Verbindungsbohrungen mit einem Durchmesser von 8 mm sollen mittels einer Vorrichtung hergestellt werden. Dafür werden die Maße x und y benötigt.

Berechne die Maße x und y in mm.

![A3_1.png](https://diversewolken.ddns.net/nextcloud/index.php/s/seRQ9owjofLwTBP/download)

#### Löungshinweis 10

Lösungsansätze für das Maß x (links) und für das Maß y (rechts)

![A3_2.png](https://diversewolken.ddns.net/nextcloud/index.php/s/Crnd2t4TSnLR4mG/download)

#### Löung 10

Lösungsansätze für das Maß x (links) und für das Maß y (rechts)

![A3_2.png](https://diversewolken.ddns.net/nextcloud/index.php/s/Crnd2t4TSnLR4mG/download)

Das Maß für x beträgt 18,97 mm.
(Zwischenschritte z = 23,51 mm; α = 1,22°; β = 53,78°)

Das Maß für y beträgt 13,44 mm.
(Zwischenschritte z = 26,16 mm; α = 26,08°; β = 30,92°)

## Trigonometrie an allgemeinen Dreiecken

Im folgenden wird angenommen, dass kein Innenwinkel des Dreiecks 90° entspricht.

![AllgemeinesDreieck.png](https://diversewolken.ddns.net/nextcloud/index.php/s/6pS8AYLiK2x25ab/download)<!-- style="width: 100%" -->

## Flächeninhalt eines allgemeinen Dreiecks

{{0-1}}
***********

$A = \dfrac{1}{2}\cdot \text{Grundseite} \cdot \text{Höhe}$

![AllgemeinesDreieck.png](https://diversewolken.ddns.net/nextcloud/index.php/s/f8Dwq75qLZ84Ykn/download)<!-- style="width: 60%" -->

***********



{{1-2}}
***********
$A = \dfrac{1}{2}\cdot \text{Grundseite} \cdot \text{Höhe}$

![AllgemeinesDreieck.png](https://diversewolken.ddns.net/nextcloud/index.php/s/EeSS7ASgzijie4f/download)<!-- style="width: 60%" -->


z.B. $A = \dfrac{1}{2}\cdot c \cdot$ <span style="color:blue">$h_c$</span>
***********

{{2}}
***********

$A = \dfrac{1}{2}\cdot \text{Grundseite} \cdot \text{Höhe}$

![AllgemeinesDreieck.png](https://diversewolken.ddns.net/nextcloud/index.php/s/EeSS7ASgzijie4f/download)<!-- style="width: 60%" -->


$A = \dfrac{1}{2}\cdot c \cdot$ <span style="color:blue">$h_c$</span>

$\boxed{A = \dfrac{1}{2}\cdot c \cdot b \cdot \sin(\alpha)}\,$ {3}{$\boxed{A = \dfrac{1}{2}\cdot a \cdot b \cdot \sin(\gamma)}\,\boxed{A = \dfrac{1}{2}\cdot a \cdot c \cdot \sin(\beta)}$}
***********

## Berechnung verschiedener n-Ecke

<section class="newspaper">

__Gegeben:__

$\alpha = 65° \hspace{0.5cm} \beta=57° $

$ a = 6,10 m \hspace{0.5cm} b = 4,00 m $

![LB.S.123.A4.png](https://diversewolken.ddns.net/nextcloud/index.php/s/a9T95TCgBDyqoEk/download)<!-- style="width: 80%" -->

<p class="cb"> __Gesucht:__ Länge c </p>

__Teilaufgaben:__

 1.1. Berechne die Länge e.

 1.2. Berechne den Winkel $\alpha_1$.

 1.3. Berechne die Winkel $\alpha_2$ und $\delta$

 1.4. Berechne c.

__Lösungshinweise:__ LB S. 123

{{1}}
************
__Weitere Aufgaben:__ (mind 1 pro Kathegorie insgesamt mind. 5)

<span style="color:orange">Wiederholung/Festigung</span>

 - [ ] LB. S. 120 / 2b (_Kosinus-Satz_)
 - [ ] LB. S. 120 / 3a (_Kosinus-Satz_)
 - [ ] LB. S. 122 / 1a oder 1c (_Flächeninhalt_)
 - [ ] LB. S. 122 / 2a (I)  (_Flächeninhalt_)

 <span style="color:orange">Anwendung</span>

 - [ ] *LB S. 122 / 9a/b (Beweis)
 - [ ] LB. S. 125 / 1 oder 2(*)
 - [ ] LB. S. 125 / 4 oder 5
 - [ ] LB. S. 126 / 9
 - [ ] LB S. 127 / 12

<div style="position: absolute;top:10px;right:50px">
   <details>
      <summary> Aufgaben </summary>
      [qr-code](https://liascript.github.io/nightly/?https://raw.githubusercontent.com/wulstbug/Klotzsche/master/02_Mathe/Kl.10_2023_2024/Trigonometrie_07_08_AllgemeineDreiecke_Uebungen/Aufgaben_nEcke.md)
   </details>
</div>

<div style="position: absolute;top:400px;right:50px">
   <details>
      <summary> Lösungen </summary>
      https://ogy.de/10bDreieck1   

      [qr-code](https://diversewolken.ddns.net/nextcloud/index.php/s/2of3Qc6BEJiW94y/download)
   </details>
</div>
 

************

</section>

# Kommentare

| | |
| [qr-code](http://10.102.1.3:8080/survey/access/gl7fejqw) | ??[tuba](http://10.102.1.3:8080/survey/results/gl7fejqw) |

