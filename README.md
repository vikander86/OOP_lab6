# OOP_lab6, Jan Schmidt Jensen

Revisiting lab2 ATM, implement SOLID principles

## Single Responsibility Principle

My first ATM was handling way too many actions which violates the SRP, it would be better to devide the code into multiple classes(interfaces), such as one for transactions and one for maintenance and one for accounts. By splitting up the code like this, the classes are now corresponding to the single responsibility principle.

## Open-Closed Principles

By including these interfaces into the code design, we now have the option of adding extra features to our current classes without modifying them directly which violates the openclosed principle.

## Liskov substitution Principle

This principle dictates that inhertance should be done right. Meaning that a parent class should be replacable with a child class without messing up the code. In my current design, there is no inheritance so the principle does not aplly here.

## Interface segregation Principle

Again, by using interfaces we can make sure that the classes only use the functions they need. Meaning that if we're in a situation where we need to change a class, its bad practice if it means we have to change all the classes depending on the first class. This is why I use the interfaces, to insure that the classes are only using the functions they would use.

## Dependency Inversion Principle

This principle states that higherlevel modules should NOT depend on lowerlevel modules. They should both depend on abstractions(interfaces).

All in all this revised ATM hopefully fulfills the SOLID principles as a whole.
