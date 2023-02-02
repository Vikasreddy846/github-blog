---
title: "Programming Language Blog"
date: 2023-01-23
---

Swift is the programming language I considered choosing.
I choose Swift because it is the programming language used in Apple platforms for the development of applications, and I anticipate that demand for Apple products will increase in the future, as will that for the Swift programming language.
I compared a few programming languages and found Swift to be more readable and understandable. 

##More about Swift Programming Language  
Objective-C, which was used prior to Swift, has been replaced by Swift.  
Swift supports procedural, object-oriented, and functional programming.  
Small command-line functions to sophisticated iOS and macOS applications can all be developed using Swift.  

# Let's start using Swift:  

We're going to start with a simple program called "Hello World," and the syntax for printing it is  
Syntax:  
      print (“Hello World”)  
Output:  
Hello World  

## 1. Comments  

Comments are used to add meaningful explanations to the code. The compiler ignores comments and does not compile them into the code. Single-line comments and multi-line comments are the two different kinds of comments available in Swift.   
In order to create a single-line comment, you must first insert two forward slashes before writing.  
Syntax:  
      //single line comment  
A forward slash and an asterisk (/*) indicate the beginning of a multi-line comment, and an asterisk and a forward slash (*/) indicate the end:  
Syntax:  
      /* multi-line  
      comment */  
## 2. Variables and Constants  
In order to store and manage data, variables and constants are used.  
Variables are mutable so that their values can be changed with the code at any point of time in a program. The "var" keyword is used to declare variables, which are then followed by their names and values:  
Syntax:  
      var course=”Software Engineering”  
      print(var)  
Output:  
Software Engineering  
Later on in your program, if you need to change the value of a variable, you just give it a new value:  
Syntax:  
      var course=”Software Development”  
Constants have a fixed value that cannot be changed after they are defined; no further alterations can be made to their value. They are immutable. To declare a constant we use the "let" keyword followed by the name of the constant and its value:  
Syntax:  
      let num=”CSCI-5300”  
      print(num)  
Output:  
CSCI-5300  
A constant's value cannot be altered once it has been set. A compile-time error will appear if you try to do this.  
## 3. Data Types  
Data types are used to define the type of values that a variable or constant can store.  Some of the data types in Swift are  
Integer: Integer data type is used to represent whole numbers and some of the data types are “Int”, “Int8”, “Int16”, “Int32” and “Int64”.  
Float: Fractional numbers are represented using a float data type. The float and double data types are available in Swift. Float is of 32 bit and Double is of 64 bit.  
Boolean: Binary values "true" or "false" are represented by boolean data types.  
String: A group of characters, such as a word or a sentence, are represented as a string data type.  
Array: For collections of ordered values, such as [1, 2, 3], arrays are used. Swift arrays can contain any kind of value, including other arrays.  
Optional: Optional is used to describe values that could be missing or nonexistent. Swift provides Optionals as a way to securely handle the potential for missing data.  
Syntax for Data Types  
      var num1: Int=25                    // Syntax for declaring Integer  
      var num2: Float=12.54    	        // Syntax for declaring Float  
      var num3: Double=5.8735536         // Syntax for declaring Double  
      var num4: String =”Vikas Reddy”    //  Syntax for declaring String  
      var num4: Bool=true  		        //  Syntax for declaring Boolean  
      var num5: Array=[1,2,3]	        // Syntax for declaring Array  
      print(num1)  
      print(num2)  
      print(num3)  
      print(num4)  
      print(num5)  

Output:  
25  
12.54  
5.8735536  
Vikas Reddy  
true  
[1,2,3]  
