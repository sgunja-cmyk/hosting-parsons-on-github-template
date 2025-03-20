---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Functions
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

## Parsons 3 (Functions)
Rearrange the blocks below so the code works. This function calculates average with a list of numbers.

<div id="function-2-sortableTrash" class="sortable-code"></div> 
<div id="function-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="function-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="function-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def calculate_average(numbers):\n" +
    "    total = sum(numbers)\n" +
    "    count = len(numbers)\n" +
    "    average = total / count\n" +
    "    return average\n" +
    "numbers = [12, 45, 23, 67, 89, 34]\n" +
    "result = calculate_average(numbers)\n" +
    "print(f&quot;The average is: {result}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "function-2-sortable",
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
  $("#function-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#function-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4 (Functions)
Rearrange the blocks below so the code works. This function checks whether the password is valid or invalid, by first checking the length, and then the case.
<div id="function-3-sortableTrash" class="sortable-code"></div> 
<div id="function-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="function-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="function-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def is_valid_password(password):\n" +
    "    if len(password) &lt; 6:\n" +
    "        return False\n" +
    "    if password.islower():\n" +
    "        return False\n" +
    "    return True\n" +
    "password = input(&quot;Enter a password: &quot;)\n" +
    "if is_valid_password(password):\n" +
    "    print(&quot;Password is valid&quot;)\n" +
    "else:\n" +
    "    print(&quot;Password is invalid&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "function-3-sortable",
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
  $("#function-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#function-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 5 (Functions)
Rearrange the blocks below so the code works. This function takes a string as input, and returns the reversed string.
<div id="function-4-sortableTrash" class="sortable-code"></div> 
<div id="function-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="function-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="function-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def reverse_string(text):\n" +
    "    reversed_text = &quot;&quot;\n" +
    "    for char in text:\n" +
    "        reversed_text = char + reversed_text\n" +
    "    return reversed_text\n" +
    "message = input(&quot;Enter a word or phrase: &quot;)\n" +
    "result = reverse_string(message)\n" +
    "print(f&quot;Reversed: {result}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "function-4-sortable",
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
  $("#function-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#function-4-feedbackLink").click(function(event){ 
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
