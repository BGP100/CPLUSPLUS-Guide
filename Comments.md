<a href="/Output/New-Lines.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Variables/Main.md">Next &gt;</a>
<hr>
Comments can be used to explain C++ code, and to make it more readable. It can also be used to prevent execution when testing alternative code. Comments can be singled-lined or multi-lined.
<h1>Single-line Comments</h1>
Single-line comments start with two forward slashes (<code>//</code>).
<br>
Any text between <code>//</code> and the end of the line is ignored by the compiler (will not be executed).
<br>
This example uses a single-line comment before a line of code:
<pre>
// This is a comment
cout &lt;&lt; "Hello World!";
</pre>
This example uses a single-line comment at the end of a line of code:
<pre>cout &lt;&lt; "Hello World!"; // This is a comment</pre>
<h1>Multi-line Comments</h1>
Multi-line comments start with <code>/*</code> and ends with <code>*/</code>.
<br>
Any text between <code>/*</code> and <code>*/</code> will be ignored by the compiler:
<pre>
/* The code below will print the words Hello World!
to the screen, and it is amazing */
cout &lt;&lt; "Hello World!";
</pre>
