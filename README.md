# C#-programming
In this project I want to practice C# and .Net features and learn more about that 

- properties</br>
public int number{set;get;}   ---> compiler create a private field ang getter and setter (we can check via comman "ildasm" for exe file of the project)

- Indexers</br>
Indexer make work with lists and dictionaries easier. Instead of setItem and getItem methods we can use indexer with this syntax:
pulic string this[string key]</br>
{</br>
get{return _dictionary[key]}</br>
set{_dictionary[key] = value}</br>
}</br>

For code reuse we can use inheritance(is a relationship) and composition(has a relationship)</br>

- Composition</br>
For implementing composition we should use the class as a private field and initialize it in the constroctor.(For example: Logger)</br>

Problems of inheritance:</br>
1- Easily abused by amateur designer</br>
2- Large hierarchies</br>
3- Fragility</br>
4-Tightly coupeling</br>

- Access Modifiers:
1-Public 
2-Private
3-Protected (Accessible from class and derived classes)
4-Internal (Accessible from the same assembly )
5-Protected Internal (Protected or Internal)

-Upcasting:</br>
There is not need to conversion </br>
Shape shape = circle</br>
after Upcasting both objects are refer to the same place</br>


- Downcasting:</br>
Circle circle2 = (Circle)shape
If we cast a object to another object that is not the parent calss we will get an error so we can use AS keyboard 
Car car = obj AS Car  (If it is not possible to cast car is null)</br>

- Reference types are stored in heap and Value types are stored in stack</br>
- Boxing</br>
The process of converting a value type instance to an object reference</br>
Example: object obj = 10 --> convert value type Number to Object type.</br>
- Unboxing</br>
Opposite of boxing</br>
Example: Object obj = 10     -> var number = (int)obj</br>
Using Generic list instead of ArrayList prevent performance penalty(Boxing and Unboxing)</br>
# Polymorphism

- Method Overriding:</br>
Modifing the implementation of an inherited method.We can Override the virtual methods of Parent class in the child class.</br>

- Abstract: </br>
If we have abstract method(which does not have declaration) the class of this method must be abstract.Abstract method must implemen in override methods in child class.</br>
Abstract classes can not be instantiated.</br>
When we want to force other developers to implement the specific design we must use abstract method. For example we want to foce developers to derived a class from the shape to implement the specific draw function we use abstaract method draw in shape.</br>
- Sealed class:</br>
There is not possible to derived a class from a sealed class. Using sealed class are faster in runtime because of some optimization. Using of the sealed are not recommende. String in c# is sealed class. With extension method can inherit from string.  
------------------------------------------------------------------------------------------


