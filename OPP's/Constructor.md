# Constructor

- Constructor is get used for object instantiation.
- Constructor name must be same as class name
- Constructor should not declare any return type and returns no value.

eg.

~~~ java 
public class Student {

  String name;
  int rollNo;
  Date dob;

}

Student s1 = new Student();
s1.name = "Ashish Malikar";
~~~

## Parameterized constructor

We can pass paramater to constructor while object instatiation.

eg. 
~~~ java
public class Student {

  String name;
  int rollNo;
  Date dob;

  public Student (String name, int rollNo) {
    this.name = name;
    this.rollNo = rollNo;
  }
}

Student s2 = new Student("Ashish Malikar", 11);
~~~

## Constructor Overloading

Like method overloading constructor can be overload
We can declare multiple constructors but with different paramater signature.

eg.

~~~ java
public class Student {

  String name;
  int rollNo;

  public Student () {

  }

  public Student (String name) {
    this.name = name;
  }

  public Student (String name, int rollNo) {
    this.name = name;
    this.rollNo = rollNo;
  }
}
~~~

Note - Keyword this referse to class level variables.

### Using super Keyword

- "super" Keyword referse to parent object constructor.

eg. 
~~~ java
public class Person {
  String name;
  public Person (String name) {
    this.name = name;
  }
} 

public class Student extends Person{
  int rollNo;

  public Student (String name, int rollNo) {
    super(name);
    this.rollNo = rollNo;
  }

}
~~~

In above example, when calling constructor of Student that extends Person.
It makes call to super that is parent constructor, it means it will instantiate parent object first then child.































