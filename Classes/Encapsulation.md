<a href="/Classes/Specifiers.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Inheritance/Main.md">Next &gt;</a>
<hr>
The meaning of Encapsulation, is to make sure that "sensitive" data is hidden from users. To achieve this, you must declare class variables/attributes as private (cannot be accessed from outside the class). If you want others to read or modify the value of a private member, you can provide public get and set methods.
<h1>Access Private Members</h1>
To access a private attribute, use public "get" and "set" methods:
<pre>
#include &lt;iostream&gt;
using namespace std;<br>
class Employee {
  private:
    // Private attribute
    int salary;<br>
  public:
    // Setter
    void setSalary(int s) {
      salary = s;
    }
    // Getter
    int getSalary() {
      return salary;
    }
};<br>
int main() {
  Employee myObj;
  myObj.setSalary(50000);
  cout &lt;&lt; myObj.getSalary();
  return 0;
}
</pre>
<h2>Example explained</h2>
The salary attribute is private, which have restricted access.
<br>
The public setSalary() method takes a parameter (s) and assigns it to the salary attribute (salary = s).
<br>
The public getSalary() method returns the value of the private salary attribute.
<br>
Inside main(), we create an object of the Employee class. Now we can use the setSalary() method to set the value of the private attribute to 50000. Then we call the getSalary() method on the object to return the value.
<h1>Why Encapsulation?</h1>
<ul>
  <li>It is considered good practice to declare your class attributes as private (as often as you can). Encapsulation ensures better control of your data, because you (or others) can change one part of the code without affecting other parts</li>
  <li>Increased security of data</li>
</ul>
