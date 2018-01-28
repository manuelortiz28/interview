---
title: Java
layout: page
---

# Java

## Access modifiers

 _ | Same class | Another class same package | Subclass from another package | Another class in another project
- | - | - | -| -
public    | X | X | X | X
protected | X | X | X | 
default   | X | X |   | 
private   | X |   |   | 


## Definitions

* **Abstract class:** A class that contains abstract methods, which are not implemented. This class can not be instantiated and all classes than extends from this one, needs to implement the abstract methods (unless is also an abstract class).
* **Interface:** This can not have any method implemented. All methods are public and abstract by default. All the attributes are static and final.
* **Static:** Members than are part of the class and not from instances. 
* **Final:** Declares a constant.
  - **Final Class:** It can not be instantiate.
  - **Final Method:** It can not be override.
* **finally, finalize:** 
  - **finally:** It is part of the try/catch/finally block. This is optional.
  - **finalize:** Part of the Object class, which is called when the garbage collector is releasing it.

## Exceptions

* **Unchecked:** Usually are produced by programmer mistakes (bugs), like the ```NullPointerException```. These are subclases of RuntimeException.java. Errors are also unchecked exceptions. Errors shouldn't need to be catched, due after an error, try to recover the app is almost imposible. For instance, after an ```OutOfMemoryError```.
* **Checked:** These are produced by a condition that we can not handle. For instance, a problem with the database or with the network; some unexisting file, etc. This kind of exception are validated in compilation time, if any of this the compiler detects that could be thrown, it asks as a mandatory rule, that a try/catch block should be added, or you will need to add the ```throws``` to the method.

![Exceptions](/images/exceptions.png)

## Collections