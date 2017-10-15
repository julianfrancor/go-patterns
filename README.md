# Design Patterns for Go
 
[![GoDoc](http://godoc.org/github.com/bvwells/go-patterns?status.svg)](http://godoc.org/github.com/bvwells/go-patterns)
[![Build Status](https://travis-ci.org/bvwells/go-patterns.svg?branch=master)](https://travis-ci.org/bvwells/go-patterns)
[![Build status](https://ci.appveyor.com/api/projects/status/ea2u4hpy555b6ady?svg=true)](https://ci.appveyor.com/project/bvwells/go-patterns)
[![codecov](https://codecov.io/gh/bvwells/go-patterns/branch/master/graph/badge.svg)](https://codecov.io/gh/bvwells/go-patterns)
[![Go Report Card](https://goreportcard.com/badge/github.com/bvwells/go-patterns)](https://goreportcard.com/report/github.com/bvwells/go-patterns)

Design patterns for the Go programming language.

``` go
import "github.com/bvwells/go-patterns"
```

To install the packages on your system,

```
$ go get -u github.com/bvwells/go-patterns/...
```

Documentation and examples are available at http://godoc.org/github.com/bvwells/go-patterns

 * [Design Patterns](#design-patterns)
 * [Creational](#creational)
 * [Structural](#structural)
 * [Behavioral](#behavioral)
 * [Go Versions Supported](#go-versions-supported)

## Design Patterns

Pattern    | Package                                   | Description
-----------|-------------------------------------------|------------
Creational | [`github.com/bvwells/go-patterns/creational`][creational-ref] | Creational design patterns are design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. The basic form of object creation could result in design problems or in added complexity to the design. Creational design patterns solve this problem by somehow controlling this object creation.
Structural | [`github.com/bvwells/go-patterns/structural`][structural-ref] | Structural design patterns are design patterns that ease the design by identifying a simple way to realize relationships between entities.
Behavioral | [`github.com/bvwells/go-patterns/behavioral`][behavioral-ref] | Behavioral design patterns are design patterns that identify common communication patterns between objects and realize these patterns. By doing so, these patterns increase flexibility in carrying out this communication.

## Creational [![GoDoc](https://godoc.org/github.com/bvwells/go-patterns/creational?status.svg)](https://godoc.org/github.com/bvwells/go-patterns/creational)

Name       | Description                               | Status
-----------|-------------------------------------------|------------
Abstract Factory | Provide an interface for creating families of related or dependent objects without specifying their concrete classes. | Implemented
Builder | Separate the construction of a complex object from its representation, allowing the same construction process to create various representations.  | Implemented
Factory Method | Define an interface for creating a single object, but let subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.  | Implemented
Object Pool | Avoid expensive acquisition and release of resources by recycling objects that are no longer in use. Can be considered a generalisation of connection pool and thread pool patterns.  | Implemented
Prototype | Specify the kinds of objects to create using a prototypical instance, and create new objects from the 'skeleton' of an existing object, thus boosting performance and keeping memory footprints to a minimum.  | Implemented
Singleton | Ensure a class has only one instance, and provide a global point of access to it. | Implemented

## Structural [![GoDoc](https://godoc.org/github.com/bvwells/go-patterns/structural?status.svg)](https://godoc.org/github.com/bvwells/go-patterns/structutal)

Name       | Description                               | Status
-----------|-------------------------------------------|------------
Adaptor | Convert the interface of a class into another interface clients expect. An adapter lets classes work together that could not otherwise because of incompatible interfaces. The enterprise integration pattern equivalent is the translator. | Implemented
Bridge | Decouple an abstraction from its implementation allowing the two to vary independently. |
Composite | Compose objects into tree structures to represent part-whole hierarchies. Composite lets clients treat individual objects and compositions of objects uniformly. |
Decorator | Attach additional responsibilities to an object dynamically keeping the same interface. Decorators provide a flexible alternative to subclassing for extending functionality. | Implemented
Facade | Provide a unified interface to a set of interfaces in a subsystem. Facade defines a higher-level interface that makes the subsystem easier to use. |
Flyweight | Use sharing to support large numbers of similar objects efficiently. |
Proxy | Provide a surrogate or placeholder for another object to control access to it. | Implemented

## Behavioral [![GoDoc](https://godoc.org/github.com/bvwells/go-patterns/behavioral?status.svg)](https://godoc.org/github.com/bvwells/go-patterns/behavioral)

Name       | Description                               | Status
-----------|-------------------------------------------|------------
Chain of Responsibility | Avoid coupling the sender of a request to its receiver by giving more than one object a chance to handle the request. Chain the receiving objects and pass the request along the chain until an object handles it. |
Command | Encapsulate a request as an object, thereby allowing for the parameterization of clients with different requests, and the queuing or logging of requests. It also allows for the support of undoable operations. |
Interpretor | Given a language, define a representation for its grammar along with an interpreter that uses the representation to interpret sentences in the language. |
Iterator | Provide a way to access the elements of an aggregate object sequentially without exposing its underlying representation. |
Mediator | Define an object that encapsulates how a set of objects interact. Mediator promotes loose coupling by keeping objects from referring to each other explicitly, and it allows their interaction to vary independently. |
Memento | Without violating encapsulation, capture and externalize an object's internal state allowing the object to be restored to this state later. |
Null Object | Avoid null references by providing a default object. |
Observer | Define a one-to-many dependency between objects where a state change in one object results in all its dependents being notified and updated automatically. |
State | Allow an object to alter its behavior when its internal state changes. The object will appear to change its class. |
Strategy | Define a family of algorithms, encapsulate each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients that use it. |
Template Method | Define the skeleton of an algorithm in an operation, deferring some steps to subclasses. Template method lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure. |
Visitor | Represent an operation to be performed on the elements of an object structure. Visitor lets a new operation be defined without changing the classes of the elements on which it operates. |

## Go Versions Supported

The most recent major version of Go is supported. You can see which versions are
currently supported by looking at the lines following `go:` in
[`.travis.yml`](.travis.yml).

[creational-ref]: https://godoc.org/github.com/bvwells/go-patterns/creational
[structural-ref]: https://godoc.org/github.com/bvwells/go-patterns/structural
[behavioral-ref]: https://godoc.org/github.com/bvwells/go-patterns/behavioral
