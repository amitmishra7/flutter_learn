# Classes

Class is the blueprint of objects and class is the collection of data member and data function means which include this 

```
class ClassName {

   // Body of class
}
```

## Declaring objects in Dart

Objects are the instance of the class and they are declared by using new keyword followed by the class name.

```
var objectName = new ClassName([ arguments ]);
```

* new is the keyword use to declare the instance of the class
* objectName is the name of the object and its naming is similar to the variable name in dart.
* ClassName is the name of the class whose instance variable is been created.
* arguments are the input which are needed to be pass if we are willing to call a constructor.

## Accessing properties and methods

```
// For accessing the property
object_name.property_name;

// For accessing the method
object_name.method_name();
```

# Mixins

Mixins are a way of reusing a class’s code in multiple class hierarchies.

```
abstract class Walker {
  // This class is intended to be used as a mixin, and should not be
  // extended directly.
  factory Walker._() => null;

  void walk() {
    print("I'm walking");
  }
}
```

```
class Cat extends Mammal with Walker {}
```

* To use a mixin, use the with keyword followed by one or more mixin name

* Its similar to interface concept which we use in OOPs

