# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?
The condition of occurring in several different forms.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.
Polymorphism is the ability of an object to take on many forms. The most common use of polymorphism in OOP occurs when a parent class reference is used to refer to a child class object. 
Any Java object that can pass more than one IS-A test is considered to be polymorphic.

3. What can we use to implement polymorphism in Java?
Abstract classes and interfaces.

4. How many 'forms' can an object take when using polymorphism?
An object can have multiple interfaces but can only  inherit from one other class.

5. Give an example of when you could use polymorphism.
Creating an interface called IConnect. The method `connect` connects devices to a network.
Desktop can be both a Desktop and an IConnect, so anything accepting IConnect can accept a Desktop. Therefore IConnect is passed into the ArrayList instead of specific devices. 

```java

private ArrayList<IConnect> devices; 

public Network(String name){
this.devices = new ArrayList<IConnect>();
this.name = name;
}

```



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?
A class that references one or more objects of other classes in instance variables. This allows you to model a has-a association between objects.

7. When would you use composition? Provide a simple example in Java.
```java
public class CPU extends Player {

private IStrategy strategy;

public CPU(IStrategy strategy) {
this.strategy = strategy;
}
```

8. What is/are the advantage(s) of using composition?
It allows reuse of existing code and a design based on object composition usually will have less classes
