<a href="/Strings/Access.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Strings/Omitting-Namespace.md">Next &gt;</a>
<hr>
It is possible to use the extraction operator >> on cin to display a string entered by a user:
<pre>
string firstName;
cout &lt;&lt; "Type your first name: ";
cin &gt;&gt; firstName; // get user input from the keyboard
cout &lt;&lt; "Your name is: " &lt;&lt; firstName;<br>
// Type your first name: John
// Your name is: John
</pre>
However, cin considers a space (whitespace, tabs, etc) as a terminating character, which means that it can only display a single word (even if you type many words):
<pre>
string fullName;
cout &lt;&lt; "Type your full name: ";
cin &gt;&gt; fullName;
cout &lt;&lt; "Your name is: " &lt;&lt; fullName;<br>
// Type your full name: John Doe
// Your name is: John
</pre>
From the example above, you would expect the program to print "John Doe", but it only prints "John".
<br>
That's why, when working with strings, we often use the getline() function to read a line of text. It takes cin as the first parameter, and the string variable as second:
<pre>
string fullName;
cout &lt;&lt; "Type your full name: ";
getline(cin, fullName);
cout &lt;&lt; "Your name is: " &lt;&lt; fullName;<br>
// Type your full name: John Doe
// Your name is: John Doe
</pre>
