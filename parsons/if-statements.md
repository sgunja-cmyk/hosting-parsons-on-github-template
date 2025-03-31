---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: IF statements
---
# Parsons Practice

## Parsons 1  
Re-arrange the blocks below: this calculates the grade, by checking the highest scores first.
<div id="if-1-sortableTrash" class="sortable-code"></div> 
<div id="if-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="if-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="if-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "score = int(input(&quot;Enter your exam score (0-100): &quot;))\n" +
    "if score &gt;= 90:\n" +
    "    grade = &quot;A&quot;\n" +
    "elif score &gt;= 80:\n" +
    "    grade = &quot;B&quot;\n" +
    "elif score &gt;= 70:\n" +
    "    grade = &quot;C&quot;\n" +
    "elif score &gt;= 50:\n" +
    "    grade = &quot;D&quot;\n" +
    "else:\n" +
    "    grade = &quot;F&quot;\n" +
    "print(f&quot;Your grade is: {grade}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "if-1-sortable",
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
  $("#if-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#if-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 2  
Re-arrange the blocks below: this gets input from the user and converts it to fahrenheit. Then, based on the temp (starting with the highest), it prints the most appropriate message to the user.

<div id="if-2-sortableTrash" class="sortable-code"></div> 
<div id="if-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="if-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="if-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "temp_c = float(input(&quot;Enter temperature in Celsius: &quot;))\n" +
    "temp_f = (temp_c * 9/5) + 32\n" +
    "print(f&quot;{temp_c}°C is equal to {temp_f}°F&quot;)\n" +
    "if temp_f &gt; 90:\n" +
    "    print(&quot;It&#039;s very hot! Stay hydrated.&quot;)\n" +
    "elif temp_f &gt; 70:\n" +
    "    print(&quot;Nice warm weather!&quot;)\n" +
    "elif temp_f &gt; 50:\n" +
    "    print(&quot;Moderate temperature. Bring a light jacket.&quot;)\n" +
    "elif temp_f &gt; 32:\n" +
    "    print(&quot;It&#039;s cold. Wear a coat.&quot;)\n" +
    "else:\n" +
    "    print(&quot;Freezing temperatures! Bundle up.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "if-2-sortable",
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
  $("#if-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#if-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 3  
Re-arrange the blocks below: this gets the age and day of the week, and then sets the base price. If the age is under 5, tickets are free. Under 18, tickets are the base price *0.7; Under 65, the tickets are base price *0.8, otherwise charge the base price. For tuesdays, tickets are half price. The price is then printed out.
<div id="if-3-sortableTrash" class="sortable-code"></div> 
<div id="if-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="if-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="if-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "age = int(input(&quot;Enter your age: &quot;))\n" +
    "day = input(&quot;Enter day of the week: &quot;).lower()\n" +
    "base_price = 12.00\n" +
    "if age &lt; 5:\n" +
    "    price = 0.00\n" +
    "elif age &lt; 18:\n" +
    "    price = base_price * 0.70\n" +
    "elif age &gt;= 65:\n" +
    "    price = base_price * 0.80\n" +
    "else:\n" +
    "    price = base_price\n" +
    "if day == &quot;tuesday&quot;:\n" +
    "    price = price * 0.50\n" +
    "print(f&quot;Your ticket price is: ${price:.2f}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "if-3-sortable",
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
  $("#if-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#if-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4 
Re-arrange the blocks below: gets age and whether user has a drivers license. if the age is over 18 and they have their license, they can drive on their own. If they are over 18 but no license.se they need to get a license. If they are over 16, they can drive with adult supervision. Otherwise, they are too young to drive.
<div id="if-4-sortableTrash" class="sortable-code"></div> 
<div id="if-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="if-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="if-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "age = int(input(&quot;Enter your age: &quot;))\n" +
    "has_license = input(&quot;Do you have a driver&#039;s license? (yes/no): &quot;).lower()\n" +
    "if age &gt;= 18:\n" +
    "    if has_license == &quot;yes&quot;:\n" +
    "        print(&quot;You can drive on your own.&quot;)\n" +
    "    else:\n" +
    "        print(&quot;You need to get a license first.&quot;)\n" +
    "else:\n" +
    "    if age &gt;= 16:\n" +
    "        print(&quot;You can drive with adult supervision.&quot;)\n" +
    "    else:\n" +
    "        print(&quot;You are too young to drive.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "if-4-sortable",
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
  $("#if-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#if-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

 
