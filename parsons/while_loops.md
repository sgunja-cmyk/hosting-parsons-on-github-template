---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: WHILE loops
---
# Parsons Practice

## Parsons 1 (Test)
Re-arrange the blocks below: the following code counts down from 10, and when it gets to 0, it prints Blast off!
<div id="whileloops-1-sortableTrash" class="sortable-code"></div> 
<div id="whileloops-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="whileloops-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="whileloops-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "number = 10\n" +
    "while number &gt; 0:\n" +
    "    print(number)\n" +
    "    number = number - 1\n" +
    "print(&quot;Blast off!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "whileloops-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#whileloops-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#whileloops-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



