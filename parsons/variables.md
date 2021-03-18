---
layout: default
title: Variables
---
## 1. Swap the variables
Arrange the code so that it swaps the values of `x` and `y`
<div id="question1-sortableTrash" class="sortable-code"></div> 
<div id="question1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="question1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="question1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "$$toggle::x::y::tmp$$ = $$toggle::x::y::tmp$$\n" +
    "$$toggle::x::y::tmp$$ = $$toggle::x::y::tmp$$\n" +
    "$$toggle::x::y::tmp$$ = $$toggle::x::y::tmp$$";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "question1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.VariableCheckGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "trashId": "question1-sortableTrash",
    "vartests": [
        {
            "message": "X value is correct",
            "initcode": "x = 2\ny = 1",
            "code": "",
            "variables": {
                "x": 1
            }
        },
        {
            "message": "Y value is correct",
            "initcode": "x = 2\ny = 1",
            "code": "",
            "variables": {
                "y": 2
            }
        }
    ]
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#question1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#question1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



[Back to list of Practice Problems](../index.html)
