<a href="/Variables/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Variables/Identifiers.md">Next &gt;</a>
<hr>
<h1>Declare Many Variables</h1>
To declare more than one variable of the same type, use a comma-separated list:
<pre>
int x = 5, y = 6, z = 50;
cout &lt;&lt; x + y + z;
</pre>
<h1>One Value to Multiple Variables</h1>
You can also assign the same value to multiple variables in one line:
<pre>
int x, y, z;
x = y = z = 50;
cout &lt;&lt; x + y + z;
</pre>
