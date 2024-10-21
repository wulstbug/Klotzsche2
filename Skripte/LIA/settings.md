<!--
author: Christian Golnik

language: de

@style
.lia-effect__circle {
    display: none !important;
}

@onload
window.LIA.settings.font_size = 2
@end

@uhr
<div style="position: fixed; right:50px; top:100px;">

   <details>

      <summary> Uhrzeit </summary>

      <div style="text-align:left;padding:1em 0;"> <iframe src="https://www.zeitverschiebung.net/clock-widget-iframe-v2?language=de&size=large&timezone=Europe%2FBerlin" width="100%" height="150" frameborder="0" seamless></iframe> </div>

   </details>

</div>

@end

@color
<div style="color:@1">@0</div>
@end

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

-->

# Settings for LIA

Image Centered

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->