<a href="/References.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Pointers/Deferencing.md">Next &gt;</a>
<hr>
You learned from the previous chapter, that we can get the memory address of a variable by using the & operator:
<pre>
string food = "Pizza"; // A food variable of type string<br>
cout &lt;&lt; food;  // Outputs the value of food (Pizza)
cout &lt;&lt; &amp;food; // Outputs the memory address of food (0x6dfed4)
</pre>
A pointer however, is a variable that stores the memory address as its value.
<br>
A pointer variable points to a data type (like int or string) of the same type, and is created with the * operator. The address of the variable you're working with is assigned to the pointer:
<pre>
string food = "Pizza"; // A food variable of type string
string* ptr = &amp;food; // A pointer variable, with the name ptr, that stores the address of food<br>
// Output the value of food (Pizza)
cout &lt;&lt; food &lt;&lt; "\n";<br>
// Output the memory address of food (0x6dfed4)
cout &lt;&lt; &amp;food &lt;&lt; "\n";<br>
// Output the memory address of food with the pointer (0x6dfed4)
cout &lt;&lt; ptr &lt;&lt; "\n";
</pre>
<h2>Example explained</h2>
Create a pointer variable with the name ptr, that points to a string variable, by using the asterisk sign * (string* ptr). Note that the type of the pointer has to match the type of the variable you're working with.
<br>
Use the & operator to store the memory address of the variable called food, and assign it to the pointer.
<br>
Now, ptr holds the value of food's memory address.
<br>
<b>Tip:</b> There are three ways to declare pointer variables, but the first way is preferred:
<pre>
string* mystring; // Preferred
string *mystring;
string * mystring;
</pre>
