## Data Types in Dart.
 
The Dart language supports the following types−
* Numbers
* Strings
* Booleans
* Lists
* Maps


#### 1. Number: The number in Dart Programming is the data type that is used to hold the numeric value. Dart numbers can be classified as: 

* The int data type is used to represent whole numbers.
* The double data type is used to represent 64-bit floating-point numbers.
* The num type is an inherited data type of the int and double types.

### Example of Integer and double-

```
void main() {
	
// declare an integer
int num1 = 2;			
	
// declare a double value
double num2 = 1.5;

// print the values
print(num1);
print(num2);
var a1 = num.parse("1");
var b1 = num.parse("2.34");
	
var c1 = a1+b1;
print("Product = ${c1}");
}


Output: 
2
1.5
Product = 3.34
```


#### 2. String: It used to represent a sequence of characters. It is a sequence of UTF-16 code units. The keyword string is used to represent string literals. String values are embedded in either single or double-quotes. 


### Example of Strings-

```

void main() {
	
	String string = 'Dogs''Are''Love';
	String str = 'Coding is ';
	String str1 = 'Fun';
	print (string);
	print (str + str1);
}

Output: 
DogsAreLove
Coding is Fun

```

#### 3. Boolean: It represents Boolean values true and false. The keyword bool is used to represent a Boolean literal in DART. 
 
### Examples of Boolean-

```

void main() {
String str = 'Coding is ';
String str1 = 'Fun';
	
bool val = (str==str1);
print (val);
}


Output: 

false

```

#### 4. List: List data type is similar to arrays in other programming languages. A list is used to represent a collection of objects. It is an ordered group of objects. 

### Example of List-


```
void main()
{
	List gfg = new List(3);
	gfg[0] = 'Looks';
	gfg[1] = 'For';
	gfg[2] = 'Looks';
	
	print(gfg);
	print(gfg[0]);
}

Output:   
[Looks, For, Looks]
Looks

```

#### 5. Map: The Map object is a key and value pair. Keys and values on a map may be of any type. It is a dynamic collection. 
 

### Example of Map-

```
void main() {
Map gfg = new Map();
gfg['First'] = 'Ravi';
gfg['Second'] = 'Teja';
gfg['Third'] = 'Reddy';
print(gfg);
}

Output: 
{First: Ravi, Second: Teja, Third: Reddy}

```

Note: If the type of a variable is not specified, the variable’s type is dynamic. The dynamic keyword is used as a type annotation explicitly.