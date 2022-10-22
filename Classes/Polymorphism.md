<a href="/Classes/Inheritance/Specifiers.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Files.md">Next &gt;</a>
<hr>
Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.
<br>
Like we specified in the previous chapter; Inheritance lets us inherit attributes and methods from another class. Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways.
<br>
For example, think of a base class called Animal that has a method called animalSound(). Derived classes of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.):
<pre>
// Base class
class Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The animal makes a sound \n";
    }
};<br>
// Derived class
class Pig : public Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The pig says: wee wee \n";
    }
};<br>
// Derived class
class Dog : public Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The dog says: bow wow \n";
    }
};
</pre>
Remember from the Inheritance chapter that we use the : symbol to inherit from a class.
<br>
Now we can create Pig and Dog objects and override the animalSound() method:
<pre>
// Base class
class Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The animal makes a sound \n";
    }
};<br>
// Derived class
class Pig : public Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The pig says: wee wee \n";
    }
};<br>
// Derived class
class Dog : public Animal {
  public:
    void animalSound() {
      cout &lt;&lt; "The dog says: bow wow \n";
    }
};<br>
int main() {
  Animal myAnimal;
  Pig myPig;
  Dog myDog;<br>
  myAnimal.animalSound();
  myPig.animalSound();
  myDog.animalSound();
  return 0;
}
</pre>
<h1>Why And When To Use "Inheritance" and "Polymorphism"?</h1>
<ul><li>It is useful for code reusability: reuse attributes and methods of an existing class when you create a new class.</li></ul>
