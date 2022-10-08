<a href="/Pointers/Deferencing.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Main.md">Next &gt;</a>
<hr>
You can also change the pointer's value. But note that this will also change the value of the original variable:
<pre>
string food = "Pizza";
string* ptr = &amp;food;<br>
// Output the value of food (Pizza)
cout &lt;&lt; food &lt;&lt; "\n";<br>
// Output the memory address of food (0x6dfed4)
cout &lt;&lt; &food &lt;&lt; "\n";<br>
// Access the memory address of food and output its value (Pizza)
cout &lt;&lt; *ptr &lt;&lt; "\n";<br>
// Change the value of the pointer
*ptr = "Hamburger";<br>
// Output the new value of the pointer (Hamburger)
cout &lt;&lt; *ptr &lt;&lt; "\n";<br>
// Output the new value of the food variable (Hamburger)
cout &lt;&lt; food &lt;&lt; "\n";
</pre>
