<a href="/Conditions/Else.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Conditions/Shorthand-if-else.md">Next &gt;</a>
<hr>
Use the else if statement to specify a new condition if the first condition is false.
<pre>
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
</pre>
<pre>
int time = 22;
if (time &lt; 10) {
  cout &lt;&lt; "Good morning.";
} else if (time &lt; 20) {
  cout &lt;&lt; "Good day.";
} else {
  cout &lt;&lt; "Good evening.";
}
// Outputs "Good evening."
</pre>
<h2>Example explained</h2>
In the example above, time (22) is greater than 10, so the first condition is false. The next condition, in the else if statement, is also false, so we move on to the else condition since condition1 and condition2 is both false - and print to the screen "Good evening".
<br>
However, if the time was 14, our program would print "Good day."
