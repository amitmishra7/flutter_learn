# Constructors

Its a function with  same name as class

### Most common constructor representation

```
class Point {
  double x = 0;
  double y = 0;

  Point(double x, double y) {
    // See initializing formal parameters for a better way
    // to initialize instance variables.
    this.x = x;
    this.y = y;
  }
}
```

* here this keyword is current instance of class and should only be used when there is conflict in names

### Intializing formal parameters

* Formal parameters in constructors are used to initialize the instance variables of a class.
* Initializing parameters can also be used to initialize non-nullable or final instance variables, which both must be initialized or provided a default value.

```
class Point {
  final double x;
  final double y;

  // Sets the x and y instance variables
  // before the constructor body runs.
  Point(this.x, this.y);
}
```

### Default constructors

If you don’t declare a constructor, a default constructor is provided for you. The default constructor has no arguments and invokes the no-argument constructor in the superclass.

### Named constructors

This are used to provide multiple constructors for a class.

```
const double xOrigin = 0;
const double yOrigin = 0;

class Point {
  final double x;
  final double y;

  Point(this.x, this.y);

  // Named constructor
  Point.origin()
      : x = xOrigin,
        y = yOrigin;
}
```

### Constant constructors

If your class produces objects that never change, you can make these objects compile-time constants. To do this, define a const constructor and make sure that all instance variables are final.

```
class Point {
  static const Point origin = ImmutablePoint(0, 0);

  final double x, y;

  const Point(this.x, this.y);
}
```

### Factory constructors

A factory constructor is a constructor that can be used when you don't necessarily want a constructor to create a new instance of your class.

```
class Area{
  int length;
  int breadth;
  int width;

  // private constructor
  const Area._internal(this.length, this.breadth) : area = length * breadth;

  // factory unnamed constructor
  factory Area(int length, int breadth) {
    if (length < 0 || breadth < 0) {
      throw Exception("Length and breadth must be positive");
    }
    // redirect to private constructor
    return Area._internal(length, breadth);
  }

  // factory named constuctor
  factory Area.default(int length, int breadth) {
    return Area._internal(10, 10);
  }
}
```

### Key Points

**Constructors aren’t inherited**

  Subclasses don’t inherit constructors from their superclass. A subclass that declares no constructors has only the default (no argument, no name) constructor.

**Order of execution of constructors**

* **[Initializer list](#initializer-list)**
* Superclass’s no-arg constructor
* Main class’s no-arg constructor

**Invoking a non-default superclass constructor**

If the superclass doesn’t have an unnamed, no-argument constructor, then you must manually call one of the constructors in the superclass. Specify the superclass constructor after a colon (:), just before the constructor body (if any).

```
class Vector2d {
  final double x;
  final double y;

  Vector2d(this.x, this.y);
}

class Vector3d extends Vector2d {
  final double z;
 
  // Below are the different way of calling super class constructor as per need

  Vector3d.type1(final double x, final double y, this.z) : super(x, y);

  Vector3d.type2(this.z) : super (1,2);

  Vector3d.type3(super.x,super.y,this.z);
}
```

## Initializer List 
Besides invoking a superclass constructor, you can also initialize instance variables before the constructor body runs. Separate initializers with commas.

```
// Initializer list sets instance variables before
// the constructor body runs.
Point.fromJson(Map<String, double> json)
    : x = json['x']!,
      y = json['y']! {
  print('In Point.fromJson(): ($x, $y)');
}
```














