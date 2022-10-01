<a href="/Conditions/Else-if.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Switch.md">Next &gt;</a>
<hr>
There is also a short-hand if else, which is known as the ternary operator because it consists of three operands. It can be used to replace multiple lines of code with a single line. It is often used to replace simple if else statements:
<pre>variable = (condition) ? expressionTrue : expressionFalse;</pre>
Instead of writing:
<pre>
int time = 20;
if (time &lt; 18) {
  cout &lt;&lt; "Good day.";
} else {
  cout &lt;&lt; "Good evening.";
}
</pre>
You can simply write:
<pre>
int time = 20;
string result = (time &lt; 18) ? "Good day." : "Good evening.";
cout &lt;&lt; result;
</pre>
