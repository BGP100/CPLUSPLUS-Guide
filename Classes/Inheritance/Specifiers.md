<a href="/Classes/Inheritance/Multiple.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Polymorphism.md">Next &gt;</a>
<hr>
You learned from the Access Specifiers chapter that there are three specifiers available in C++. Until now, we have only used public (members of a class are accessible from outside the class) and private (members can only be accessed within the class). The third specifier, protected, is similar to private, but it can also be accessed in the inherited class:
<pre>
// Base class
class Employee {
  protected: // Protected access specifier
    int salary;
};<br>
// Derived class
class Programmer: public Employee {
  public:
    int bonus;
    void setSalary(int s) {
      salary = s;
    }
    int getSalary() {
      return salary;
    }
};<br>
int main() {
  Programmer myObj;
  myObj.setSalary(50000);
  myObj.bonus = 15000;
  cout &lt;&lt; "Salary: " &lt;&lt; myObj.getSalary() &lt;&lt; "\n";
  cout &lt;&lt; "Bonus: " &lt;&lt; myObj.bonus &lt;&lt; "\n";
  return 0;
}
</pre>
