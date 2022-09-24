<a href="/Data-Types/Characters.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Operators/Arithmetic.md">Next &gt;</a>
<hr>
The string type is used to store a sequence of characters (text). This is not a built-in type, but it behaves like one in its most basic usage. String values must be surrounded by double quotes:
<pre>
string greeting = "Hello";
cout &lt;&lt; greeting;
</pre>
To use strings, you must include an additional header file in the source code, the <string> library:
<pre>
// Include the string library
#include &lt;string&gt;<br>
// Create a string variable
string greeting = "Hello";<br>
// Output string value
cout &lt;&lt; greeting;
</pre>
