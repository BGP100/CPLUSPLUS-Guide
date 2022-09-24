<a href="/Data-Types/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Data-Types/Booleans.md">Next &gt;</a>
<hr>
Use int when you need to store a whole number without decimals, like 35 or 1000, and float or double when you need a floating point number (with decimals), like 9.99 or 3.14515.
<pre>
int myNum = 1000;
cout &lt;&lt; myNum;
</pre>
<pre>
float myNum = 5.75;
cout &lt;&lt; myNum;
</pre>
<pre>
double myNum = 19.99;
cout &lt;&lt; myNum;
</pre>
<h1>Scientific Numbers</h1>
A floating point number can also be a scientific number with an "e" to indicate the power of 10:
<pre>
float f1 = 35e3;
double d1 = 12E4;
cout &lt;&lt; f1;
cout &lt;&lt; d1;
</pre>
