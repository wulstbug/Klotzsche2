<!--
@style
.lia-effect__circle {
    display: none !important;
}
@end

@color
<div style="color:@1">@0</div>
@end

@test
end
@end

@rangeQuiz
<!-- data-solution-button="off" -->
[[ @0 ]]
<script>
let input = "@input".replace(",", ".")

try {
    input = Math.abs(eval(input)-@0)/Math.abs(input)
    
    input <= 0.03
} catch (e) {
    false
}
</script>
@end

-->

# Settings for LIA

Image Centered

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

# RangeQuiz

@rangeQuiz(0.5)
