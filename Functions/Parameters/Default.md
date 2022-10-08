<a href="/Functions/Parameters/Arguments.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters/Multiple.md">Next &gt;</a>
<hr>
You can also use a default parameter value, by using the equals sign (=).
<br>
If we call the function without an argument, it uses the default value ("Norway"):
<pre>
void myFunction(string country = "Norway") {
  cout &lt;&lt; country &lt;&lt; "\n";
}<br>
int main() {
  myFunction("Sweden");
  myFunction("India");
  myFunction();
  myFunction("USA");
  return 0;
}<br>
// Sweden
// India
// Norway
// USA
</pre>
A parameter with a default value, is often known as an "optional parameter". From the example above, country is an optional parameter and "Norway" is the default value.
