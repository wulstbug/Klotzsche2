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


@rangeQuiz2
<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;">
@0 =
</div> 
<div style="float:left">
<!-- data-solution-button="off" -->
[[ @1 ]]
<script>
let input = "@input".replace(",", ".")
try {
    input = Math.abs(eval(input)-@1)/Math.abs(input)
    input <= 0.03
} catch (e) {
    false
}
</script>
</div> 
<div style="float:left;width:100px;">
@2
</div>
</div>
@end

-->

# Settings for LIA

Image Centered

![Plattenkondensator](https://diversewolken.ddns.net/nextcloud/index.php/s/Sw39rmgGTYbZL7S/download) <!--style="display:block;margin-left:auto;margin-right:auto; max-width:400px"-->

# RangeQuiz

@rangeQuiz(0.5)

<div style="display: flex;flex-direction: row;flex-wrap: nowrap">
<div style="float:left;">
F=
</div> 
<div style="float:left;width:100px;">
@rangeQuiz(0.5)
</div> 
<div style="float:left;width:100px;">
N
</div>
</div>

@rangeQuiz2(F,0.51,N)