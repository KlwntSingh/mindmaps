# Design Patterns
Head first book

## Design Principals:
rules which are followed in design pattern

### encapsulate what varies

- strategy pattern
- encapsulating part which varies with every new requirement, let us change/extend it without effecting other parts
- possible cases where this is applicable

	- if/else
	- same code with different implementations

- eg:

### code to supertype(interface or abstract class)

- strategey pattern
- code to interface rather than implementation

	- using new operator means coding to implementation
	- Using supertype to refer a object
	- favor interface over abstract class because once abstract class is inherited, no other class can be inherited, which is serious limitation

- Program to interface and not implementation
- factory pattern is power technique to do this

### favor composition over inheritance

- strategey pattern

### Strive for loosely coupled design between objects that interact

- observer patten

	- way observer is notified from observable without observable knowing about observers

### classes should be open for extension but closed for modification

- another example is observer patter, subject or observable can be extended by adding new observers without changing any code in subject
- two ways of doing it

	- inheritance
	- composition is way to do it.
we can compose new objects to add new functionality rather than changing existing code

		- decorator pattern

### depend upon abstraction. do not depend upon concrete class

- factory method and abstract factory method makes your code indpendent of concrete class
- helps in loosely coupled concrete classes from application
- dependency inversion principle

	- factory method is one technique adhering to it
	- depend upon abstractions do not depend upon concrete classes

### principle of least knowledge. talk only to close friends

- facade pattern helps in implementing the pattern

	- facade makes client only to be friends with facade class and not dependent on other classes

### Hollywood principle; don't call us, we will call you

- factory method, strategy pattern, template pattern
- high level components calls the methods of algorithm in subclasses and not vice versa

### Single Responsibility Principle: class should have only reason to change

## inheritance

### use

- code reuse

### baggage

- if subclass don't want to use any method from superclass, than it is not possible 
- child class will not able to inherit any other class

### alternative to inheritance are

- composition
- wrapping object or decorator pattern

### It is compile time

- extension at runtime is more powerful then at compile time using inheritance

### two benefits

- behaviour reuse
- type control

## composition

### use

- encapsulate family of algorithms in it's own classes, hence code reuse
- runtime change of algorithm

### baggage

### it is runtime

## patterns

### Strategy

### Observer Pattern

- defines loosely coupled design

### Decorator pattern

- adding additional responsibilities to object dynamically. it provides flexibility alternative to subclassing or extending functionality
- decorating class has-a and is-a relationship with decorated class

### factory method

- subclass decides which object to create

### abstract factory

### singleton

- ensure class has only one instance and provide global point of access to it

### command pattern

- adds level of indirection
- different types of object getting wrapped by class implementing same interface

### adapter pattern

- class implements the interface compatible with client and composes object which client needs to use but was incompatible

### facade pattern

- wrapping multiple objects together to call methods on object easier
- violates Single responsiblility principle

### template method pattern

- high level classes calling low level classes

### iterator pattern

- provides way to access elements without client knowing the underlying aggregate structure used

## personal notes

### decision on making new subclass or object will be enough is based on following points

- if different methods, than subclass
- if different instance variables, than subclass
- if different values of instance variables than objects

### abstract class is class which is just above implementation in class hierarchy

### we need to think of classss and bojects close to rela world

- eg: if there can only be one of anything present, we need make only one object of that thing in our application

### questions to ask while designing

- with every new NOUN(class name)?

	- tells you to design interface/class, which is independent of implementation. 
gives you a way to think in abstract

- tries to break the problem as much as you can

## problems patterns solve

### resusability

### maintainability

- because of change

### extensibility

## different types of design patterns

### used at runtime/compile

- runtime

	- strategy pattern
	- decorator pattern

		- dynamic mix and match class saves a lot number of class

	- singleton pattern
	- factory method and abstract factory

- compile

	- command pattern
	- decorator pattern

		- because developer does not have to write all the classes

### code structural
which code flow

- observer pattern
- command pattern

