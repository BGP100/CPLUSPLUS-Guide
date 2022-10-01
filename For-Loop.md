<a href="/While-Loop.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/BreakAndContinue.md">Next &gt;</a>
<hr>
When you know exactly how many times you want to loop through a block of code, use the for loop instead of a while loop:
<pre>
for (statement 1; statement 2; statement 3;) {
  // code block to be executed
}
</pre>
Statement 1 is executed (one time) before the execution of the code block.
<br>
Statement 2 defines the condition for executing the code block.
<br>
Statement 3 is executed (every time) after the code block has been executed.
<br>
The example below will print the numbers 0 to 4:
<pre>
for (int i = 0; i &lt; 5; i++) {
  cout &lt;&lt; i &lt;&lt; "\n";
}
</pre>
<h2>Example explained</h2>
Statement 1 sets a variable before the loop starts (int i = 0).
<br>
Statement 2 defines the condition for the loop to run (i must be less than 5). If the condition is true, the loop will start over again, if it is false, the loop will end.
<br>
Statement 3 increases a value (i++) each time the code block in the loop has been executed.
<h1>Another Example</h1>
This example will only print even values between 0 and 10:
<pre>
for (int i = 0; i <= 10; i = i + 2) {
  cout << i << "\n";
}
</pre>
