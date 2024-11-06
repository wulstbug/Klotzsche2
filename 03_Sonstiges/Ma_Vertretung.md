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

mode: presentation

-->

# Lösungen Lehrbuch

__Aufgabe 14__

- {1}{![14_a](https://diversewolken.ddns.net/nextcloud/index.php/s/p2SCed3xdgFJ5Ad/download)}

- {2}{![14_b](https://diversewolken.ddns.net/nextcloud/index.php/s/aFqFW2rGi4zF6AL/download)}

- {3}{![14_c](https://diversewolken.ddns.net/nextcloud/index.php/s/4eJkYqPH7tRwHEH/download)}

<p class="newspaper">

__Seite 23__

![1](https://diversewolken.ddns.net/nextcloud/index.php/s/kZRrH5eyaZHSWjm/download)

![2](https://diversewolken.ddns.net/nextcloud/index.php/s/4Jg9pRxc9djqzTB/download)

![3](https://diversewolken.ddns.net/nextcloud/index.php/s/gASgziKdwYn7JyD/download)

![4](https://diversewolken.ddns.net/nextcloud/index.php/s/KLkqNG6Yir4grfD/download)

![5](https://diversewolken.ddns.net/nextcloud/index.php/s/9j54ZBFddrzsQBq/download)


<p class="cb">

__Seite 24__

![1](https://diversewolken.ddns.net/nextcloud/index.php/s/kZRrH5eyaZHSWjm/download)

![2](https://diversewolken.ddns.net/nextcloud/index.php/s/8NxzwqkKH6D9RGa/download)

![3](https://diversewolken.ddns.net/nextcloud/index.php/s/5JpK2NTcnrB6pCb/download)

![4](https://diversewolken.ddns.net/nextcloud/index.php/s/toN3ioPaRWjoZFC/download)


</p>

</p>

