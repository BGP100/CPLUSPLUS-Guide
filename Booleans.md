<a href="/Math.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Conditions/If.md">Next &gt;</a>
<hr>
Very often, in programming, you will need a data type that can only have one of two values, like:
<ul>
  <li>YES / NO</li>
  <li>ON / OFF</li>
  <li>TRUE / FALSE</li>
</ul>
For this, C++ has a bool data type, which can take the values true (1) or false (0).
<h1>Boolean Values</h1>
A boolean variable is declared with the bool keyword and can only take the values true or false:
<pre>
bool isCodingFun = true;
bool isFishTasty = false;
cout &lt;&lt; isCodingFun; // Outputs 1 (true)
cout &lt;&lt; isFishTasty; // Outputs 0 (false)
</pre>
From the example above, you can read that a true value returns 1, and false returns 0.
<h1>Boolean Expressions</h1>
A Boolean expression is a C++ expression that returns a boolean value: 1 (true) or 0 (false).
<br>
You can use a comparison operator, such as the greater than (>) operator to find out if an expression (or a variable) is true:
<pre>
int x = 10;
int y = 9;
cout &lt;&lt; (x &gt; y); // returns 1 (true), because 10 is higher than 9
</pre>
Or even easier:
<pre>cout &lt;&lt; (10 &gt; 9); // returns 1 (true), because 10 is higher than 9</pre>
In the examples below, we use the equal to (==) operator to evaluate an expression:
<pre>
int x = 10;
cout &lt;&lt; (x == 10); // returns 1 (true), because the value of x is equal to 10
</pre>
<pre>cout << (10 == 15); // returns 0 (false), because 10 is not equal to 15</pre>
