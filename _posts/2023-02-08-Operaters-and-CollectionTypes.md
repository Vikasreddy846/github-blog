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
