# OOPs

OOps concepts brings data and behavious at same one place called "Class".

OOPs is a programming paradigm based on conepts of "Object" that contain data and methods.

eg. 

~~~ java
public class Car {

  // data 
  private Engine engine;
  private Body body;

  // Behaviours or methods
  public void start () {
    // to do 
  }

  public void run () {
    // to do 
  }

  public void stop () {
    // to do 
  }

  public void horn () {
    // to do 
  }

}
~~~

## OOPs features:

1. Classes
2. Objects
3. Data Abstraction
4. Encapsulation
5. Inheritance
6. Polymorphism

### What is Class?

Class is real world entity which acts like blueprint of objects.
 
~~~ Java 
public class Student {
  String id;
  String course;
  int age;
  void enroll () {
    System.ou.println("Enrolling Student");
  }
} 
~~~ 

### What is an object?

Object can be seen as instance of a classs. We can create any number of instannce of the class.

~~~ java 
Student s1 = new Student();
Student s2 = new Student();

s1.enroll();
~~~

### What is Abstration?

Abstration is the proocess of show only relevent data and hide unneccesary details of the object from user.

In Java we can achive with two types

1. Interface
2. Abstract class.

#### Interface
- To achive total abstraction
- All the methods are declared as abstract only.

For example.

~~~ java 
public interface Car {
  public void changeGear();
  public void applyBreaks();
}
~~~



