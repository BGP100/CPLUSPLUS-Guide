<a href="/Pointers/Create.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Pointers/Modify.md">Next &gt;</a>
<hr>
<h1>Get Memory Address and Value</h1>
In the example from the previous page, we used the pointer variable to get the memory address of a variable (used together with the &amp; reference operator). However, you can also use the pointer to get the value of the variable, by using the <code>*</code> operator (the dereference operator):
<pre>
string food = "Pizza"; // Variable declaration
string* ptr = &amp;food;   // Pointer declaration<br>
// Reference: Output the memory address of food with the pointer (0x6dfed4)
cout &lt;&lt; ptr &lt;&lt; "\n";<br>
// Dereference: Output the value of food with the pointer (Pizza)
cout &lt;&lt; *ptr &lt;&lt; "\n";
</pre>
Note that the <code>*</code> sign can be confusing here, as it does two different things in our code:
<ul>
  <li>When used in declaration (string* ptr), it creates a pointer variable.</li>
  <li>When not used in declaration, it act as a dereference operator.</li>
</ul>
