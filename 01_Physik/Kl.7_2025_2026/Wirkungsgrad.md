<!--
icon:   https://diversewolken.ddns.net/klotzsche/logo.png 

author: Christian Golnik

language: de

logo: https://snu.edu.in/site/assets/files/18322/nanotechnology-molecule-atom-model-image-mixed-media_2.1600x0.webp

import: https://raw.githubusercontent.com/wulstbug/Klotzsche2/2025_2026/03_Sonstiges/settings.md

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

h1, h2, h3, h4, h5, h6 {
  column-span: all;
}

.cb {
    break-before: column;
    display: block;
}

@end

@onload
window.LIA.settings.font_size = 2


const canvas = document.querySelector('.lia-canvas')
if (canvas) {
  canvas.classList.remove('lia-navigation--visible')
  canvas.classList.add('lia-navigation--hidden')
}

@end

mode: presentation

-->

# Der Wirkungsgrad

## Die Energieformen

```ascii
                            +--------------------------------------------------+
                            |               FORMEN DER ENERGIE                 |
                            +--------------------------------------------------+

                                          .----------------.
                                         (  Lichtenergie    )
                                          '----------------'

 .----------------.                                                             .----------------------.
(   Kernenergie    )                                                           ( chemische Energie      )
 '----------------'                                                             '----------------------'

                                        .---------------------------.  
 .----------------.                    ( Thermische Energie          )            .----------------.
( Rotationsenergie )                   ( (Wärmeenergie)              )           ( Bewegungsenergie )
 '----------------'                     '---------------------------'            ( = kinetische E.  )
                                                                                  '----------------'


 .----------------.                     .----------------.                       .----------------.
( Rotationsenergie )                   ( magnetische      )                     ( elektrische      )
 '----------------'                    ( Energie          )                     ( Energie          )
                                        '----------------'                       '----------------' 
                                                                                
                                                                                


                            
```

## Beispiel 1


```ascii

+------------------------------------------------------+
|                       BEISPIEL 1                     |
+------------------------------------------------------+


                 +----------------------+
                 | chemische Energie    |
                 +----------------------+
                            |
          +-----------------+-----------------+
          |                 |                 |
          v                 v                 v

 +----------------+ +----------------+ +----------------------+
 | Bewegungs-     | | Rotations-     | | thermische Energie   |
 | energie        | | energie        | | (Wärmeenergie)       |
 +----------------+ +----------------+ +----------------------+

```

## Beispiel 2


```ascii

+------------------------------------------------------+
|                       BEISPIEL 2                     |
+------------------------------------------------------+


                 +----------------------+
                 | elektr. Energie      |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v

          +----------------+   +----------------------+
          | Lichtenergie   |   | thermische Energie   |
          |                |   | (Wärmeenergie)       |
          +----------------+   +----------------------+


```

## Beispiel 3

```ascii

+------------------------------------------------------+
|                       BEISPIEL 3                     |
+------------------------------------------------------+


                 +----------------------+
                 |     Kernenergie      |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v

          +----------------+   +----------------------+
          |elektr. Energie |   | thermische Energie   |
          |                |   | (Wärmeenergie)       |
          +----------------+   +----------------------+


```
## Beispiel 4

```ascii

+------------------------------------------------------+
|                       BEISPIEL 4                     |
+------------------------------------------------------+


                 +----------------------+
                 | magnetische Energie  |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v

          +----------------+   +----------------------+
          |  pot . Energie |   | Bewegungsenergie     |
          |                |   |                      |
          +----------------+   +----------------------+


```

## Beispiel 5

```ascii

+------------------------------------------------------+
|                       BEISPIEL 5                     |
+------------------------------------------------------+


                 +----------------------+
                 | chem. Energie        |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v
          +----------------+   +----------------------+
          |  Lichtenergie  |   | thermische Energie   |
          |                |   | (Wärmeenergie)       |
          +----------------+   +----------------------+


```

## Beispiel 6

