<a href="/Functions/Parameters/Multiple.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters/Pass-By-Reference.md">Next &gt;</a>
<hr>
The void keyword, used in the previous examples, indicates that the function should not return a value. If you want the function to return a value, you can use a data type (such as int, string, etc.) instead of void, and use the return keyword inside the function:
<pre>
int myFunction(int x) {
  return 5 + x;
}<br>
int main() {
  cout &lt;&lt; myFunction(3);
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
This example returns the sum of a function with two parameters:
<pre>
int myFunction(int x, int y) {
  return x + y;
}<br>
int main() {
  cout &lt;&lt; myFunction(5, 3);
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
You can also store the result in a variable:
<pre>
Example
int myFunction(int x, int y) {
  return x + y;
}<br>
int main() {
  int z = myFunction(5, 3);
  cout &lt;&lt; z;
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
