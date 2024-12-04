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

@color
<bdi style="color:@1">@0</bdi>
@end


@rangeQuiz2
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

@onload
window.LIA.settings.font_size = 2
@end

-->

# LB 4 Modellierung und Simulation


![ModellierungSimulation](https://diversewolken.ddns.net/nextcloud/index.php/s/ETBrpgNNii6A2gE/download)

## 4.1 Einführung

![TB_Simulation_1](https://diversewolken.ddns.net/nextcloud/index.php/s/TcbtzC4iX557WHe/download)

![TB_Simulation_1](https://diversewolken.ddns.net/nextcloud/index.php/s/bRRYfqjs7oKe2d5/download)


## 4.2 Demonstrations-Experiment: Freier Fall mit Reibung

![TB_Demo_FreierFall_1](https://diversewolken.ddns.net/nextcloud/index.php/s/wXxCppGqtw8A5ag/download)

![Tafelbild_Demo_FreierFall_2](https://diversewolken.ddns.net/nextcloud/index.php/s/sdMRCrsy24LAC9K/download)

