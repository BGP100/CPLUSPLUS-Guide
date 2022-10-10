<a href="/Classes/OOP.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Methods.md">Next &gt;</a>
<hr>
C++ is an object-oriented programming language.
<br>
Everything in C++ is associated with classes and objects, along with its attributes and methods. For example: in real life, a car is an object. The car has attributes, such as weight and color, and methods, such as drive and brake.
<br>
Attributes and methods are basically variables and functions that belongs to the class. These are often referred to as "class members".
<br>
A class is a user-defined data type that we can use in our program, and it works as an object constructor, or a "blueprint" for creating objects.
<h1>Create a Class</h1>
To create a class, use the class keyword:
<pre>
class MyClass {      // The class
  public:            // Access specifier
    int myNum;       // Attribute (int variable)
    string myString; // Attribute (string variable)
};
</pre>
<h2>Example explained</h2>
<ul>
  <li>The class keyword is used to create a class called MyClass.</li>
  <li>The public keyword is an access specifier, which specifies that members (attributes and methods) of the class are accessible from outside the class. You will learn more about access specifiers later.</li>
  <li>Inside the class, there is an integer variable myNum and a string variable myString. When variables are declared within a class, they are called attributes.</li>
  <li>At last, end the class definition with a semicolon ;.</li>
</ul>
<h1>Create an Object</h1>
In C++, an object is created from a class. We have already created the class named MyClass, so now we can use this to create objects.
<br>
To create an object of MyClass, specify the class name, followed by the object name.
<br>
To access the class attributes (myNum and myString), use the dot syntax (.) on the object:
<pre>
class MyClass {      // The class
  public:            // Access specifier
    int myNum;       // Attribute (int variable)
    string myString; // Attribute (string variable)
};<br>
int main() {
  MyClass myObj;  // Create an object of MyClass<br>
  // Access attributes and set values
  myObj.myNum = 15; 
  myObj.myString = "Some text";<br>
  // Print attribute values
  cout &lt;&lt; myObj.myNum &lt;&lt; "\n";
  cout &lt;&lt; myObj.myString;
  return 0;
}
</pre>
<h1>Multiple Objects</h1>
You can create multiple objects of one class:
<pre>
// Create a Car class with some attributes
class Car {
  public:
    string brand;   
    string model;
    int year;
};<br>
int main() {
  // Create an object of Car
  Car carObj1;
  carObj1.brand = "BMW";
  carObj1.model = "X5";
  carObj1.year = 1999;<br>
  // Create another object of Car
  Car carObj2;
  carObj2.brand = "Ford";
  carObj2.model = "Mustang";
  carObj2.year = 1969;<br>
  // Print attribute values
  cout &lt;&lt; carObj1.brand &lt;&lt; " " &lt;&lt; carObj1.model &lt;&lt; " " &lt;&lt; carObj1.year &lt;&lt; "\n";
  cout &lt;&lt; carObj2.brand &lt;&lt; " " &lt;&lt; carObj2.model &lt;&lt; " " &lt;&lt; carObj2.year &lt;&lt; "\n";
  return 0;
}
