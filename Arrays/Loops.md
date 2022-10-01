<a href="/Arrays/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays/Omit-Size.md">Next &gt;</a>
<hr>
You can loop through the array elements with the for loop.
<br>
The following example outputs all elements in the cars array:
<pre>
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
for (int i = 0; i &lt; 4; i++) {
  cout &lt;&lt; cars[i] &lt;&lt; "\n";
}
</pre>
The following example outputs the index of each element together with its value:
<pre>
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
for (int i = 0; i &lt; 4; i++) {
  cout &lt;&lt; i &lt;&lt; ": " &lt;&lt; cars[i] &lt;&lt; "\n";
}
</pre>
