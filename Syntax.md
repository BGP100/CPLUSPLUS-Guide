<a href="/Get-Started.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Output/Print-Text.md">Next &gt;</a>
<hr>
Let's break up the following code to understand it better:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
int main() {
  cout &lt;&lt; "Hello World!";
  return 0;
}
</pre>
<h1>Example explained</h1>
Line 1: <code>#include &lt;iostream&gt;</code> is a header file library that lets us work with input and output objects, such as cout (used in line 5). Header files add functionality to C++ programs.
<br>
Line 2: using namespace <code>std</code> means that we can use names for objects and variables from the standard library.
<br>
Don't worry if you don't understand how <code>#include &lt;iostream&gt;</code> and using namespace std works. Just think of it as something that (almost) always appears in your program.
<br>
Line 3: A blank line. C++ ignores white space. But we use it to make the code more readable.
<br>
Line 4: Another thing that always appear in a C++ program, is int main(). This is called a function. Any code inside its curly brackets <code>{}</code> will be executed.
<br>
Line 5: cout (pronounced "see-out") is an object used together with the insertion operator (<code>&lt;&lt;</code>) to output/print text. In our example it will output "Hello World".
<br>
<b>Note:</b> Every C++ statement ends with a semicolon <code>;</code>.
<br>
<b>Note:</b> The body of <code>int main()</code> could also been written as:
<pre>int main(){cout &lt;&lt; "Hello World!";return 0;}</pre>
<b>Remember:</b> The compiler ignores white spaces. However, multiple lines makes the code more readable.
<br>
Line 6: <code>return 0</code> ends the main function.
<br>
Line 7: Do not forget to add the closing curly bracket <code>}</code> to actually end the main function.
<h1>Omitting Namespace</h1>
You might see some C++ programs that runs without the standard namespace library. The using namespace std line can be omitted and replaced with the std keyword, followed by the :: operator for some objects:
<pre>
#include &lt;iostream&gt;<br>
int main() {
  std::cout &lt;&lt; "Hello World!";
  return 0;
}
</pre>
<b>Note:</b> It is up to you if you want to include the standard namespace library or not.
