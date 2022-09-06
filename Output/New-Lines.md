<a href="/Output/Print-Text.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Comments.md">Next &gt;</a>
<hr>
To insert a new line, you can use the \n character:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World! \n";
  cout &lt;&lt; "I am learning C++";
  return 0;
}
</pre>
<b>Tip:</b> Two <code>\n</code> characters after each other will create a blank line:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World! \n\n";
  cout &lt;&lt; "I am learning C++";
  return 0;
}
</pre>
Another way to insert a new line, is with the endl manipulator:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World!" &lt;&lt; endl;
  cout &lt;&lt; "I am learning C++";
  return 0;
}
</pre>
Both <code>\n</code> and endl are used to break lines. However, <code>\n</code> is most used.
<h1>What is <code>\n</code> exactly?</h1>
The newline character (<code>\n</code>) is called an escape sequence, and it forces the cursor to change its position to the beginning of the next line on the screen. This results in a new line.
<br>
Examples of other valid escape sequences are:
<table>
  <tr>
    <th>Escape Sequence</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>\t</code></td>
    <td>Creates a horizontal tab</td>
  </tr>
  <tr>
    <td><code>\\</code></td>
    <td>Inserts a backslash character (<code>\</code>)</td>
  </tr>
  <tr>
    <td><code>\"</code> or <code>\'</code></td>
    <td>Inserts the quotes character</td>
  </tr>
</table>
