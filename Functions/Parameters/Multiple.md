<a href="/Functions/Parameters/Default.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters/Return.md">Next &gt;</a>
<hr>
Inside the function, you can add as many parameters as you want:
<pre>
void myFunction(string fname, int age) {
  cout &lt;&lt; fname &lt;&lt; " Refsnes. " &lt;&lt; age &lt;&lt; " years old. \n";
}<br>
int main() {
  myFunction("Liam", 3);
  myFunction("Jenny", 14);
  myFunction("Anja", 30);
  return 0;
}<br>
// Liam Refsnes. 3 years old.
// Jenny Refsnes. 14 years old.
// Anja Refsnes. 30 years old.
</pre>
Note that when you are working with multiple parameters, the function call must have the same number of arguments as there are parameters, and the arguments must be passed in the same order.
