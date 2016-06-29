---
title: Subclassing and Interfaces
type: Homework
duration: "1:00"
creator:
    name: Charlie Drews
    city: NYC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Subclassing, Abstract Classes, and Interfaces

> ***Note:*** _You can discuss with classmates, but everyone must submit their own answers_

## Exercise

#### Requirements

- Fork this repo, then add your answers direcly to this **readme.md** file
  - After forking, you can clone, edit the readme in the text editor of your choice, and push back to Github...
  - Or, you can edit the readme [right from the browser](https://help.github.com/articles/editing-files-in-your-repository/)
- After adding your answers, submit a **pull request**

#### Questions

1. What is the difference between *member variables* (also called *instance variables*) and *class variables* (w/ keyword `static`)? Which can be accessed without creating an instance of the class?

-Member variables are shared among all members of a class, instance variables are for each instance of a class. Member variables can be created without making an instance of the class.

2. Does it make sense to write  *getter* and *setter* methods for a `public` member variable? What about `private` variables?

-Public member variables are already accessible from outside a class. It makes sense for private variables.

3. What are some benefits of making member variables `private`?

-It can't be accessed from outside the class

4. If class A extends class B, which is the super class and which is the sub class? Which would you call parent, and which would you call child?

-B is the upser class and A is the subclass. B is the parent and A is the child.

5. What does it mean for a class to *inherit* methods and/or variables from its parent class?

-A child class assumes properties from its parent class.

6. Consider the following code, where class Refrigerator extends class Appliance, and `getTemperature()` is a method in Refrigertor, but NOT in Appliance:
  ```
  Appliance myAppliance = new Refrigerator();
  double temperature = myAppliance.getTemperature();
  ```
  Why will this call to `getTemperature()` cause an error? How will *casting* help solve this issue?
  
  -getTemperature() is not a method of the Appliance class. Casting myAppliance to the Refrigerator class treats it as a Refrigerator.

7. In a normal class (also called a *concrete* class), do you need to *implement* all of the methods, or can your simply *declare* some? What about in an `abstract` class?

-You don't have to implement all methods in a concrete class. In an abstract class, you have to implement them for all subclasses.

8. What about an `interface`? Can you implement any methods in an interface? Can you declare methods in an interface?

-Interface lets you declare methods but you can choose how and where to implement them.

9. Can you create an instance of an `abstract` class? Also, look up the Java keyword `final` and see if you can explain why a class CANNOT be both `abstract` and `final`.

-You can't make an instance of an abstract class. A class cannot be both abstract and final because an abstract is a class that is incomplete and yet to be fully defined, but a final class is fully defined.

10. What happens when a method *overrides* another method? If a parent and child class have methods with the same name, when you call that method on an instance of the child class, which implementation of the method will be executed?

-Override is when a method in a subclass is executed over a method in the superclass. The child class's method will be executedd

11. What is the relationship between `List`, `LinkedList`, and `ArrayList`? Why do we call a method *polymorphic* if it takes an input of type `List` rather than an input of type `LinkedList` or `Arraylist`, and why is that useful?

-LinkedList and ArrayList are subclasses of the List class. It's polymorphic because it can take an input of List or any of its subclasses. It's useful because it gives you flexibility over which type you can use.

#### Deliverable

This file, with your answers added

## Additional Resources

Refer to the [Classes lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/classes-lesson), the [Subclassing lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/subclasses-lesson), and the [Interfaces & Abstract Classes lesson](https://github.com/ga-adi-nyc/Course-Materials/tree/master/lessons/java-essentials/interfaces-and-abstract-classes-lesson).

Feel free to google these concepts as well. There are plenty of Java tutorial websites and StackOverflow posts that can help you. But be sure to write up your answers in your own words - copying and pasting some text does NOT help you actually learn!
