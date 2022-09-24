<a href="/Variables/Constants.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Data-Types/Main.md">Next &gt;</a>
<hr>
You have already learned that cout is used to output (print) values. Now we will use cin to get user input.
<br>
cin is a predefined variable that reads data from the keyboard with the extraction operator (>>).
<br>
In the following example, the user can input a number, which is stored in the variable x. Then we print the value of x:
<pre>
int x; 
cout &lt;&lt; "Type a number: "; // Type a number and press enter
cin &gt;&gt; x; // Get user input from the keyboard
cout &lt;&lt; "Your number is: " << x; // Display the input value
</pre>
<b>Good To Know</b>
<br>
cout is pronounced "see-out". Used for output, and uses the insertion operator (<code>&lt;&lt;</code>)
<br>
cin is pronounced "see-in". Used for input, and uses the extraction operator (<code>&gt;&gt;</code>)
<h1>Creating a Simple Calculator</h1>
In this example, the user must input two numbers. Then we print the sum by calculating (adding) the two numbers:
<pre>
int x, y;
int sum;
cout &lt;&lt; "Type a number: ";
cin &gt;&gt; x;
cout &lt;&lt; "Type another number: ";
cin &gt;&gt; y;
sum = x + y;
cout &lt;&lt; "Sum is: " &lt;&lt; sum;
</pre>
There you go! You just built a basic calculator!
