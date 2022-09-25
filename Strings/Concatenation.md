<a href="/Operators/Logical.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Strings/Concatenation.md">Next &gt;</a>
<hr>
The <code>+</code> operator can be used between strings to add them together to make a new string. This is called concatenation:
<pre>
string firstName = "John ";
string lastName = "Doe";
string fullName = firstName + lastName;
cout &lt;&lt; fullName;
</pre>
In the example above, we added a space after firstName to create a space between John and Doe on output. However, you could also add a space with quotes (<code>" "</code> or <code>' '</code>):
<pre>
string firstName = "John";
string lastName = "Doe";
string fullName = firstName + " " + lastName;
cout &lt;&lt; fullName;
</pre>
<h1>Append</h1>
A string in C++ is actually an object, which contain functions that can perform certain operations on strings. For example, you can also concatenate strings with the <code>append()</code> function:
<pre>
string firstName = "John ";
string lastName = "Doe";
string fullName = firstName.append(lastName);
cout &lt;&lt; fullName;
</pre>
