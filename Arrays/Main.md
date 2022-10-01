<a href="/BreakAndContinue.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays/Loops.md">Next &gt;</a>
<hr>
Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.
<br>
To declare an array, define the variable type, specify the name of the array followed by square brackets and specify the number of elements it should store:
<pre>string cars[4];</pre>
We have now declared a variable that holds an array of four strings. To insert values to it, we can use an array literal - place the values in a comma-separated list, inside curly braces:
<pre>string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};</pre>
To create an array of three integers, you could write:
<pre>int myNum[3] = {10, 20, 30};</pre>
<h1>Access the Elements of an Array</h1>
You access an array element by referring to the index number inside square brackets [].
<br>
This statement accesses the value of the first element in cars:
<pre>
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
cout << cars[0];
// Outputs Volvo
</pre>
<b>Note:</b> Array indexes start with 0: [0] is the first element. [1] is the second element, etc.
<h1>Change an Array Element</h1>
To change the value of a specific element, refer to the index number:
<pre>cars[0] = "Opel";</pre>
<pre>
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
cars[0] = "Opel";
cout &lt; cars[0];
// Now outputs Opel instead of Volvo
</pre>
