---
title: "Programming Language Blog"
date: 2023-01-23
---

Swift is the programming language I considered choosing.
I choose Swift because it is the programming language used in Apple platforms for the development of applications, and I anticipate that demand for Apple products will increase in the future, as will that for the Swift programming language.
I compared a few programming languages and found Swift to be more readable and understandable. 

## More about Swift Programming Language  
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
      
## 4. Operators 

Here is a list of the most commonly used operators in Swift:  

Arithmetic Operators:  

Addition (+)  
Subtraction (-)  
Multiplication (*)  
Division (/)  
Modulo (%)  

Comparison Operators:  

Equal to (==)  
Not equal to (!=)  
Greater than (>)  
Less than (<)  
Greater than or equal to (>=)  
Less than or equal to (<=)  

Logical Operators:  

Logical AND (&&)  
Logical OR (||)  
Logical NOT (!)  

Range Operators:  

Closed Range (a...b)  
Half-open range operator(a..<b)  

Ternary Conditional Operator:  

Ternary conditional operator: a ? b :c, If a is true, it evaluates b and returns its value; otherwise, it evaluates c and returns its value.  

Syntax for Operators: 

            //Assignment Operator  

            var a = 23  
            var name = "Josh"  

            //Arithmetic Operator +, -, *, / and %  

            var hello = "Hello " + "Playground!"  
            var sum = 10 + 30.8  

            var p = 20  
            var q = 5  

            p - q  
            p * q  
            p / q  
            p % q  

            //Compound Assignment  

            p += q  

            //Comparison Operator  

            var r = 32  
            var s = 12  

            r == s //Equality Operator  
            r > s //Greater than operator  
            r < s //Less than operator  
            r >= s //Greater than equal to  
            r <= s //Greater than equal to  

            //Ternary Operator  

            var number = 33  
            var parity = "None"  

            parity = number % 2 == 0 ? "Even" : "Odd"  

            //Ranges  

            for i in 1..<5 {  
                print(i)  
            }  

            //Logical Operators Not (!), AND (&&), OR (||)  

            var i= false  
            var j= true  

            if (i && j) {  
                print("True")  
            } else {  
                print("False")  
            }  

            var m= false  
            var n= true  

            if (!m || n) {  
                print("True")  
            } else {  
                print("False")  
            }  

            //Combine Them  

            if (m && n) || (!m) {  
                print("True")  
            }  
         

Output:  

            1  
            2  
            3  
            4  
            False  
            True  
            True  

## 5. Collection Types  

Arrays: A collection of values that are ordered and of any type, including other arrays, is known as an array. You can access specific values by using their index because the values are stored in a specific order.  

Sets: A set is an unordered collection of unique values. Sets don't have a defined order like arrays do, and the values are stored in any order. To make sure that every value is unique or to check for the existence of a specific value, sets are helpful.  

Dictionaries: A dictionary is a collection of key-value pairs. You can use the keys to access the corresponding values, and the order in which the values are stored is not important.  

