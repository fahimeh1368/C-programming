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
1- Easily abused by amateur designer
2- Large hierarchies
3- Fragility
4-Tightly coupeling

