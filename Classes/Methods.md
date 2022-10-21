<a href="/Classes/Objects.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Constructors.md">Next &gt;</a>
<hr>
Methods are functions that belongs to the class.
<br>
There are two ways to define functions that belongs to a class:
<ul>
  <li>Inside class definition</li>
  <li>Outside class definition</li>
</ul>
In the following example, we define a function inside the class, and we name it "myMethod".
<br>
Note: You access methods just like you access attributes; by creating an object of the class and using the dot syntax (.):
<pre>
class MyClass {       // The class
  public:             // Access specifier
    void myMethod() { // Method/function defined inside the class
      cout &lt;&lt; "Hello World!";
    }
};<br>
int main() {
  MyClass myObj;    // Create an object of MyClass
  myObj.myMethod(); // Call the method
  return 0;
};
</pre>
To define a function outside the class definition, you have to declare it inside the class and then define it outside of the class. This is done by specifiying the name of the class, followed the scope resolution :: operator, followed by the name of the function:
<pre>
class MyClass {        // The class
  public:              // Access specifier
    void myMethod();   // Method/function declaration
};<br>
// Method/function definition outside the class
void MyClass::myMethod() {
  cout &lt;&lt; "Hello World!";
}<br>
int main() {
  MyClass myObj;     // Create an object of MyClass
  myObj.myMethod();  // Call the method
  return 0;
};
</pre>
Parameters
You can also add parameters:
<pre>
#include <iostream>
using namespace std;<br>
class Car {
  public:
    int speed(int maxSpeed);
};<br>
int Car::speed(int maxSpeed) {
  return maxSpeed;
};<br>
int main() {
  Car myObj; // Create an object of Car
  cout &lt;&lt; myObj.speed(200); // Call the method with an argument
  return 0;
};
</pre>
