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

.red {
    color: red;
}

.blue {
    color: blue;
}

.darkgreen {
    color: darkgreen;
}

.orange {
    color: orange;
}

.purple {
    color: purple;
}

@end


@onload
window.LIA.settings.font_size = 2
@end

-->

### Aufgaben zur Kreisbewegung

Im Folgenden sind Aufgaben zur Kreisbewegung gestellt. Die Aufgaben sind mit "Aufwändigkeits-Marken" versehen. 

- (+) geringer Aufwand
- (++) mittlerer Aufwand
- (+++) erhöhter Aufwand


<p style="color:red">
>> __Löse insgesamt 7 Aufgaben. Davon sollen mindestens zwei Aufgaben (++) und eine Aufgabe (+++) enthalten sein.__
</p>

#### 1. Kugel am Faden (++)

Eine Kugel (m = 2,5 kg) wird gleichförmig an einem Faden der Länge 40 cm mit einer Bahngeschwindigkeit von 36 km/h auf einer Kreisbahn bewegt.​

---

1. 1. Benenne die Kraft, welche auf die Kugel wirkt und als Zentripedalkraft fungiert.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.1 </summary>

Der Faden hält die Kugel auf der Kreisbahn. Demzufolge fungiert die Fadenkraft hier als Zentripedalkraft.

</details>

</div>

---


1. 2. Berechne die Kraft, welche auf die Kugel wirkt und als Zentripedalkraft fungiert.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.2 </summary>

Rechne sämtliche gegebenen Größen in die Standardeinheiten um und setze diese in die Formel für die Zentripedalkraft (2.9.) ein.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.2 </summary>

$$F_r = \dfrac{m \cdot v^2}{r} = \dfrac{2,5\,kg \cdot (10\frac{m}{s})^2}{0,4\,m} = 625\,N$$

</details>

</div>

---

1. 2. Berechne die Zeit, die nötig ist, damit die Kugel zwei Umdrehungen schafft.

<div style="text-indent:10%">

<details>

<summary> Hinweis 1.3 </summary>

Berechne aus den gegebenen Werten den Umfang $u$ des Kreises. Die Kugel legt in gleichförmiger Bewegung die Strecke $2u$ zurück. Mit der gegebenen Geschwindigkeit lässt sich die Zeit ermitteln.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 1.3 </summary>

Der Umfang $u$ eines Kreises wird berechnet mit $u = 2\pi\cdot r$. Die Zeit, welche die Kugel bei gleichförmiger Bewegung für 2 Umläufe braucht ist daher $$t=\frac{2\cdot u}{v}\approx0,503\,s$$.

</details>

</div>

#### 2. Fahrradtachometer (++)

Ein Fahrradtachometer bestehend aus einem Sensor und einem Magneten (mittig montiert auf der Speiche zwischen Lauffläche und Nabe). Das Rad hat einen Durchmesser von 635 mm. Er misst alle 0,25s eine Umdrehung.

---

2. 1. Fertige eine Skizze zur Aufgabe an. Trage die gegebenen Größen ein.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.1 </summary>

