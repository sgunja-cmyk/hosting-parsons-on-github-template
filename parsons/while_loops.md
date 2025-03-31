---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: WHILE loops
---
# Parsons Practice

## Parsons 1  
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


## Parsons 2 
Re-arrange the blocks below: it sets some variables, then allows the user 3 attempts to enter the correct password. If the user input is correct, access is granted. Otherwise, account is locked.

<div id="whileloops-2-sortableTrash" class="sortable-code"></div> 
<div id="whileloops-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="whileloops-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="whileloops-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "correct_password = &quot;secure123&quot;\n" +
    "user_input = &quot;&quot;\n" +
    "attempts = 0\n" +
    "while user_input != correct_password and attempts &lt; 3:\n" +
    "    user_input = input(&quot;Enter password: &quot;)\n" +
    "    attempts = attempts + 1\n" +
    "    \n" +
    "if user_input == correct_password:\n" +
    "    print(&quot;Access granted&quot;)\n" +
    "else:\n" +
    "    print(&quot;Account locked&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "whileloops-2-sortable",
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
  $("#whileloops-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#whileloops-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 3
Re-arrange the blocks below: this program sums numbers from 1 to 100.
<div id="whileloops-3-sortableTrash" class="sortable-code"></div> 
<div id="whileloops-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="whileloops-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="whileloops-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "total = 0\n" +
    "number = 1\n" +
    "while number &lt;= 100:\n" +
    "    total = total + number\n" +
    "    number = number + 1\n" +
    "    \n" +
    "print(&quot;Sum of numbers from 1 to 100:&quot;, total)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "whileloops-3-sortable",
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
  $("#whileloops-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#whileloops-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4
Re-arrange the blocks below: this program finds the highest value in a list of numbers

<div id="whileloops-4-sortableTrash" class="sortable-code"></div> 
<div id="whileloops-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="whileloops-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="whileloops-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "numbers = [15, 8, 42, 37, 29, 64, 18]\n" +
    "index = 0\n" +
    "highest = numbers[0]\n" +
    "while index &lt; len(numbers):\n" +
    "    if numbers[index] &gt; highest:\n" +
    "        highest = numbers[index]\n" +
    "    index = index + 1\n" +
    "    \n" +
    "print(&quot;The highest value is:&quot;, highest)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "whileloops-4-sortable",
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
  $("#whileloops-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#whileloops-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 5
Re-arrange the blocks below: this generates a random number for a number guessing game. The user has 5 attempts to guess a number between 1 and 20, and with each guess, they get feedback whether their guess is too low or too high. If they guess the secret number, the game shows their attempts and gives an appropriate message. If the number isnt guessed within 5 attempts, the user gets a message saying they lost.
<div id="whileloops-5-sortableTrash" class="sortable-code"></div> 
<div id="whileloops-5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="whileloops-5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="whileloops-5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import random\n" +
    "secret = random.randint(1, 20)\n" +
    "guess = 0\n" +
    "attempts = 0\n" +
    "while guess != secret and attempts &lt; 5:\n" +
    "    guess = int(input(&quot;Guess a number between 1 and 20: &quot;))\n" +
    "    attempts = attempts + 1\n" +
    "    if guess &lt; secret:\n" +
    "        print(&quot;Too low!&quot;)\n" +
    "    elif guess &gt; secret:\n" +
    "        print(&quot;Too high!&quot;)\n" +
    "        \n" +
    "if guess == secret:\n" +
    "    print(&quot;You won in&quot;, attempts, &quot;attempts!&quot;)\n" +
    "else:\n" +
    "    print(&quot;You lost! The number was&quot;, secret)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "whileloops-5-sortable",
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
  $("#whileloops-5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#whileloops-5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
