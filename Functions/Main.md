<a href="/Pointers/Modify.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters/Arguments.md">Next &gt;</a>
<hr>
A function is a block of code which only runs when it is called.
<br>
You can pass data, known as parameters, into a function.
<br>
Functions are used to perform certain actions, and they are important for reusing code: Define the code once, and use it many times.
<h1>Create a Function</h1>
C++ provides some pre-defined functions, such as main(), which is used to execute code. But you can also create your own functions to perform certain actions.
<br>
To create (often referred to as declare) a function, specify the name of the function, followed by parentheses ():
<pre>
void myFunction() {
  // code to be executed
}
</pre>
<h2>Example Explained</h2>
<ul>
  <li>myFunction() is the name of the function</li>
  <li>void means that the function does not have a return value. You will learn more about return values later in the next chapter</li>
  <li>inside the function (the body), add code that defines what the function should do</li>
</ul>
<h1>Call a Function</h1>
Declared functions are not executed immediately. They are "saved for later use", and will be executed later, when they are called.
<br>
To call a function, write the function's name followed by two parentheses () and a semicolon ;
<br>
In the following example, myFunction() is used to print a text (the action), when it is called:
<pre>
// Create a function
void myFunction() {
  cout &lt;&lt; "I just got executed!";
}<br>
int main() {
  myFunction(); // call the function
  return 0;
}<br>
// Outputs "I just got executed!"
</pre>
A function can be called multiple times:
<pre>
void myFunction() {
  cout &lt;&lt; "I just got executed!\n";
}<br>
int main() {
  myFunction();
  myFunction();
  myFunction();
  return 0;
}<br>
// I just got executed!
// I just got executed!
// I just got executed!
</pre>
<h1>Function Declaration and Definition</h1>
A C++ function consist of two parts:
<ul>
  <li><b>Declaration:</b> the return type, the name of the function, and parameters (if any)</li>
  <li><b>Definition:</b> the body of the function (code to be executed)</li>
</ul>
<pre>
void myFunction() { // declaration
  // the body of the function (definition)
}
</pre>
<b>Note:</b> If a user-defined function, such as myFunction() is declared after the main() function, an error will occur:
<pre>
int main() {
  myFunction();
  return 0;
}<br>
void myFunction() {
  cout &lt;&lt; "I just got executed!";
}<br>
// Error
</pre>
However, it is possible to separate the declaration and the definition of the function - for code optimization.
<br>
You will often see C++ programs that have function declaration above main(), and function definition below main(). This will make the code better organized and easier to read:
<pre>
// Function declaration
void myFunction();<br>
// The main method
int main() {
  myFunction();  // call the function
  return 0;
}<br>
// Function definition
void myFunction() {
  cout &lt;&lt; "I just got executed!";
}
</pre>
