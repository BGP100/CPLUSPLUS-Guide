<a href="/Classes/Encapsulation.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Inheritance/Multilevel.md">Next &gt;</a>
<hr>
In C++, it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:
<ul>
  <li>derived class (child) - the class that inherits from another class</li>
  <li>base class (parent) - the class being inherited from another class</li>
</ul>
To inherit from a class, use the <code>:</code> symbol.
<br>
In the example below, the Car class (child) inherits the attributes and methods from the Vehicle class (parent):
<pre>
// Base class
class Vehicle {
  public:
    string brand = "Ford";
    void honk() {
      cout << "Tuut, tuut! \n" ;
    }
};<br>
// Derived class
class Car: public Vehicle {
  public:
    string model = "Mustang";
};<br>
int main() {
  Car myCar;
  myCar.honk();
  cout << myCar.brand + " " + myCar.model;
  return 0;
}
</pre>
<h1>Why And When To Use "Inheritance"?</h1>
<ul><li>It is useful for code reusability: reuse attributes and methods of an existing class when you create a new class.</li></ul>
