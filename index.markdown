---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Multiple Parson's Problems on One Page
---
# Parsons Practice

## Parsons 1 (Test)
Re-arrange the blocks below.

<div id="code-1-sortableTrash" class="sortable-code"></div> 
<div id="code-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="code-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="code-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "num1 = int(input(&#039;Enter number 1: &#039;))\n" +
    "num2 = int(input(&#039;Enter number 2: &#039;))\n" +
    "answer = num1 + num2\n" +
    "print(answer)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "code-1-sortable",
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
  $("#code-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#code-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Parsons 2 (Function)
Rearrange the blocks below so the code works. This function checks whether a number is even or odd.

<div id="function-1-sortableTrash" class="sortable-code"></div> 
<div id="function-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="function-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="function-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def check_even_odd(number):\n" +
    "    if number % 2 == 0:\n" +
    "        result = &quot;even&quot;\n" +
    "    else:\n" +
    "        result = &quot;odd&quot;\n" +
    "    \n" +
    "    return result\n" +
    "num = int(input(&quot;Enter a number: &quot;))\n" +
    "answer = check_even_odd(num)\n" +
    "print(f&quot;The number {num} is {answer}.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "function-1-sortable",
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
  $("#function-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#function-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

### Implementation Notes

When you host multiple Parson's problems on a single markdown page, you need to add a unique prefix. You can easily do this in the Codio generator by typing a unique prefix into the "Prefix" textbox and pressing Enter/Return. Then you can simply copy-paste like normal.

If want each problem to be it's own page, you can use relative path links at the bottom of each of your markdown pages as seen below. If you want students to be able to return to previous problems in this format, consider adding previous links or link to a table of contents like page.

### Example Next Link
[Next](./parsons/example1.html)
