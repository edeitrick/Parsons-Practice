---
layout: default
title: Variables
---
## 1. Swap the variables
Arrange the code so that it swaps the values of `x` and `y`
<div id="sortableTrash" class="sortable-code"></div>
<div id="sortable" class="sortable-code"></div>
<div style="clear:both;"></div>

<p>
    <input id="feedbackLink" value="Get Feedback" type="button" />
    <input id="newInstanceLink" value="Reset Problem" type="button" />
</p>

<script type="text/javascript">
var initial = "1\n" +
    "2\n" +
    "3\n" +
    "4\n" +
    "5";
var parsonsPuzzle2 = new ParsonsWidget({
    "sortableId": "sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en"
});
parsonsPuzzle2.init(initial);
parsonsPuzzle2.shuffleLines();
$("#newInstanceLink").click(function(event){
    event.preventDefault();
    parsonsPuzzle2.shuffleLines();
});
$("#feedbackLink").click(function(event){
    event.preventDefault();
    parsonsPuzzle2.getFeedback();
});
</script>



[Back to list of Practice Problems](../index.html)
