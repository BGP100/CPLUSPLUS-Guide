<a href="/Strings/User-Input.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Math.md">Next &gt;</a>
<hr>
You might see some C++ programs that runs without the standard namespace library. The using namespace std line can be omitted and replaced with the std keyword, followed by the <code>::</code> operator for string (and cout) objects:
<pre>
#include &lt;iostream&gt;
#include &lt;string&gt;<br>
int main() {
  std::string greeting = "Hello";
  std::cout &lt;&lt; greeting;
  return 0;
}
</pre>
