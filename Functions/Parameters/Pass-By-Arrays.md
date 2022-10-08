<a href="/Functions/Parameters/Pass-By-Reference.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Overloading.md">Next &gt;</a>
<hr>
You can also pass arrays to a function:
<pre>
void myFunction(int myNumbers[5]) {
  for (int i = 0; i &lt; 5; i++) {
    cout &lt;&lt; myNumbers[i] &lt;&lt; "\n";
  }
}<br>
int main() {
  int myNumbers[5] = {10, 20, 30, 40, 50};
  myFunction(myNumbers);
  return 0;
}
</pre>
