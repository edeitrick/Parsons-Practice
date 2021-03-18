---
layout: default
title: Conditionals
---
## 1. Detect if a number is even
Arrange the code so that `even` is set to True or False based on if the value of `num` is even or not
<div id="question1-sortableTrash" class="sortable-code"></div> 
<div id="question1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="question1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="question1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if(num % 2 == 0 )\n" +
    "    even = True;\n" +
    "else\n" +
    "    even = False;";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "question1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LanguageTranslationGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "question1-sortableTrash",
    "executable_code": "if num % 2 == 0:\n    even = \"True\"\nelse:\n    even = \"False\"",
    "programmingLang": "java",
    "vartests": [
        {
            "message": "Testing an odd number",
            "initcode": "num = 5\neven = True",
            "code": "",
            "variables": {
                "even": "False"
            }
        },
        {
            "message": "Testing an even number",
            "initcode": "num = 6\neven = False",
            "code": "",
            "variables": {
                "even": "True"
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
