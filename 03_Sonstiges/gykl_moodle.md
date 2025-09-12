<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.jpg 

logo: https://upload.wikimedia.org/wikipedia/commons/f/f8/Enigma_%2820967055154%29.jpg

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

# GYKL - Moodle

![Moodle-Logo](https://www.lucushost.com/blog/wp-content/uploads/2023/06/que-es-moodle.png)

>__Gliederung__
>
>- Zugang zu Gykl-Moodle (Lehrkräfte)
>
>- Kurze Demo (LK/Test)
>
>- Einführung in Kursadministration
>
>- Logins der SuS
>
>- gemeinsam Fragen erstellen
>
>- Fragen erstellen mit KI-Support

## Zugang zu Gykl-Moodle

[https://ogy.de/gyklmoodle](https://ogy.de/gyklmoodle)

[qr-code](https://ogy.de/gyklmoodle)

## Demo-Kurs

[Link-Zum-Demo-Kurs](https://diversewolken.ddns.net/moodle/enrol/index.php?id=43)


## Einführung in Kursadministration

<div style="position: relative; width: 100%; height: 0; padding-top: 56.2500%;
 padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
 border-radius: 8px; will-change: transform;">
  <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
    src="https://www.canva.com/design/DAGwmSNfdIY/5ZMtDCtfQRzg-1brphZMtw/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
  </iframe>
</div>
<a href="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAGwmSNfdIY&#x2F;5ZMtDCtfQRzg-1brphZMtw&#x2F;view?utm_content=DAGwmSNfdIY&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener">Demo-Bio-LK</a> von Golnik Ch

## Logins der SuS

__Login-Name__ jedes SoS ist die Lernsax-Email-Adresse:

> *nachname.vorname@gykl.lernsax.de*

__Erstpasswort__ ist immer das was vor dem @ Symbol steht, also:

> _nachname.vorname_

__Passwort vergessen?__

> Unterhalb des Login-Bereichs gibt es den Button 
>
> _Passwort vergessen_ 

__Notfall: von Lehrkraft einloggen lassen__

> Im Notfall kann die Lehrkraft jede Person einloggen. Dazu:

1. Als Lehrkraft im Kurs einloggen

2. Auf der linken Seite den Link _Teilnehmer/innnen_ auswählen

3. Auf der rechten Seite den jeweiligen Namen suchen und anklicken

4. Im rechten Bereich gibt es unterhalb von Teilnehmer/innen den Reiter _More_

5. Herunterscrollen und den Eintrag __Anmelden als__ verwenden


## Frage erstellen

<p class="newspaper">

![Fragetypen](https://diversewolken.ddns.net/nextcloud/index.php/s/BsTgZ36zmr3sTbP/download)

<p class="cb">

> - Fragetyp auswählen
>
> - Geforderte Felder ausfüllen
>
> - Speichern
>
> - Unter _Fragen_ in den Test einfügen

</p>

</p>


## Frage mit KI Unterstüztung erstellen


<p style="color:blue">
Kopiere den Prompt in das Feld der KI (nutze den Button _Kopieren_). Beantworte dann die gestellten Aufgabe.
</p>

---

__Aufgabe:__<br> Kopiere den Text.

<div class="container" style="margin-left:10%">
__Prompt__ <br>
<span class="text-box" id="textToCopy2"> Erstelle mir eine Multiple-Choice Frage in einem Format dass ich in Moodle importieren kann. Die Frage lautet: Was ist der erste Buchstabe des Alphabet. Möglichkeiten: A (richtig), B(falsch), C(falsch). </span>
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

Login: golnik.ch@gykl.lernsax.de

Passwort: golnik.ch

[KI-OpenWebUI](http://10.102.1.3:3001)

