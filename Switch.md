<a href="/Conditions/Shorthand-if-else.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/While-Loop.md">Next &gt;</a>
<hr>
Use the switch statement to select one of many code blocks to be executed.
<pre>
switch (expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
</pre>
This is how it works:
<ul>
  <li>The switch expression is evaluated once</li>
  <li>The value of the expression is compared with the values of each case</li>
  <li>If there is a match, the associated block of code is executed</li>
  <li>The break and default keywords are optional, and will be described later in this chapter</li>
</ul>
The example below uses the weekday number to calculate the weekday name:
<pre>
int day = 4;
switch (day) {
  case 1:
    cout &lt;&lt; "Monday";
    break;
  case 2:
    cout &lt;&lt; "Tuesday";
    break;
  case 3:
    cout &lt;&lt; "Wednesday";
    break;
  case 4:
    cout &lt;&lt; "Thursday";
    break;
  case 5:
    cout &lt;&lt; "Friday";
    break;
  case 6:
    cout &lt;&lt; "Saturday";
    break;
  case 7:
    cout &lt;&lt; "Sunday";
    break;
}
// Outputs "Thursday" (day 4)
</pre>
<h1>The break Keyword</h1>
When C++ reaches a break keyword, it breaks out of the switch block.
<br>
This will stop the execution of more code and case testing inside the block.
<br>
When a match is found, and the job is done, it's time for a break. There is no need for more testing.
<br>
A break can save a lot of execution time because it "ignores" the execution of all the rest of the code in the switch block.
<h1>The default Keyword</h1>
The default keyword specifies some code to run if there is no case match:
<pre>
int day = 4;
switch (day) {
  case 6:
    cout &lt;&lt; "Today is Saturday";
    break;
  case 7:
    cout &lt;&lt; "Today is Sunday";
    break;
  default:
    cout &lt;&lt; "Looking forward to the Weekend";
}
// Outputs "Looking forward to the Weekend"
</pre>
<b>Note:</b> The default keyword must be used as the last statement in the switch, and it does not need a break.
