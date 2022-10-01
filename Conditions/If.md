<a href="/Booleans.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Conditions/Else.md">Next &gt;</a>
<hr>
C++ supports the usual logical conditions from mathematics:
<ul>
  <li>Less than: a &lt; b</li>
  <li>Less than or equal to: a &lt;= b</li>
  <li>Greater than: a &gt; b</li>
  <li>Greater than or equal to: a &gt;= b</li>
  <li>Equal to a == b</li>
  <li>Not Equal to: a != b</li>
</ul>
You can use these conditions to perform different actions for different decisions.
<br>
C++ has the following conditional statements:
<ul>
  <li>Use if to specify a block of code to be executed, if a specified condition is true</li>
  <li>Use else to specify a block of code to be executed, if the same condition is false</li>
  <li>Use else if to specify a new condition to test, if the first condition is false</li>
  <li>Use switch to specify many alternative blocks of code to be executed</li>
</ul>
<h1>The if Statement</h1>
Use the if statement to specify a block of C++ code to be executed if a condition is true.
<pre>
if (condition) {
  // block of code to be executed if the condition is true
}
</pre>
Note that if is in lowercase letters. Uppercase letters (If or IF) will generate an error.
<br>
In the example below, we test two values to find out if 20 is greater than 18. If the condition is true, print some text:
<pre>
if (20 &gt; 18) {
  cout &lt;&lt; "20 is greater than 18";
}
</pre>
We can also test variables:
<pre>
int x = 20;
int y = 18;
if (x &gt; y) {
  cout &lt;&lt; "x is greater than y";
}
</pre>
<h2>Example explained</h2>
In the example above we use two variables, x and y, to test whether x is greater than y (using the > operator). As x is 20, and y is 18, and we know that 20 is greater than 18, we print to the screen that "x is greater than y".
