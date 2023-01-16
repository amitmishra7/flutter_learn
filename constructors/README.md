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






