<a href="/Strings/Length.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Strings/User-Input.md">Next &gt;</a>
<hr>
You can access the characters in a string by referring to its index number inside square brackets [].
<br>
This example prints the first character in myString:
<pre>
string myString = "Hello";
cout &lt;&lt; myString[0];
// Outputs H
</pre>
<b>Note:</b> String indexes start with 0: <code>[0]</code> is the first character. <code>[1]</code> is the second character, etc.
<br>
This example prints the second character in myString:
<pre>
string myString = "Hello";
cout &lt;&lt; myString[1];
// Outputs e
</pre>
<h1>Change String Characters</h1>
To change the value of a specific character in a string, refer to the index number, and use single quotes:
<pre>
string myString = "Hello";
myString[0] = 'J';
cout &lt;&lt; myString;
// Outputs Jello instead of Hello
</pre>
