###  Design Patterns 101
### Languages which we will take a look at 
- Java
- Python
- Golang
- Javascript 
- Clojure 

#### Creational Design Pattern
Creational patterns provide various mechanisms by which we can create object with a virtue of 
- reuse, 
- less memory foot-print
- flexibility
##### Patterns 
- Factory Method
Create an instance of several derived classes.
Factory Method provides an interface for creating objects in a superclass, 
but allows subclasses to alter the type of objects that will be created.
When to use:
  - When you dont know beforehand the exact types and dependencies of the objects 
  - When you want to provide users a way to extend its internal components. 
  - When you want to save system resources by reusing exiting objects instead of rebuilding them each time.
   
- Abstract Factory
Creates an instance of several families of classes.  
Abstract Factory let you produce families of related objects without specifying their concrete classes.
When to use:
  - When we need to work with various families of related products, 
  but dont want to depends on the concrete classes of those products. 
  - This will allow for future extensibility. 
  
- Builder
Separates object construction from its representation.
Builder lets you construct complex objects step by steps. 
The pattern allows you to produce different types and representations of an object using the same construction code. 
When to use: 
  - When you want to support fluent API's for object creations.
  
- Object Pool
Avoid expensive acquisition and release of resources by recycling objects that are no longer in use.
 
- Prototype
Prototype interface declares the cloning methods, "clone". 
Lets you copy exiting objects without making your code dependent on their classes

- Singleton
A class of which only a single instance can exit. 

#### Structural Design Pattern
- Adapter
Match interface of different classes
Allows objects with incompatible interfaces to collaborate
 - Adaptor works after code is designed.
 - Adaptor provides a variance to the interface 
 When to use:
 - You want to use some existing class but its interface isn't compatible with rest of code.
 - You want to reuse several existing subclasses that lack some 
 common functionality that can't be added to the superclass 

- Bridge
Separates an object's interface from its implementation.
 - Designed upfront, to provide abstraction.
 - decouple an abstraction from it's implementation so that the two can vary independently. 
 When to use:
  - you want runtime binding of the implementation.
  
  
Example: TV and remote: holds a bridge but implementation of each may vary.
 
- Composite
A tree structure of simple and composite objects. 
Let you compose objects into tree structures and then work with
these structures as if they were individual objects.
When to use:
 - when we have composition like structure for extension

- Decorator
- Facade
- Flyweight
- Private Class Data
- Proxy 

#### Behavioral Design Pattern
- Chain of responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- Null Object
- Observer
- State
- Strategy
- Template method
- Visitor 




