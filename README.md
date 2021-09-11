# 002.1_JDVLAOIS_

The project is include the next list of topics:<br/>
* DataTypes,
* Variables,
* Loops,
* Arrays,
* Operators,
* If-Else operator 
* Switch operator
---

## <p align=center>DataTypes</p>

Java is a **statically and strongly typed language** because these functions are inherited from C and C++.

Data Types in Java:
![Data types in Java](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20191105111644/Data-types-in-Java.jpg)
---
<br/>

# Java has two categories of data: 
 
1. **Primitive Data Type**: such as *boolean, char, int, short, byte, long, float, and double*<br/>
2. **Non-Primitive Data Type** or **Object Data type**: such as *String, Array and etc.*

![Data types in Java](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20191105122725/Primitive-Data-Types-in-Java-4.jpg)
<br/>


## <p align=center><b>Primitive Data Types</b></p>
# 

Primitive data are only single values and have no special capabilities. 

1. **boolean:** The data type represents only one bit of information either *true* or *false*, but the size of the boolean data type is virtual machine-dependent.<br/>
**Default value:** *false*

Basic syntax for declaring a boolean
```java
boolean <boolVariableName>;
```
Example :
```java
// Declaring and assigning a value
boolean flag = false;
```

<br/>

1. **byte:** The data type is an 8-bit signed integer. Useful for saving memory in large arrays.<br/> 
**Default value:** *0*

Basic syntax for declaring a byte
```java
byte <byteVariableName>;
```
Example :
```java
// Declaring and assigning a value
byte bVar = -128;
```

<br/>

1. **short:** The data type is a 16-bit signed integer. Useful for saving memory in large arrays such as byte.<br/> 
**Default value:** *0*

Basic syntax for declaring a short
```java
short <shortVariableName>;
```
Example :
```java
// Declaring and assigning a value
short shortVar = -15562;
```

<br/>

4. **int:** It is a 32-bit (4 Bytes) signed integer.<br/>
**Default value:** *0* 

Basic syntax for declaring a int
```java
int <integerVariableName>;
```
Example :
```java
// Declaring and assigning a value
int intVar = 89;
```
*Note:* In Java SE 8 and later, we can use the int data type to represent an **unsigned** 32-bit integer, which has value in the range [0 ... 2<sup>32</sup> -1]. Use the **Integer class** to use int data type as an *unsigned integer*.

<br/>

5. **long:** The data type is a 64-bit (8 Bytes) signed integer.<br/>
**Default value:** *0* 

Basic syntax for declaring a long
```java
long <longVariableName>;
```
Example :
```java
// Declaring and assigning a value
long longVar = -504588810;
```
*Note:* In Java SE 8 and later, you can use the long data type to represent an **unsigned** 64-bit long, which has a minimum value of 0 and a maximum value of 2<sup>64</sup>-1. The **Long class** also contains methods like *comparing Unsigned*, *divide Unsigned* and etc. **to support arithmetic operations for unsigned long**.<br/>

<br/>

6.  **float:** The data type is a single-precision 32-bit (4 Bytes) [IEEE 754][1] floating-point. Useful for saving memory (instead of double) in large arrays of floating-point numbers.<br/>
**Default value:** *0.0* 


Basic syntax for declaring a float
```java
float <floatVariableName>;
```

<p align=center><b>:warning: BE CAREFULLY :warning:</b></p>

> By *DEFAULT* in Java, the value of **real data types** is *DOUBLE*   
> Everywhere for the FLOAT values you have to use **f** as a suffix

Example :
```java
// Declaring and assigning a value
float floatVar = 4.7333434f;
```
<br/>

7.  **double:** The data type is a double-precision 64-bit (8 Bytes) [IEEE 754][1] floating-point.<br/> For **decimal values**, this data type is generally use by  DEFAULT.<br/>
**Default value:** *0.0*

Basic syntax for declaring a double
```java
double <doubleVariableName>;
```
Example :
```java
// Declaring and assigning a value
double doubleVar = -2454.355453532;
```
*Note:* Both float and double data types were designed especially for scientific calculations, where approximation errors are acceptable.<br/> If precision is a top priority, it is *strongly recommended to use* the **[*BigDecimal*][2] class** instead of these primitive data type.<br/> Please see this for details: [*Rounding off errors in Java*][3]
<br/>

8.  **char:** The data type is a single 16-bit (2 Bytes) Unicode character (UNSIGNED). <br>
**Default value:** *\u0000*

Basic syntax for declaring a char
```java
char <charVariableName>;
```
>*Note:* The char data type may contain the escape consequences!

Example:
```java
// Declaring and assigning a value
char endLine = '\n';
```
### **Why is the size of char is 2 byte in Java?** <br/>
In other languages like C/C++ uses only ASCII characters and to represent all ASCII characters 8-bits is enough, 
But java uses the Unicode system not the ASCII code system and to represent Unicode system 8 bit is not enough to represent all characters so Java uses 2 bytes for characters.<br/>
***Unicode** defines a fully international character set that can represent most of the world’s written languages. It is a unification of dozens of character sets, such as Latin, Greeks, Cyrillic, Katakana, Arabic, and many more.*
---
<br/>

