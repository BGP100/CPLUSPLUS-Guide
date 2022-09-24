<a href="/Variables/Multiple.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Variables/Constants.md">Next &gt;</a>
<hr>
All C++ variables must be identified with unique names.
<br>
These unique names are called identifiers.
<br>
Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
<br>
<b>Note:</b> It is recommended to use descriptive names in order to create understandable and maintainable code:
<pre>
// Good
int minutesPerHour = 60;<br>
// OK, but not so easy to understand what m actually is
int m = 60;
</pre>
The general rules for naming variables are:
<ul>
  <li>Names can contain letters, digits and underscores</li>
  <li>Names must begin with a letter or an underscore (<code>_</code>)</li>
  <li>Names are case sensitive (<code>myVar</code> and <code>myvar</code> are different variables)</li>
  <li>Names cannot contain whitespaces or special characters like <code>!</code>, <code>#</code>, <code>%</code>, etc.</li>
  <li>Reserved words (like C++ keywords, such as <code>int</code>) cannot be used as names</li>
</ul>
