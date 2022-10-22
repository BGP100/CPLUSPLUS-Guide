<a href="/Classes/Inheritance/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Inheritance/Multiple.md">Next &gt;</a>
<hr>
A class can also be derived from one class, which is already derived from another class.
<br>
In the following example, MyGrandChild is derived from class MyChild (which is derived from MyClass).
<pre>
// Base class (parent)
class MyClass {
  public:
    void myFunction() {
      cout &lt;&lt; "Some content in parent class." ;
    }
};<br>
// Derived class (child)
class MyChild: public MyClass {
};<br>
// Derived class (grandchild)
class MyGrandChild: public MyChild {
};<br>
int main() {
  MyGrandChild myObj;
  myObj.myFunction();
  return 0;
};
</pre>
