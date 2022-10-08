<a href="/Functions/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters/Default.md">Next &gt;</a>
<hr>
Information can be passed to functions as a parameter. Parameters act as variables inside the function.
<br>
Parameters are specified after the function name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma:
<pre>
void functionName(parameter1, parameter2, parameter3) {
  // code to be executed
}
</pre>
The following example has a function that takes a string called fname as parameter. When the function is called, we pass along a first name, which is used inside the function to print the full name:
<pre>
void myFunction(string fname) {
  cout << fname << " Refsnes\n";
}<br>
int main() {
  myFunction("Liam");
  myFunction("Jenny");
  myFunction("Anja");
  return 0;
}<br>
// Liam Refsnes
// Jenny Refsnes
// Anja Refsnes
</pre>
