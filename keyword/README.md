
## 1. Const- const
Value must be known at compile-time, const birthday  = "2008/12/25" Can't be changed after initialized.

## Example :
```
void main(){
   const name = "mukul";
   print(name);

   ### Output
       mukul
}
```


## 2. Final- final
Value must be known at run-time, final birthday = getBirthDateFromDB() Can't be changed after initialized.
## Example :
```
void main(){
   final int xy = 10;
   print(xy);
}
### Output
    10
}
```


## 3. Late- late
In some instances you would not know the value of a variable initially. And the value could possibly be null
## Example :
```
class Person {
  late String name;
}

void main() {
    Person person = Person();
    person.name = "Maria Elijah";

    print(person.name);
}

### Output
    Maria Elijah
```

## 4. Static- static
The static keyword is used for a class-level variable and method that is the same for every instance of a class, this means if a data member is static, it can be accessed without creating an object. The static keyword allows data members to persist Values between different instances of a class
## Example :
 ```

class StaticMem {
static int num;
static disp() {
	print("#GFG the value of num is ${StaticMem.num}") ;
}
}
void main() {
StaticMem.num = 75;
	
// initialize the static variable }
StaticMem.disp();
	
### Output:

#GFG the value of num is 75
}

```
## 5. Dynamic- dynamic
If a variable is declared dynamic you can change its type anytime
```
void main()
{
	// Assigning value to seek variable
	dynamic seek = "Seeks For Seeks";

	// Printing variable seek
	print(seek);

	// Reassigning the data to variable and printing it
	seek = 3.14157;
	print(seek);
}

Output:

Seeks For Seeks
3.14157
```


## 6. Var- var
If a variable is declared with var keyword and have an initial value its type can’t be changed else iff ti’s not initialised you can change its DataType anytime too.
```
Example -

var name = 'Andrew'
```


