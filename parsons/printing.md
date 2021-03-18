---
layout: default
title: Printing Practice
---

## 1. Java Printing
Construct a Java program that prints out "Hello World!"
<div id="question1-sortableTrash" class="sortable-code"></div> 
<div id="question1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="question1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="question1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "System.out.print(&quot;Hello &quot;)\n" +
    "System.out.println(&quot;World!&quot;)\n" +
    "System.out.println(&quot;Hello &quot;) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "question1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "trashId": "question1-sortableTrash"
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

## 2. Python Printing
Construct a Python program that prints out "Hello World!"
<div id="question2-sortableTrash" class="sortable-code"></div> 
<div id="question2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="question2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="question2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Hello &quot;, endl=&quot;&quot;)\n" +
    "print(&quot;World!&quot;)\n" +
    "print(&quot;Hello &quot;) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "question2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "trashId": "question2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#question2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#question2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## 3. C++ Printing
Construct a C++ program that prints out "Hello World!"

<div id="question3-sortableTrash" class="sortable-code"></div> 
<div id="question3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="question3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="question3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "cout &lt;&lt; &quot;Hello &quot;;\n" +
    "cout &lt;&lt; &quot;World!&quot; &lt;&lt; endl;\n" +
    "cout &lt;&lt; &quot;Hello&quot; &lt;&lt; endl; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "question3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en",
    "trashId": "question3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#question3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#question3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Back to list of Practice Problems](../index.html)
