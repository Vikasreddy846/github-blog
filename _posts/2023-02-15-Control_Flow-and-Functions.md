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