[1]: https://en.wikipedia.org/wiki/IEEE_floating_point
[2]: http://docs.oracle.com/javase/1.5.0/docs/api/java/math/BigDecimal.html
[3]: https://www.geeksforgeeks.org/rounding-off-errors-java/

<br/>


## <p align=center><b>Non-Primitive</b> Data Type or <b>Reference</b> Data Types</p>
# 

The **Reference Data Types** will contain a memory address of variable value because the reference types won’t store the variable value directly in memory. They are [*arrays*][4], [*strings*][5], [*class*][10], [*objects*][6], [*interface*][13], etc.

[4]: https://github.com/yoricsv/002.1_JDVLAOIS_.git
[5]: https://github.com/yoricsv/002.3_JStringRegExp_.git
[6]: https://github.com/yoricsv/004.1_JCOIP_.git

* [**String:**][4] Strings are defined as an array of characters. The difference between a character array and a string in Java is, the string is designed to hold a sequence of characters in a single variable whereas, a character array is a collection of separate char type entities.
* Unlike C/C++, Java strings are not terminated with a null character.
Below is the basic syntax for declaring a string in Java programming language.

Basic syntax for declaring a string
```java
<StringType> <stringName> = “<stringSequence>”;
```

Example *(without memory allocation on the heap)*:
```java
// Declaring 
String str = "Hello, world!";
```

Example *(with memory allocation on the heap)*:
```java
// Declare String using new operator 
String str = new String("Hello, world!"); 
```
* [Class:][10] A class is a user-defined blueprint or prototype from which objects are created.  It represents the set of properties or methods that are common to all objects of one type. In general, class declarations can include these components, in order: 
   1. **Modifiers:** A class can be public or has default access (Refer [*this*][11] for details).
   2. **Class name:** The name should begin with a initial letter (capitalized by convention).
   3. **Superclass (*if any*):** The name of the class’s parent (superclass), if any, preceded by the keyword extends. A class can only extend (subclass) one parent.
   4. **Interfaces (*if any*):** A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword implements. A class can implement more than one interface.
   5. **Body:** The class body surrounded by braces, *{ }*.

[10]: https://www.geeksforgeeks.org/classes-objects-java/
[11]: https://www.geeksforgeeks.org/access-specifiers-for-classes-or-interfaces-in-java/

* [**Object:**][12] It is a basic unit of Object-Oriented Programming and represents the real-life entities.  A typical Java program creates many objects, which as you know, interact by invoking methods. An object consists of : 
   1. **State:** It is represented by attributes of an object. It also reflects the properties of an object.
   2. **Behavior:** It is represented by methods of an object. It also reflects the response of an object with other objects.
   3. **Identity:** It gives a unique name to an object and enables one object to interact with other objects.

[12]: https://www.geeksforgeeks.org/classes-objects-java/

* [**Interface:**][13] Like a class, an interface can have methods and variables, but the methods declared in an interface are by default abstract (only method signature, nobody).   
   * Interfaces specify what a class must do and not how. It is the blueprint of the class.
   * An Interface is about capabilities like a Player may be an interface and any class implementing Player must be able to (or must implement) move(). So it specifies a set of methods that the class has to implement.
   * If a class implements an interface and does not provide method bodies for all functions specified in the interface, then the class must be declared abstract.
   * A Java library example is, [*Comparator Interface*][14]. If a class implements this interface, then it can be used to sort a collection.

[13]: https://www.geeksforgeeks.org/interfaces-in-java/
[14]: https://www.geeksforgeeks.org/comparator-interface-java/
---
<br/>


## <p align=center><b>Arrays</b></p>
# 

* [**Array:**][4] An array is a group of like-typed variables that are referred to by a common name. Arrays in Java work differently than they do in C/C++. The following are some important points about Java arrays. 
   * In Java, all arrays are dynamically allocated. (discussed below) 
 
   * Since arrays are objects in Java, we can find their length using member length. This is different from C/C++ where we find length using size.
   * A Java array variable can also be declared like other variables with [] after the data type.
   * The variables in the array are ordered and each has an index beginning from 0.
   * Java array can be also be used as a static field, a local variable or a method parameter.
   * The size of an array must be specified by an int value and not long or short.
   * The direct superclass of an array type is [Object][7].
   
   * Every array type implements the interfaces [Cloneable][8] and [java.io.Serializable][9].

[7]: https://www.geeksforgeeks.org/object-class-in-java/
[8]: https://www.geeksforgeeks.org/serialization-in-java/
[9]: https://www.geeksforgeeks.org/marker-interface-java/

---
<br/>


## <p align=center><b>Loops</b></p>
# 

---
<br/>


## <p align=center><b>Operators</b></p>
# 

---
<br/>


## <p align=center><b>If-Else operator</b></p>
# 

---
<br/>


## <p align=center><b>Switch operator</b></p>
# 

