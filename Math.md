<a href="/Strings/Omitting-Namespace.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Booleans.md">Next &gt;</a>
<hr>
C++ has many functions that allows you to perform mathematical tasks on numbers.
<h1>Max and min</h1>
The max(x,y) function can be used to find the highest value of x and y:
<pre>cout << max(5,10); // Outputs 10</pre>
And the min(x,y) function can be used to find the lowest value of x and y:
<pre>cout << min(5,10); // Outputs 5</pre>
<h1>&lt;cmath&gt; Header</h1>
Other functions, such as sqrt (square root), round (rounds a number) and log (natural logarithm), can be found in the &lt;cmath&gt; header file:
<pre>
// Include the cmath library
#include &lt;cmath&gt;<br>
cout &lt;&lt; sqrt(64);
cout &lt;&lt; round(2.6);
cout &lt;&lt; log(2);
</pre>
