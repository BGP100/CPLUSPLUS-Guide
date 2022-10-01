<a href="/Arrays/Omit-Size.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays/Multidimensional.md">Next &gt;</a>
<hr>
A multi-dimensional array is an array of arrays.
<br>
To declare a multi-dimensional array, define the variable type, specify the name of the array followed by square brackets which specify how many elements the main array has, followed by another set of square brackets which indicates how many elements the sub-arrays have:
<pre>string letters[2][4];</pre>
As with ordinary arrays, you can insert values with an array literal - a comma-separated list inside curly braces. In a multi-dimensional array, each element in an array literal is another array literal.
<pre>
string letters[2][4] = {
  { "A", "B", "C", "D" },
  { "E", "F", "G", "H" }
};
</pre>
Each set of square brackets in an array declaration adds another dimension to an array. An array like the one above is said to have two dimensions.
<br>
Arrays can have any number of dimensions. The more dimensions an array has, the more complex the code becomes. The following array has three dimensions:
<pre>
string letters[2][2][2] = {
  {
    { "A", "B" },
    { "C", "D" }
  },
  {
    { "E", "F" },
    { "G", "H" }
  }
};
</pre>
<h1>Access the Elements of a Multi-Dimensional Array</h1>
To access an element of a multi-dimensional array, specify an index number in each of the array's dimensions.
<br>
This statement accesses the value of the element in the first row (0) and third column (2) of the letters array.
<pre>
string letters[2][4] = {
  { "A", "B", "C", "D" },
  { "E", "F", "G", "H" }
};<br>
cout &lt;&lt; letters[0][2];  // Outputs "C"
</pre>
Remember that: Array indexes start with 0: [0] is the first element. [1] is the second element, etc.
<h1>Change Elements in a Multi-Dimensional Array</h1>
To change the value of an element, refer to the index number of the element in each of the dimensions:
<pre>
string letters[2][4] = {
  { "A", "B", "C", "D" },
  { "E", "F", "G", "H" }
};
letters[0][0] = "Z";<br>
cout &lt;&lt; letters[0][0];  // Now outputs "Z" instead of "A"
</pre>
<h1>Loop Through a Multi-Dimensional Array</h1>
To loop through a multi-dimensional array, you need one loop for each of the array's dimensions.
<br>
The following example outputs all elements in the letters array:
<pre>
string letters[2][4] = {
  { "A", "B", "C", "D" },
  { "E", "F", "G", "H" }
};<br>
for(int i = 0; i &lt; 2; i++) {
  for(int j = 0; j &lt; 4; j++) {
    cout &lt;&lt; letters[i][j] &lt;&lt; "\n";
  }
}
</pre>
This example shows how to loop through a three-dimensional array:
<pre>
string letters[2][2][2] = {
  {
    { "A", "B" },
    { "C", "D" }
  },
  {
    { "E", "F" },
    { "G", "H" }
  }
};<br>
for(int i = 0; i &lt; 2; i++) {
  for(int j = 0; j &lt; 2; j++) {
    for(int k = 0; k &lt; 2; k++) {
      cout &lt;&lt; letters[i][j][k] &lt;&lt; "\n";
    }
  }
}
</pre>
<h1>Why Multi-Dimensional Arrays?</h1>
Multi-dimensional arrays are great at representing grids. This example shows a practical use for them. In the following example we use a multi-dimensional array to represent a small game of Battleship:
<pre>
// We put "1" to indicate there is a ship.
bool ships[4][4] = {
  { 0, 1, 1, 0 },
  { 0, 0, 0, 0 },
  { 0, 0, 1, 0 },
  { 0, 0, 1, 0 }
};<br>
// Keep track of how many hits the player has and how many turns they have played in these variables
int hits = 0;
int numberOfTurns = 0;<br>
// Allow the player to keep going until they have hit all four ships
while (hits &lt; 4) {
  int row, column;<br>
  cout &lt;&lt; "Selecting coordinates\n";<br>
  // Ask the player for a row
  cout &lt;&lt; "Choose a row number between 0 and 3: ";
  cin &gt;&gt; row;<br>
  // Ask the player for a column
  cout &lt;&lt; "Choose a column number between 0 and 3: ";
  cin &gt;&gt; column;<br>
  // Check if a ship exists in those coordinates
  if (ships[row][column]) {
    // If the player hit a ship, remove it by setting the value to zero.
    ships[row][column] = 0;<br>
    // Increase the hit counter
    hits++;<br>
    // Tell the player that they have hit a ship and how many ships are left
    cout &lt;&lt; "Hit! " &lt;&lt; (4-hits) &lt;&lt; " left.\n\n";
  } else {
    // Tell the player that they missed
    cout &lt;&lt; "Miss\n\n";
  }<br>
  // Count how many turns the player has taken
  numberOfTurns++;
}<br>
cout &lt;&lt; "Victory!\n";
cout &lt;&lt; "You won in " &lt;&lt; numberOfTurns &lt;&lt; " turns";
</pre>
