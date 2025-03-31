---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: FOR loops
---
# Parsons Practice

## Parsons 1  
Re-arrange the blocks below: the code prints the 7 times table.
<div id="forloops-1-sortableTrash" class="sortable-code"></div> 
<div id="forloops-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="forloops-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="forloops-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "number = 7\n" +
    "for i in range(1, 13):\n" +
    "    result = number * i\n" +
    "    print(f&quot;{number} × {i} = {result}&quot;)\n" +
    "print(&quot;End of multiplication table&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "forloops-1-sortable",
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
  $("#forloops-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#forloops-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 2  
Re-arrange the blocks below: the code creates a list of fruits that have more than 5 letters in their name, and prints these out.
<div id="forloops-2-sortableTrash" class="sortable-code"></div> 
<div id="forloops-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="forloops-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="forloops-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "fruits = [&quot;apple&quot;, &quot;banana&quot;, &quot;cherry&quot;, &quot;kiwi&quot;, &quot;mango&quot;]\n" +
    "long_fruits = []\n" +
    "for fruit in fruits:\n" +
    "    if len(fruit) &gt; 5:\n" +
    "        long_fruits.append(fruit)\n" +
    "        \n" +
    "print(&quot;Fruits with more than 5 letters:&quot;, long_fruits)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "forloops-2-sortable",
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
  $("#forloops-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#forloops-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
## Parsons 3  
Re-arrange the blocks below: this counts the number of vowels in a given sentence.
<div id="forloops-3-sortableTrash" class="sortable-code"></div> 
<div id="forloops-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="forloops-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="forloops-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "sentence = &quot;Hello, World!&quot;\n" +
    "vowels = &quot;aeiouAEIOU&quot;\n" +
    "vowel_count = 0\n" +
    "for char in sentence:\n" +
    "    if char in vowels:\n" +
    "        vowel_count += 1\n" +
    "        print(f&quot;Found vowel: {char}&quot;)\n" +
    "        \n" +
    "print(f&quot;Total vowels found: {vowel_count}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "forloops-3-sortable",
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
  $("#forloops-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#forloops-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4 
Re-arrange the blocks below: this calculates and prints the factorial of a number.
<div id="forloops-4-sortableTrash" class="sortable-code"></div> 
<div id="forloops-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="forloops-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="forloops-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "number = 5\n" +
    "factorial = 1\n" +
    "for i in range(1, number + 1):\n" +
    "    factorial = factorial * i\n" +
    "    print(f&quot;After multiplying by {i}, factorial is {factorial}&quot;)\n" +
    "    \n" +
    "print(f&quot;{number}! = {factorial}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "forloops-4-sortable",
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
  $("#forloops-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#forloops-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 5  
Re-arrange the blocks below: this plays the game Fizzbuzz (look up this game if you arent familiar with it).
<div id="forloops-5-sortableTrash" class="sortable-code"></div> 
<div id="forloops-5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="forloops-5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="forloops-5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "for i in range(1, 21):\n" +
    "    if i % 3 == 0 and i % 5 == 0:\n" +
    "        print(&quot;FizzBuzz&quot;)\n" +
    "    elif i % 3 == 0:\n" +
    "        print(&quot;Fizz&quot;)\n" +
    "    elif i % 5 == 0:\n" +
    "        print(&quot;Buzz&quot;)\n" +
    "    else:\n" +
    "        print(i)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "forloops-5-sortable",
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
  $("#forloops-5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#forloops-5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