![KB_Lsg_2.1](https://diversewolken.ddns.net/nextcloud/index.php/s/PEYT5WH9o8x4GGH/download)

</details>

</div>

---

2. 2. Berechne die Bahngeschwindigkeiten des Magneten und der Lauffläche.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.2 </summary>

![KB_Lsg_2.2](https://diversewolken.ddns.net/nextcloud/index.php/s/6GEe3gTeiG7pMyS/download)

</details>

</div>

---

2. 3. Berechne die Kraft, die nötig ist, damit der Magnet ($m=10g$) an der Speiche bleibt.

<div style="text-indent:10%">

<details>

<summary> Lösung 2.3 </summary>

![KB_Lsg_2.3](https://diversewolken.ddns.net/nextcloud/index.php/s/P3W7LZBZ3LaHCnB/download)

</details>

</div>

#### 3. Satellitenbahn (+++)

3. 1. Erläutere die Bewegung eines Satelliten um die Erde. Erkläre warum der Satellit nicht auf die Erde stürzt. 

<div style="text-indent:10%">

<details>

<summary> Lösung 3.1 </summary>

![KB_Lsg_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/kYBZsG4kTxDngXf/download)

</details>

</div>

---

3. 2. Zeige, dass der Radius des geostationären Orbits für Erdsatteliten etwa 42000 km beträgt. <br> _Hinweis: Bei einem geostationären Orbit bleibt der Satellit immer über dem gleichen Punkt auf der Erdoberfläche._

<div style="text-indent:10%">

<details>

<summary> Hinweis 3.2. A</summary>

Recherchiere, wie sich die Gravitationskraft in größerer Entfernung von der Erde berechnen lässt (hier gilt nicht $F_g=m\cdot g$).

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Hinweis 3.2. B </summary>

$$ F_g = G\cdot\frac{m\cdot M}{r^2} $$ 

($M$..Erdmasse, $G$..Graviationskonstante)

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 3.2 A </summary>

![KB_Lsg_3.2A](https://diversewolken.ddns.net/nextcloud/index.php/s/9Tbn8xWaW97xXCL/download)

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 3.2 B </summary>

![KB_Lsg_3.2B](https://diversewolken.ddns.net/nextcloud/index.php/s/RiTem8mfeWk2ZZt/download)

</details>

</div>

#### 4. Kurvenfahrt (+++)

Bei Kurvenfahrten mit konstanter Geschwindigkeit treten an einem Fahrzeug zwischen Reifen und Fahrbahn zwei Arten von Reibungskräften auf. Die Rollreibung wirkt parallel zur Bewegungsrichtung, Haftreibung wirkt senkrecht zur Bewegungsrichtung. 
Ein Fahrzeug (1,5 t) bewegt sich auf einer kreisförmigen Kurve (Radius 50 m) mit einer konstanten Geschwindigkeit von 72 km/h. Die Haftreibungszahl µHaft zwischen Reifen und Fahrbahn beträgt 0,85. Die Rollreibungszahl µRoll beträgt 0,025.

---

4. 1. Entscheiden Sie, ob die Haftreibung in diesem Fall eine erwünschte oder eine unerwünschte Reibungskraft ist. Begründen Sie Ihre Entscheidung. Ermitteln Sie den Wert der Haftreibungskraft.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.1</summary>

Für eine Kreisbewegung muss eine Kraft als Zentripedalkraft zum Mittelpunkt der Kreis/Kurvenbahn zeigen. Überlegen Sie welche der beschriebenen Kräfte, das sein könnte und entscheiden Sie dann, ob diese Kraft erwünscht ist.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.1 A</summary>

Da die Zentripedalkraft immer senkrecht zur Bewegungsrichtung wirkt, kommt hier nur die Haftreibungskraft als Zentripedalkraft in Frage. Diese wäre dann eine erwünschte Reibungskraft, weil sonst die Kurvenfahrt nicht durchgeführt werden könnte.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.1 B</summary>

$F_{haft} = F_g \cdot \mu_{haft} = m \cdot g \cdot \mu_{haft} = 1500\,kg\cdot9,81\,\frac{N}{kg}\cdot0,85$

$\underline{F_{haft} = 12508 N}$


</details>

</div>

---

4. 2. Begründen Sie, warum das Fahrzeug nicht mit beliebig hoher Geschwindigkeit durch die Kurve fahren kann. Diskutieren Sie dazu die für die Kreisbewegung relevanten Kräfte.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.2 </summary>

Die Haftreibungskraft wirkt als Zentripedalkraft. Überprüfen Sie anhand der Formel den Zusammenhang von Zentripedalkraft und Geschwindigkeit. Schätzen Sie ein, ob sich die Haftreibungskraft mit zunehmender Geschwindigkeit ändert?

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.2</summary>

Die Haftreibungskraft ist nicht von der Geschwindigkeit abhängig. Bei wachsender Geschwindigkeit aber festem Kurvenradius muss die Zentripedalkraft wachsen, damit die Kreisbewegung stattfinden kann. Überschreitet die geforderte Zentripedalkraft die Haftreibungskraft, so rutscht das Fahrzeug aus der Kurve.

</details>

</div>

---

4. 3. Ermitteln Sie die Höchstgeschwindigkeit für die beschriebene Kurvenfahrt.

<div style="text-indent:10%">

<details>

<summary> Hinweis 4.3 </summary>

Setzen Sie für den Grenzfall Haftreibungskraft und Zentripedalkraft gleich.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 4.3 </summary>

![KB_Lsg_4.3](https://diversewolken.ddns.net/nextcloud/index.php/s/9Zjg4azKE4CmNAA/download)

</details>

</div>

#### 5. Erdrotation (+)

5. Der Erdradius beträgt etwa 6370 km. Ermitteln Sie die Geschwindigkeit, mit der sich ein Punkt auf der Erdoberfläche des Äquators bei der Erddrehung bewegt? Beachten Sie: Die Erde dreht sich in einem Tag einmal um sich selbst.

<div style="text-indent:10%">

<details>

<summary> Lösung 5. </summary>

>![Lsg_3.1](https://diversewolken.ddns.net/nextcloud/index.php/s/JDkA7GJwBgw8Led/download)

</details>

</div>

#### 6. Turmuhr (++)

6.1  Die Spitze des Minutenzeigers einer Turmuhr hat die Geschwindigkeit $1,5 \frac{mm}{s}$. Ermitteln Sie die Zeigerlänge?

<div style="text-indent:10%">

<details>

<summary> Lösung 6.1 </summary>

>![Lsg_3.2](https://diversewolken.ddns.net/nextcloud/index.php/s/LQAmgYazNjHo3rD/download)

</details>

</div>

---

6.2  Bestimmen Sie unter Berücksichtigung physikalisch möglicher Geschwindigkeiten die maximale (hypotetische) Größe einer Uhr, d.h. ihrer Zeigerlänge (Minutenzeiger). Setzen Sie Ihr Ergebnis mit einer typischen astronomischen Entfernung sinnvoll ins Verhältnis.

<div style="text-indent:10%">

<details>

<summary> Hinweis 6.2 </summary>

Ermitteln Sie die größte überhaupt mögliche Geschwindigkeit. Überlegen Sie, welcher Teil der Uhr sich mit der größten Geschwindigkeit bewegt. Setzen Sie die Maximalgeschwindigkeit für diesen Teil an.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 6.2 A</summary>

Die maximal mögliche Geschwindigkeit ist die Lichtgeschwindigkeit $c=300.000\,\frac{km}{s}$. Der schnellste Teil einer Uhr ist die Zeigerspitze des Minutenzeigers. Dieser kann sich nach physikalischen Prinzipien nicht schneller als mit Lichtgeschwindigkeit bewegen. Setzt man Lichtgeschwindigkeit für die Zeigerspitze an, ergibt sich die größtmögliche Uhr. Setzen Sie dieses Ergebnis mit einer astronomischen Entfernung sinnvoll ins Verhältnis.

</details>

</div>

<div style="text-indent:10%">

<details>

<summary> Lösung 6.2 A</summary>

$ c = \dfrac{2\pi\cdot r}{T}$ mit $T=60\cdot60\,s$ und $c=300.000.000\,\frac{m}{s}$

$ r = \dfrac{T\cdot c}{2\pi} = \dfrac{3600\,s\cdot 300.000.000 \frac{m}{s}}{2\pi}$

$ \underline{r \approx 1,72 \cdot 10^{11}m}$

Der Abstand Erde Sonne (auch eine astronomische Einheit genannt) beträgt etwa $1,5\cdot 10^{11}m$. Der Minutenzeiger einer Uhr und deren Zeiger sich um das Zentrum der Sonne drehen würden, deren Länge etwas weiter als bis zur Erde reichen würde, hätten an der Spitze ungefähr Lichtgeschwindigkeit.

Alternativ: Das Verhältnis der hypothetischen Zeigerlänge zum Abstand Erde-Sonne beträgt etwa 1,15.

</details>

</div>

#### 7. Dynamo (+)

7. Fahrradfahren/Dynamo

![A3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/Xz8KES8f8kHPE3G/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 7. </summary>

> ![Lsg_3.3](https://diversewolken.ddns.net/nextcloud/index.php/s/XsJtHCgnrrBqPb5/download)

</details>

</div>

#### 8. Flugzeugturbinen (+)

8. Turbinen und Drehgeschwindigkeit

![A3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/A4yG37d3eHf6ZTL/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 8. </summary>

> ![Lsg_3.4](https://diversewolken.ddns.net/nextcloud/index.php/s/qTEzgnK4ZZcGcxB/download)

</details>

</div>

#### 9. Winkelschleifer (+)

![A3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/5xsPM2oXRNsEmzZ/download)

<div style="text-indent:10%">

<details>

<summary> Lösung 9. </summary>

> ![Lsg_3.5](https://diversewolken.ddns.net/nextcloud/index.php/s/dEGwgjJLZ5Lx9YY/download)

</details>

</div>