```ascii

+------------------------------------------------------+
|                       BEISPIEL 6                     |
+------------------------------------------------------+


                 +----------------------+
                 | chem. Energie        |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v
          +----------------+   +----------------------+
          | elektr. Energie|   | thermische Energie   |
          |                |   | (Wärmeenergie)       |
          +----------------+   +----------------------+


```

## Beispiel 7

```ascii

+------------------------------------------------------+
|                       BEISPIEL 7                     |
+------------------------------------------------------+


                 +----------------------+
                 | elektr. Energie      |
                 +----------------------+
                            |
          +-----------------+-----------------+
          |                 |                 |
          v                 v                 v

 +----------------+ +----------------+ +----------------------+
 | Bewegungs-     | | Rotations-     | | thermische Energie   |
 | energie        | | energie        | | (Wärmeenergie)       |
 +----------------+ +----------------+ +----------------------+


```

## Beispiel 8

```ascii

+------------------------------------------------------+
|                       BEISPIEL 8                     |
+------------------------------------------------------+


                 +----------------------+
                 | potentielle Energie  |
                 +----------------------+
                            |
          +-----------------+-----------------+
          |                 |                 |
          v                 v                 v

 +----------------+ +----------------+ +----------------------+
 | Bewegungs-     | | Rotations-     | | thermische Energie   |
 | energie        | | energie        | | (Wärmeenergie)       |
 +----------------+ +----------------+ +----------------------+


```

## Beispiel 9

```ascii

+------------------------------------------------------+
|                       BEISPIEL 9                     |
+------------------------------------------------------+


                 +----------------------+
                 |    elektr. Energie   |
                 +----------------------+
                            |
                            +
                            |
                            v
                +----------------------+
                | thermische Energie   |
                | (Wärmeenergie)       |
                +----------------------+


```

## Beispiel 10

```ascii

+------------------------------------------------------+
|                       BEISPIEL 10                    |
+------------------------------------------------------+


                 +----------------------+
                 |    Rotationsenergie  |
                 +----------------------+
                            |
                            +
                            |
                            v
                +----------------------+
                | thermische Energie   |
                | (Wärmeenergie)       |
                +----------------------+


```

## Beispiel 11

```ascii

+------------------------------------------------------+
|                       BEISPIEL 11                    |
+------------------------------------------------------+


                 +----------------------+
                 |     Lichtenergie     |
                 +----------------------+
                            |
                            +
                            |
                            v
                +----------------------+
                |      chem. Energie   |
                +----------------------+


```

## Beispiel 12

```ascii

+------------------------------------------------------+
|                       BEISPIEL 6                     |
+------------------------------------------------------+


                 +----------------------+
                 | Kernenergieenergie   |
                 +----------------------+
                            |
                    +-------+-------+
                    |               |
                    v               v
          +----------------+   +----------------------+
          |  Lichtenergie  |   | thermische Energie   |
          |                |   | (Wärmeenergie)       |
          +----------------+   +----------------------+


```

# Die Effizienz von Energiewandlern

__Technische Geräte oder Vorgänge in der Natur wandeln__ @color(zugeführte Energie $E_{zu}$, orange) in eine oder mehrere Energieformen um. Dabei können wir oft nur eine umgewandelte @color(Energieform nutzen $E_{nutz}$, blue).

{{1}}
***********
> Der Wirkungsgrad für gibt an, welchen Anteil (in %) wir von der @color(zugeführten Energie $E_{zu}$) überhaupt @color(nutzen, blue) können.
>
> $$ \boxed{\eta = \dfrac{\orange{E_{nutz}}}{\blue{E_{zu}}}}$$
***********

{{2}}
***********
Man sagt: "Je __höher__ der Wirkungsgrad, desto __effizienter__ arbeitet ein Energiewandler."
***********

{{3}}
***********
__Aufgaben:__

- AH. S.31  /A. 1, 3
- LB. S.116 /A. 3, 4 (gemeinsam)
- LB. S.122 /A. 1
- AH. S.31  /A. 2, 4
- LB. S.122 /A. 3, 4
***********