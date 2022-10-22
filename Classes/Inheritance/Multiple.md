<a href="/Classes/Inheritance/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Inheritance/Multiple.md">Next &gt;</a>
<hr>
A class can also be derived from more than one base class, using a comma-separated list:
<pre>
// Base class
class MyClass {
  public:
    void myFunction() {
      cout &lt;&lt; "Some content in parent class." ;
    }
};<br>
// Another base class
class MyOtherClass {
  public:
    void myOtherFunction() {
      cout &lt;&lt; "Some content in another class." ;
    }
};<br>
// Derived class
class MyChildClass: public MyClass, public MyOtherClass {
};<br>
int main() {
  MyChildClass myObj;
  myObj.myFunction();
  myObj.myOtherFunction();
  return 0;
}
</pre>
