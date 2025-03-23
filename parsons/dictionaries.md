---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Dictionaries
---
# Parsons Practice

## Parsons 1 (Dictionary)
Re-arrange the blocks below.

<div id="dict-1-sortableTrash" class="sortable-code"></div> 
<div id="dict-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "australian_capitals = {\n" +
    "    &quot;New South Wales&quot;: &quot;Sydney&quot;,\n" +
    "    &quot;Victoria&quot;: &quot;Melbourne&quot;,\n" +
    "}\n" +
    "print(australian_capitals[&quot;Victoria&quot;])";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-1-sortable",
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
  $("#dict-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Parsons 2 (Dictionary)
Re-arrange the blocks below: Create a student marks dictionary, add a new subject, update an existing mark, and print the final dictionary.

<div id="dict-2-sortableTrash" class="sortable-code"></div> 
<div id="dict-2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "student_marks = {&quot;Maths&quot;: 85, &quot;English&quot;: 75, &quot;Science&quot;: 90}\n" +
    "student_marks[&quot;History&quot;] = 82\n" +
    "student_marks[&quot;English&quot;] = 78\n" +
    "print(&quot;Final marks:&quot;, student_marks)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-2-sortable",
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
  $("#dict-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 3 (Dictionary)
Re-arrange the blocks below: Count the frequency of each word in a sentence.
<div id="dict-3-sortableTrash" class="sortable-code"></div> 
<div id="dict-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "sentence = &quot;the quick brown fox jumps over the lazy dog&quot;\n" +
    "words = sentence.split()\n" +
    "word_count = {}\n" +
    "for word in words:\n" +
    "    if word in word_count:\n" +
    "        word_count[word] = word_count[word] + 1\n" +
    "    else:\n" +
    "        word_count[word] = 1\n" +
    "print(word_count)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-3-sortable",
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
  $("#dict-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4 (Dictionary)
Re-arrange the blocks below: Create a dictionary of student ages and find the oldest student.
<div id="dict-4-sortableTrash" class="sortable-code"></div> 
<div id="dict-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "student_ages = {&quot;Alice&quot;: 16, &quot;Bob&quot;: 17, &quot;Charlie&quot;: 15}\n" +
    "oldest_age = 0\n" +
    "for age in student_ages.values():\n" +
    "    if age &gt; oldest_age:\n" +
    "        oldest_age = age\n" +
    "print(&quot;The oldest student is&quot;, oldest_age, &quot;years old&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-4-sortable",
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
  $("#dict-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 5 (Dictionary)
Re-arrange the blocks below: Dictionaries can be nested! Create a student information dictionary and print a specific detail.

<div id="dict-5-sortableTrash" class="sortable-code"></div> 
<div id="dict-5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "student = {\n" +
    "    &quot;name&quot;: &quot;Alice&quot;,\n" +
    "    &quot;details&quot;: {\n" +
    "        &quot;age&quot;: 16,\n" +
    "        &quot;grade&quot;: 11\n" +
    "    }\n" +
    "}\n" +
    "student_grade = student[&quot;details&quot;][&quot;grade&quot;]\n" +
    "print(&quot;Alice is in grade:&quot;, student_grade)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-5-sortable",
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
  $("#dict-5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 6 (Dictionary)
Re-arrange the blocks below:  Create a dictionary with students' names as keys and their test scores as values in a list, then calculate the average score for each student.

<div id="dict-6-sortableTrash" class="sortable-code"></div> 
<div id="dict-6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "students = {&quot;Alice&quot;: [85, 90, 78], &quot;Bob&quot;: [76, 88, 92], &quot;Charlie&quot;: [91, 84, 89]}\n" +
    "for student in students:\n" +
    "    scores = students[student]\n" +
    "    average = sum(scores) / len(scores)\n" +
    "    print(student + &quot;&#039;s average score:&quot;, average)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-6-sortable",
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
  $("#dict-6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 7 (Dictionary)
Re-arrange the blocks below: Compare two dictionaries of student scores from different tests and identify students who improved their scores.
<div id="dict-7-sortableTrash" class="sortable-code"></div> 
<div id="dict-7-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="dict-7-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="dict-7-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "test1_scores = {&quot;Alice&quot;: 85, &quot;Bob&quot;: 76, &quot;Charlie&quot;: 90, &quot;David&quot;: 82}\n" +
    "test2_scores = {&quot;Alice&quot;: 88, &quot;Bob&quot;: 72, &quot;Charlie&quot;: 95, &quot;David&quot;: 85}\n" +
    "improved_students = []\n" +
    "for student in test1_scores:\n" +
    "    if student in test2_scores:\n" +
    "        if test2_scores[student] &gt; test1_scores[student]:\n" +
    "            improved_students.append(student)\n" +
    "print(&quot;Students who improved:&quot;, improved_students)\n" +
    "print(&quot;Number of students who improved:&quot;, len(improved_students))";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "dict-7-sortable",
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
  $("#dict-7-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#dict-7-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
