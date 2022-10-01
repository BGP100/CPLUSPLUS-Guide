<a href="/Conditions/If.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Conditions/Else-if.md">Next &gt;</a>
<hr>
Use the else statement to specify a block of code to be executed if the condition is false.
<pre>
if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
</pre>
<pre>
int time = 20;
if (time &lt; 18) {
  cout &lt;&lt; "Good day.";
} else {
  cout &lt;&lt; "Good evening.";
}
// Outputs "Good evening."
</pre>
<h2>Example explained</h2>
In the example above, time (20) is greater than 18, so the condition is false. Because of this, we move on to the else condition and print to the screen "Good evening". If the time was less than 18, the program would print "Good day".
