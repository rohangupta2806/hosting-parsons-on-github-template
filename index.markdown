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

## Parsons 3: Temperature Conversion

Write code to convert either from Celsius to Kelvin or from Fahrenheit to Kelvin. You will take a string value to determine whether the input is Celsius or Fahrenheit. If the input string is not Celsius or Fahrenheit, print "Unknown Scale". 
The equation for converting from Celsius to Kelvin is: 


<div id="temperature-sortableTrash" class="sortable-code"></div> 
<div id="temperature-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="temperature-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="temperature-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "scale = &#039;celsius&#039;\n" +
    "temperature = 25\n" +
    "if scale == &#039;celsius&#039;:\n" +
    "    kelvin = temperature + 273.15\n" +
    "elif scale == &#039;fahrenheit&#039;:\n" +
    "    kelvin = (temperature + 459.67) * 5/9\n" +
    "else:\n" +
    "    print(&#039;Unknown scale&#039;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "temperature-sortable",
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
  $("#temperature-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#temperature-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Parsons 4: Factorial

<div id="factorial-sortableTrash" class="sortable-code"></div> 
<div id="factorial-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="factorial-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="factorial-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "result = 1\n" +
    "for i in range(1, 8):\n" +
    "    result *= i\n" +
    "print(f&#039;The result is {result}&#039;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "factorial-sortable",
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
  $("#factorial-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#factorial-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
