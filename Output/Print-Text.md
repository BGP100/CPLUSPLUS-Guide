<a href="/Syntax.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Output/New-Lines.md">Next &gt;</a>
<hr>
The cout object, together with the <code>&lt;&lt;</code> operator, is used to output values/print text:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World!";
  return 0;
}
</pre>
You can add as many cout objects as you want. However, note that it does not insert a new line at the end of the output:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World!";
  cout &lt;&lt; "I am learning C++";
  return 0;
}
</pre>
