<a href="/Arrays/Get-Size.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures.md">Next &gt;</a>
<hr>
Structures (also called structs) are a way to group several related variables into one place. Each variable in the structure is known as a member of the structure.
<br>
Unlike an array, a structure can contain many different data types (int, string, bool, etc.).
<h1>Create a Structure</h1>
To create a structure, use the struct keyword and declare each of its members inside curly braces.
<br>
After the declaration, specify the name of the structure variable (myStructure in the example below):
<pre>
struct {           // Structure declaration
  int myNum;       // Member (int variable)
  string myString; // Member (string variable)
} myStructure;     // Structure variable
</pre>
<h1>Access Structure Members</h1>
To access members of a structure, use the dot syntax (.):
<pre>
// Create a structure variable called myStructure
struct {
  int myNum;
  string myString;
} myStructure;<br>
// Assign values to members of myStructure
myStructure.myNum = 1;
myStructure.myString = "Hello World!";<br>
// Print members of myStructure
cout &lt;&lt; myStructure.myNum &lt;&lt; "\n";
cout &lt;&lt; myStructure.myString &lt;&lt; "\n";
</pre>
<h1>One Structure in Multiple Variables</h1>
You can use a comma (,) to use one structure in many variables:
<pre>
struct {
  int myNum;
  string myString;
} myStruct1, myStruct2, myStruct3; // Multiple structure variables separated with commas
</pre>
This example shows how to use a structure in two different variables:
<pre>
struct {
  string brand;
  string model;
  int year;
} myCar1, myCar2; // We can add variables by separating them with a comma here<br>
// Put data into the first structure
myCar1.brand = "BMW";
myCar1.model = "X5";
myCar1.year = 1999;<br>
// Put data into the second structure
myCar2.brand = "Ford";
myCar2.model = "Mustang";
myCar2.year = 1969;<br>
// Print the structure members
cout &lt;&lt; myCar1.brand &lt;&lt; " " &lt;&lt; myCar1.model &lt;&lt; " " &lt;&lt; myCar1.year &lt;&lt; "\n";
cout &lt;&lt; myCar2.brand &lt;&lt; " " &lt;&lt; myCar2.model &lt;&lt; " " &lt;&lt; myCar2.year &lt;&lt; "\n";
</pre>
<h1>Named Structures</h1>
By giving a name to the structure, you can treat it as a data type. This means that you can create variables with this structure anywhere in the program at any time.
<br>
To create a named structure, put the name of the structure right after the struct keyword:
<pre>
struct myDataType { // This structure is named "myDataType"
  int myNum;
  string myString;
};
</pre>
To declare a variable that uses the structure, use the name of the structure as the data type of the variable:
<pre>myDataType myVar;</pre>
<pre>
// Declare a structure named "car"
struct car {
  string brand;
  string model;
  int year;
};<br>
int main() {
  // Create a car structure and store it in myCar1;
  car myCar1;
  myCar1.brand = "BMW";
  myCar1.model = "X5";
  myCar1.year = 1999;<br>
  // Create another car structure and store it in myCar2;
  car myCar2;
  myCar2.brand = "Ford";
  myCar2.model = "Mustang";
  myCar2.year = 1969;<br>
  // Print the structure members
  cout &lt;&lt; myCar1.brand &lt;&lt; " " &lt;&lt; myCar1.model &lt;&lt; " " &lt;&lt; myCar1.year &lt;&lt; "\n";
  cout &lt;&lt; myCar2.brand &lt;&lt; " " &lt;&lt; myCar2.model &lt;&lt; " " &lt;&lt; myCar2.year &lt;&lt; "\n";<br>
  return 0;
}
</pre>