Syntax for Collection Types:  
            
            //Arrays
            
            var emptyArray = [String]()  
            var zeros = [Int](repeating: 0, count: 20)  
            print(zeros.count)  
            var groceryList = ["Eggs", "Milk", "Oranges", "Tooth Brush", "Tooth Paste"]  
            var evenNumbers = [2, 4, 6, 8, 10]  

            groceryList.append("Hair Brush")  
            print(groceryList)  

            groceryList += ["Pineapples"]  
            print(groceryList)  

            groceryList.insert("Talcum Powder", at: 2)  

            var secondItem = groceryList[1]  

            var firstThree = groceryList[0...2]  

            var removedItem = groceryList.remove(at: 2)  
            print(removedItem)  

            for eachElement in groceryList {  
                print(eachElement)  
            }  

            for (index, element) in groceryList.enumerated() {  
                print("Number of the Item : \(index + 1) Value : \(element)")  
            }  

            //Multi Dimentional Array  

            var multiArray: [[Int]] = [[1,2,3],[4,5,6],[7,8,9]]  
            multiArray[2][1] = 88  
            print(multiArray)  

            //Dictionary  

            var student = [Int:String]()  
            student[11] = "John"  
            student[79] = "Rudra"  
            print(student)  

            student = [:]  

            var neighbours1: [Int:String] = [223: "Mr. Holmes", 229: "Dr. Nagar"]  
            var neighbours2 = [223: "Mr. H", 229: "Dr. N"]  

            var stocks = ["AAPL":"Apple", "GOOG":"Google","MSFT":"Microsoft"]  
            var company = stocks["GOOG"]  

            stocks["AAPL"] = "Apple Inc."  
            stocks["FB"] = "Facebook"  
            print(stocks)  

            for (key,value) in stocks {  
                print("Key: \(key) Value: \(value)")  
            }  

            print("All Keys")  
            for keys in stocks.keys {  
                print(keys)  
            }  

            print("All Values")  
            for value in stocks.values {  
                print(value)  
            }  

            // Sets  

            var num: Set = [2, 3, 5, 1]  

            print("Initial Set: \(num)")  

            // using insert method  
            num.insert(8)  
            print("Updated Set: \(num)")  

            var name: Set = ["mortal", "viper", "nova"]  
            print("Initial Set: \(name)")  

            // remove Java from a set  
            let removedValue = name.remove("nova")  
            print("Set after remove(): \(name)")  

Output:  

            20  
            ["Eggs", "Milk", "Oranges", "Tooth Brush", "Tooth Paste", "Hair Brush"]  
            ["Eggs", "Milk", "Oranges", "Tooth Brush", "Tooth Paste", "Hair Brush", "Pineapples"]  
            Talcum Powder  
            Eggs  
            Milk  
            Oranges  
            Tooth Brush  
            Tooth Paste  
            Hair Brush  
            Pineapples  
            Number of the Item : 1 Value : Eggs  
            Number of the Item : 2 Value : Milk  
            Number of the Item : 3 Value : Oranges  
            Number of the Item : 4 Value : Tooth Brush  
            Number of the Item : 5 Value : Tooth Paste  
            Number of the Item : 6 Value : Hair Brush  
            Number of the Item : 7 Value : Pineapples  
            [[1, 2, 3], [4, 5, 6], [7, 88, 9]]  
            [11: "John", 79: "Rudra"]  
            ["MSFT": "Microsoft", "GOOG": "Google", "AAPL": "Apple Inc.", "FB": "Facebook"]  
            Key: MSFT Value: Microsoft  
            Key: GOOG Value: Google  
            Key: AAPL Value: Apple Inc.  
            Key: FB Value: Facebook  
            All Keys  
            MSFT  
            GOOG  
            AAPL  
            FB  
            All Values  
            Microsoft  
            Google  
            Apple Inc.  
            Facebook  
            Initial Set: [5, 2, 3, 1]  
            Updated Set: [5, 2, 3, 1, 8]  
            Initial Set: ["viper", "nova", "mortal"]  
            Set after remove(): ["viper", "mortal"]  
            
## 6. Control Flow:  

Control flow in the Swift programming language is the method of choosing the sequence in which statements in your program are executed. Control flow structures let you manage various scenarios, such as branching or repeating code based on specific conditions, and control the order of execution.  

The following are a few of the most typical Swift control flow structures:  

### If/else statements: 

Depending on a condition, you can run various code blocks using an if/else statement.  

Syntax  

            if condition {  
                // The code here would be executed if the condition is true.  
            } else {  
                // The code here would be executed if the condition is false.  
            }  

 ### Loops:  
 
You can iterate over a block of code using loops. The two loop types in Swift are 'for in' loops and 'while' loops.  

For in: To iterate over a series, such as an array, a set of numbers, or a string, a "for in" loop is used.   

Syntax  

            for element in sequence {  
                // For the provided range of values, code will be executed.  
            }  
      
While: In a while loop, a block of code is repeated until a condition is no longer true.   

Syntax  

            while condition {  
                // The code here would be executed until the condition is false.  
            }  

 ### Switch statements: 
 
