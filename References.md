<a href="/Structures.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Pointers/Create.md">Next &gt;</a>
<hr>
<h1>Creating References</h1>
A reference variable is a "reference" to an existing variable, and it is created with the & operator:
<pre>
string food = "Pizza"; // food variable
string &amp;meal = food;   // reference to food
</pre>
Now, we can use either the variable name food or the reference name meal to refer to the food variable:
<pre>
string food = "Pizza";
string &amp;meal = food;<br>
cout &lt;&lt; food &lt;&lt; "\n";  // Outputs Pizza
cout &lt;&lt; meal &lt;&lt; "\n";  // Outputs Pizza
</pre>
<h1>Memory Address</h1>
In the example above, the & operator was used to create a reference variable. But it can also be used to get the memory address of a variable; which is the location of where the variable is stored on the computer.
<br>
When a variable is created in C++, a memory address is assigned to the variable. And when we assign a value to the variable, it is stored in this memory address.
<br>
To access it, use the & operator, and the result will represent where the variable is stored:
<pre>
string food = "Pizza";<br>
cout << &amp;food; // Outputs 0x6dfed4
</pre>
<b>Note:</b> The memory address is in hexadecimal form (0x..). Note that you may not get the same result in your program.
<br>
And why is it useful to know the memory address?
<br>
References and Pointers (which you will learn about in the next chapter) are important in C++, because they give you the ability to manipulate the data in the computer's memory - which can reduce the code and improve the performance.
<br>
These two features are one of the things that make C++ stand out from other programming languages, like Python and Java.
