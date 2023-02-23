## 8. Structures and Classes  

In Swift, you can define custom types that can have properties and methods using either structures or classes.  

### Structures:  

In Swift, a structure is a value type, so whenever you assign or pass a structure instance to a variable or function, a copy of the original structure is created. The dot notation can be used to access a structure's properties and methods.  

Firstly you should define structure using “struct" keyword.  
Once you have defined a structure, you can create instances.  
Then you can access the properties of a structure using dot notation.  

Here is an example of a basic structure definition:  

          //Defining a Structure  

          struct Student {  
              var name: String  
              var Id: Int  
              var Course: String  
          }  

          //Creating Instances of a Structure  

          let student = Student(name: "Mortal", Id: 50, Course: "CS")  

          //Accessing Properties of a Structure  

          print(student.name)  
          print(student.Id)  
          print(student.Course)   

Output:  

          Mortal  
          50  
          CS  

### Classes:  

In Swift, classes are also custom types, but they are reference types, so when you assign a class instance to a variable or pass it to a function, you are really passing a reference to the original object, not a copy. The dot notation can be used to access a class's methods and properties as well.  

Firstly you should define a class using the “class" keyword.  
Once you have defined a class, you can create instances.  
Then you can access the properties and methods of an instance of a class using dot notation.  

Here's an example of how to define a class in Swift:  

          //Defining a Class  

          class Student{  
              var name: String  
              var Id: Int  

              init(name: String, Id: Int) {  
                  self.name = name  
                  self.Id = Id  
              }  

              func display_details() {  
                  print("The student name is \(name) holding a student Id \(Id).")  
              }  
          }  

          //Creating an Instance of a Class  

          let student = Student(name: "Viper", Id: 45)  

          //Accessing Properties and Methods  

          print(student.name)  
          print(student.Id)  
          student.display_details()  

Output:  

          Viper  
          45  
          The student name is Viper holding a student Id 45.  

## 9. Methods:  

The term "method" in Swift refers to a function that belongs to a specific type. They are used to package a particular set of instructions that can be executed on a particular type of instance and which can alter the instance's data and behavior.  

In Swift, there are two different kinds of methods: instance methods and type methods.  

### Instance Methods:  

Methods known as instance methods are those that are connected to a specific instance of a class, or structure. They are called on instances of the type for which they were defined, whether it be a class, or structure. Instance methods have access to and control over the instance's properties. They can also call type methods and other instance methods.  

Example of Instance Method:  

          class Student{  
              var name: String  
              var Id: Int  

              init(name: String, Id:Int) {  
                  self.name = name  
                  self.Id = Id  
              }  

             func display_details() {  
                  print("The student name is \(name) holding a student Id \(Id).")  
              }  
          }  

          let student = Student(name: "Nova", Id: 67)  
          student.display_details()  

Output:  

          The student name is Nova holding a student Id 67.  

As a result of being associated with an instance of the "Student" class in this example, the "display details" method is an instance method. Name and ID are two of the details printed by it.  

### Type methods:

Methods known as "type methods" are those that are associated with a type itself rather than a specific instance of the type. The "static" or "class" keyword is used to define them, and they are called on the type itself rather than on a specific instance of the type. In addition to calling other type methods and instance methods, type methods have access to and control over the type's static properties.  

Example of Type Method:  

          class Student{  
              static func display_details(_ name: String, _ Id: Int) -> String{  
                  return ("The student name is \(name) holding a student Id \(Id).")  
              }  
          }  

          let student = Student.display_details("Scout", 53)  
          print(student)  

Output:  

          The student name is Scout holding a student Id 53.  

The "display details" method in this illustration is a type method since it belongs to the "Student" class itself rather than a specific instance of the class. It requires two parameters and returns information about the student.  

## Challenges 

I had some difficulty understanding the "type method," and I had some trouble defining it.  

## References  

W3 Schools (https://www.w3schools.in/swift)  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/classesandstructures  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/methods  
