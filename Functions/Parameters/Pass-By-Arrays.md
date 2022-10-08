<a href="/Functions/Parameters/Pass-By-Reference.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Overloading.md">Next &gt;</a>
<hr>
In the examples from the previous page, we used normal variables when we passed parameters to a function. You can also pass a reference to the function. This can be useful when you need to change the value of the arguments:
<pre>
void swapNums(int &amp;x, int &amp;y) {
  int z = x;
  x = y;
  y = z;
}<br>
int main() {
  int firstNum = 10;
  int secondNum = 20;<br>
  cout &lt;&lt; "Before swap: " &lt;&lt; "\n";
  cout &lt;&lt; firstNum &lt;&lt; secondNum &lt;&lt; "\n";<br>
  // Call the function, which will change the values of firstNum and secondNum
  swapNums(firstNum, secondNum);<br>
  cout &lt;&lt; "After swap: " &lt;&lt; "\n";
  cout &lt;&lt; firstNum &lt;&lt; secondNum &lt;&lt; "\n";<br>
  return 0;
}
</pre>