You can run various code blocks depending on the value of a variable or expression by using a switch statement.  

Syntax:  

            switch variable {  
            case value1:   
                // The code here would be executed if variable equals value1  
            case value2:  
                // The code here would be executed if variable equals value2  
            default:  
                //The code here would be executed if variable does not equal any of the cases  
            }  

Examples of Control Flow:  

            //if..else if..else..  

            var percentage = 45.0  
            if (percentage >= 35.0) {  
                print("Pass")  
            } else {  
                print("Fail")  
            }  

            if (percentage >= 85) {  
                print("Excellent Score")  
            } else if (percentage >= 70) {  
                print("Good Score")  
            } else if (percentage >= 35) {  
                print("Pass but needs to improve")  
            } else {  
                print("Fail")  
            }  

            //Switch Statements  

            let myNum = 56  
            switch myNum {  
            case 0:  
                print("My number is 0")  
            case 1, 3, 5, 7, 9:  
                print("My Number is Odd")  
            case 10..<100:  
                print("The number is between 10 and 100")  
            default:  
                print("none of the above")  
            }  

            let point = (0,0)  

            switch point {  
            case (0,0):  
                print("It is at origin")  
                fallthrough  
            case (0,_):  
                print("It is at y-axis")   
            case (_,0):  
                print("it is on x-axis")  
            default:  
                print("the point is anywhere but the x & y axis")  
            }  

            //Looping Constructs  

            //while loop  

            var n = 0  
            while (n < 3) {  
                print("Num: \(n)")  
                n += 1  
            }  

            var count = 0  
            repeat{  
                print("count -> \(count)")  
            } while(count < -1)  


            //For in Loops  

            for i in 1...4 {  
                print("num : \(i)")  
            }  

            for _ in 1...5 {  
                print("mortal")  
            }  

            print("-------------")  

            for c in 1...10 {  

                if c == 3{  
                    continue  
                }  

                if c == 7 {  
                    break  
                }  
                print("Counter c is \(c)")  
            }  

Output:  

            Pass  
            Pass but needs to improve  
            The number is between 10 and 100  
            It is at origin  
            it is on y-axis  
            Num: 0  
            Num: 1  
            Num: 2  
            count -> 0  
            num : 1  
            num : 2  
            num : 3  
            num : 4  
            mortal  
            mortal  
            mortal  
            mortal  
            mortal  

            -------------  

            Counter c is 1  
            Counter c is 2  
            Counter c is 4  
            Counter c is 5  
            Counter c is 6  

## 7. Functions:  

A function in the Swift programming language is an independent unit of code that carries out a particular task. Swift programming uses functions as a fundamental building block to encapsulate code and increase its reusability.  

Syntax:  

            func func_Name(parameters)-> returnType {  
              // function body   
            }  

Examples of functions:  

            // Functions Without Parameters and Return Values  

            // declare a function  
            func name() {  
              print("mortal")  
            }  
            // call the function  
            name()  

            //Functions Without Parameters  

            func name1() -> String {  
              return "mortal"  
            }  
            print(name1())  

            //Functions With One Parameter  

            func mul(n: Int) -> Int {  
                let num = n*n  
                return num  
            }  
            print("square of a given number is  \(mul(n: 5))")  

            //Functions With Multiple Parameters and Multiple Return Values  

            func min_max (x: Double, y: Double, z: Double) -> (x1: Double, x2: Double) {  

                let min_num = min(x,y,z)  
                let max_num = max(x,y,z)  
                return (min_num, max_num)  
            }  

            print("minimum and maximum number is the given set of numbers \(min_max(x: 8, y: 94, z:3))")  

Output:

            mortal
            mortal
            square of a given number is  25
            minimum and maximum number is the given set of numbers (x1: 3.0, x2: 94.0)

            
## Challenges  

I have faced some challenges in predefined functions like insert, appending used in arrays.
I encountered some difficulties when defining the parameters and the return type in the function.

## Referances  
W3 Schools (https://www.w3schools.in/swift)  

https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html
