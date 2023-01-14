---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: For Loop Debug
---
# Parsons Practice
## Parsons 1 (Line Based Grader)
Re-arrange the blocks below so that the variables are declared and it prints out the times tables grid using a for loop

<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "numberToMultiply = 1\n" +
    "startNumber = 1\n" +
    "endNumber = 10\n" +
    "for i in range(startNumber, endNumber + 1):\n" +
    "  print(numberToMultiply,\"x\",i, \"= \", numberToMultiply*i )";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.VariableCheckGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "sortableTrash",
    "vartests": [
        {
            "message": "Check",
            "initcode": "10\n5",
            "code": "Correct",
            "variables": {}
        },
        {
            "message": "Check",
            "initcode": "10\n5",
            "code": "Correct",
            "variables": {}
        }
    ]
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>




