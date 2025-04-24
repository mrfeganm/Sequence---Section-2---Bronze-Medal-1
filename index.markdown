---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

## Sequence - Section 2 - Bronze Medal 1
Re-arrange the blocks below.

<div id="bronze-medal-challenge-say-my-name-sortableTrash" class="sortable-code"></div> 
<div id="bronze-medal-challenge-say-my-name-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="bronze-medal-challenge-say-my-name-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="bronze-medal-challenge-say-my-name-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#Bronze medal challenge: Say my name\n" +
    "first_name = input(&#039;Enter your first name&#039;)\n" +
    "second_name = input(&#039;Enter your second name&#039;)\n" +
    "print(&#039;Hello&#039;)\n" +
    "print(first_name)\n" +
    "print(second_name)\n" +
    "print(&#039;Nice to meet you&#039;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "bronze-medal-challenge-say-my-name-sortable",
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
  $("#bronze-medal-challenge-say-my-name-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#bronze-medal-challenge-say-my-name-feedbackLink").click(function(event){ 
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
