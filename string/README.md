## What is Strings in Dart??
<br /> 
The String data type represents a sequence of characters. A Dart string is a sequence of UTF 16 code units.
String values in Dart can be represented using either single or double or triple quotes. Single line strings are represented using single or double quotes. Triple quotes are used to represent multi-line strings.

---
<br /> 

## The syntax of representing string values in Dart.
<br /> 

```
void main() { 

   String str1 = 'this is a single line string';  
   String str2 = "this is a single line string";  
   String str3 = '''this is a multiline line string''';  
   String str4 = """this is a multiline line string"""; 
   
   print(str1);  
   print(str2);   
   print(str3);   
   print(str4);   
}

### Output:

this is a single line string   
this is a single line string   
this is a multiline line string   
this is a multiline line string  

```


---
<br /> 
<br /> 

## What are Strings Interpolation??
<br /> 

String Interpolation is the process of adding a string to another string.  
The operator plus (+) is a commonly used mechanism to concatenate / interpolate strings.
<br /> 
<br /> 

## Example of String Interpolation
<br /> 

```

void main() { 

   String str1 = "hello";   
   String str2 = "world";   
   String res = str1+str2;   
   
   print("The concatenated string : ${res}"); 
}


### Output:
The concatenated string : Helloworld

```
---   
<br /> 
<br /> 
<br /> 
### String Properties- 
<br /> 
<br /> 

|Sr.No	| Property & Description
|--     |---
|1	|codeUnits : Returns an unmodifiable list of the UTF-16 code units of this string.
|2	|isEmpty : Returns true if this string is empty.
|3  |	Length : Returns the length of the string including space, tab and newline characters.


---
<br /> 
<br /> 
<br /> 

### Methods to Manipulate Strings-
<br /> 

|Sr.No	| Methods & Description
|--     |--
|1	|toLowerCase() : Converts all characters in this string to lower case.
|2	|toUpperCase() : Converts all characters in this string to upper case.
|3	|trim() : Returns the string without any leading and trailing whitespace.
|4	|compareTo() : Compares this object to another.
|5	|replaceAll() : Replaces all substrings that match the specified pattern with a given value.
|6	|split() : Splits the string at matches of the specified delimiter and returns a list of substrings.
|7	|substring() : Returns the substring of this string that extends from startIndex, inclusive, to endIndex, exclusive.
|8	| toString() : Returns a string representation of this object.
