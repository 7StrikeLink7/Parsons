---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: For Loop Debug
---
# Parsons Practice
![image](https://user-images.githubusercontent.com/68385109/216836410-b7b6f44f-81a6-4793-adfd-1d2637e4b01a.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;First, read all the lines.&quot;)\n" +
    "print(&quot;Second, Cut and Copy lines into the right order.&quot;)\n" +
    "print(&quot;Third, take a screenshot.&quot;)\n" +
    "print(&quot;Lastly, give yourself a pat on the back.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "0-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#0-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#0-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## For Loop 1: Multiplying
Re-arrange the blocks below so that the variables are declared and it prints out the times tables grid using a for loop
<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "numberToMultiply = 1\n" +
    "startNumber = 1\n" +
    "endNumber = 10\n" +
    "for i in range(startNumber, endNumber + 1):\n" +
    "  print(numberToMultiply,&quot;x&quot;,i, &quot;= &quot;, numberToMultiply*i )";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## For Loop 2: Crack the password
Rearrange the code so that the it outputs "Cracking the Password" and one character of the password for every the length of the password. E.g. Cracking the password p cracking the password a cracking the password s .....
<div id="2-sortableTrash" class="sortable-code"></div> 
<div id="2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "superPassword = &quot;passw0rd&quot;\n" +
    "for letter in superPassword:\n" +
    "  print(&quot;Cracking the password...&quot;)\n" +
    "  print(letter)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "2-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>




