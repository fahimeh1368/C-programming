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


