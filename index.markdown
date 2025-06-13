---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Multiple Parson's Problems on One Page
---
# Parsons Practice

## Parsons 1 (Leap Year)
Re-arrange the blocks below to determine if a year is a leap year or not:

<div id="leap_year-sortableTrash" class="sortable-code"></div> 
<div id="leap_year-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="leap_year-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="leap_year-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "year = 2004\n" +
    "leap_year = False\n" +
    "if year % 4 == 0:\n" +
    "    print(year)\n" +
    "    leap_year = True\n" +
    "    if year % 100 == 0:\n" +
    "        if year % 400 != 0:\n" +
    "            leap_year = False\n" +
    "if leap_year: \n" +
    "	print(&quot;leap year&quot;)\n" +
    "else:\n" +
    "	print(&quot;not a leap year&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "leap_year-sortable",
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
  $("#leap_year-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#leap_year-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Parsons 2 (If Elif Structure)
Write a program that identifies the compound based on the chemical structure and gives the common name. Options are H2O (Water), CO2 (Carbon Dioxide) and CH3 (Methane).

<div id="if_elif-sortableTrash" class="sortable-code"></div> 
<div id="if_elif-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="if_elif-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="if_elif-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "compound = &#039;H2O&#039;\n" +
    "if compound == &#039;H2O&#039;:\n" +
    "    print(&#039;water&#039;)\n" +
    "elif compound == &#039;CO2&#039;:\n" +
    "    print(&#039;carbon dioxide&#039;)\n" +
    "elif compound == &#039;CH3&#039;:\n" +
    "    print(&#039;methane&#039;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "if_elif-sortable",
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
  $("#if_elif-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#if_elif-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
