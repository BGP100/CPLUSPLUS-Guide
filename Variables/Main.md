<a href="/Comments.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Variables/Multiple.md">Next &gt;</a>
<hr>
Variables are containers for storing data values.
<br>
In C++, there are different types of variables (defined with different keywords), for example:
<ul>
  <li><code>int</code> - stores integers (whole numbers), without decimals, such as 123 or -123</li>
  <li><code>double</code> - stores floating point numbers, with decimals, such as 19.99 or -19.99</li>
  <li><code>char</code> - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes</li>
  <li><code>string</code> - stores text, such as "Hello World". String values are surrounded by double quotes</li>
  <li><code>bool</code> - stores values with two states: true or false</li>
</ul>
<h1>Declaring (Creating) Variables</h1>
To create a variable, specify the type and assign it a value:
<pre>type variableName = value;</pre>
Where type is one of C++ types (such as int), and variableName is the name of the variable (such as x or myName). The equal sign is used to assign values to the variable.
<br>
To create a variable that should store a number, look at the following example:
<pre>
int myNum = 15;
cout &lt;&lt; myNum;
</pre>
You can also declare a variable without assigning the value, and assign the value later:
<pre>
int myNum;
myNum = 15;
cout &lt;&lt; myNum;
</pre>
Note that if you assign a new value to an existing variable, it will overwrite the previous value:
<pre>
int myNum = 15; // myNum is 15
myNum = 10; // Now myNum is 10
cout &lt;&lt; myNum; // Outputs 10
</pre>
<h1>Other Types</h1>
A demonstration of other data types:
<pre>
int myNum = 5;            // Integer (whole number without decimals)
double myFloatNum = 5.99; // Floating point number (with decimals)
char myLetter = 'D';      // Character
string myText = "Hello";  // String (text)
bool myBoolean = true;    // Boolean (true or false)
</pre>
You will learn more about the individual types in the Data Types chapter.
<h1>Display Variables</h1>
The cout object is used together with the << operator to display variables.
<br>
To combine both text and a variable, separate them with the << operator:
<pre>
int myAge = 35;
cout &lt;&lt; "I am " &lt;&lt; myAge &lt;&lt; " years old.";
</pre>
Add Variables Together
To add a variable to another variable, you can use the + operator:
<pre>
int x = 5;
int y = 6;
int sum = x + y;
cout &lt;&lt; sum;
</pre>
