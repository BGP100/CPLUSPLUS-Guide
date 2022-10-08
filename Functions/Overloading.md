<a href="/Functions/Parameters/Pass-By-Arrays.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Recursion.md">Next &gt;</a>
<hr>
With function overloading, multiple functions can have the same name with different parameters:
<pre>
int myFunction(int x)
float myFunction(float x)
double myFunction(double x, double y)
</pre>
Consider the following example, which have two functions that add numbers of different type:
<pre>
int plusFuncInt(int x, int y) {
  return x + y;
}<br>
double plusFuncDouble(double x, double y) {
  return x + y;
}<br>
int main() {
  int myNum1 = plusFuncInt(8, 5);
  double myNum2 = plusFuncDouble(4.3, 6.26);
  cout &lt;&lt; "Int: " &lt;&lt; myNum1 &lt;&lt; "\n";
  cout &lt;&lt; "Double: " &lt;&lt; myNum2;
  return 0;
}
</pre>
Instead of defining two functions that should do the same thing, it is better to overload one.
<br>
In the example below, we overload the plusFunc function to work for both int and double:
<pre>
int plusFunc(int x, int y) {
  return x + y;
}<br>
double plusFunc(double x, double y) {
  return x + y;
}<br>
int main() {
  int myNum1 = plusFunc(8, 5);
  double myNum2 = plusFunc(4.3, 6.26);
  cout &lt;&lt; "Int: " &lt;&lt; myNum1 << "\n";
  cout &lt;&lt; "Double: " &lt;&lt; myNum2;
  return 0;
}
</pre>
<b>Note:</b> Multiple functions can have the same name as long as the number and/or type of parameters are different.
