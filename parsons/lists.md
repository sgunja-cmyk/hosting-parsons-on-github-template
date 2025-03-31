---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Lists
---
# Parsons Practice

## Parsons 1  
Re-arrange the blocks below: this prints the sum of a list of numbers.
<div id="lists-1-sortableTrash" class="sortable-code"></div> 
<div id="lists-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="lists-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="lists-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "numbers = [4, 7, 2, 9, 5, 1, 8]\n" +
    "total = 0\n" +
    "for num in numbers:\n" +
    "    total += num\n" +
    "print(&quot;List:&quot;, numbers)\n" +
    "print(&quot;Sum of all elements:&quot;, total)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "lists-1-sortable",
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
  $("#lists-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#lists-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Parsons 2  
Re-arrange the blocks below: this finds the maximum value from a list of numbers
<div id="lists-2-sortableTrash" class="sortable-code"></div> 
<div id="lists-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="lists-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="lists-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "scores = [85, 92, 78, 95, 88, 76, 90]\n" +
    "max_score = scores[0]\n" +
    "for score in scores:\n" +
    "    if score &gt; max_score:\n" +
    "        max_score = score\n" +
    "print(&quot;Scores:&quot;, scores)\n" +
    "print(&quot;Highest score:&quot;, max_score)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "lists-2-sortable",
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
  $("#lists-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#lists-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 3  
Re-arrange the blocks below: this finds the even numbers in a list of numbers, and appends each even number to a new list. The program then prints the original list and the new list of even numbers.

<div id="lists-3-sortableTrash" class="sortable-code"></div> 
<div id="lists-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="lists-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="lists-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "numbers = [11, 24, 35, 42, 59, 60, 77, 88]\n" +
    "even_numbers = []\n" +
    "for num in numbers:\n" +
    "    if num % 2 == 0:\n" +
    "        even_numbers.append(num)\n" +
    "print(&quot;Original list:&quot;, numbers)\n" +
    "print(&quot;Even numbers:&quot;, even_numbers)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "lists-3-sortable",
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
  $("#lists-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#lists-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Parsons 4 
Re-arrange the blocks below: this reverses a list of elements.
<div id="lists-4-sortableTrash" class="sortable-code"></div> 
<div id="lists-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="lists-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="lists-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "pets = [&quot;dog&quot;, &quot;cat&quot;, &quot;rabbit&quot;, &quot;hamster&quot;, &quot;fish&quot;]\n" +
    "reversed_pets = []\n" +
    "for i in range(len(pets) - 1, -1, -1):\n" +
    "    reversed_pets.append(pets[i])\n" +
    "print(&quot;Original list:&quot;, pets)\n" +
    "print(&quot;Reversed list:&quot;, reversed_pets)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "lists-4-sortable",
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
  $("#lists-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#lists-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 5  
Re-arrange the blocks below: this searches for an element within a list, and prints out if it was found. If its found, it also prints out the index number/position where it was found.

<div id="lists-5-sortableTrash" class="sortable-code"></div> 
<div id="lists-5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="lists-5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="lists-5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "fruits = [&quot;apple&quot;, &quot;banana&quot;, &quot;orange&quot;, &quot;grape&quot;, &quot;kiwi&quot;, &quot;mango&quot;]\n" +
    "search_item = &quot;orange&quot;\n" +
    "found = False\n" +
    "position = -1\n" +
    "for i in range(len(fruits)):\n" +
    "    if fruits[i] == search_item:\n" +
    "        found = True\n" +
    "        position = i\n" +
    "        break\n" +
    "if found:\n" +
    "    print(f&quot;{search_item} found at position {position}&quot;)\n" +
    "else:\n" +
    "    print(f&quot;{search_item} not found in the list&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "lists-5-sortable",
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
  $("#lists-5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#lists-5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
