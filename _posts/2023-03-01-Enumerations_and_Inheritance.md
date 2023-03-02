## 10. Enumerations  

Enumeration is a user-defined data type in Swift that enables you to define a collection of connected values. It is comparable to a mathematical enumeration, where a set of unique values is defined.  

Syntax:  

      enum NameOfEnumeration {  
          // enumeration definition  
      }  

Enumerations can be made and used in Swift in the following ways:  

Creating an Enumeration: You can create an enumeration by using the enum keyword followed by the name of the enumeration.  
Using an Enumeration: Once you have defined an enumeration, you can use it to create variables and constants of that type.  
Switch Statements with Enumeration: One of the most common use cases for enumerations is to use them in switch statements.  

Example:  

      enum CompassPoint {  
        case north  
        case south  
        case east  
        case west  
      }  
      var direction: CompassPoint = .north  
      switch direction {  
      case .north:  
          print("Heading North")  
      case .south:  
          print("Heading South")  
      case .east:  
          print("Heading East")  
      case .west:  
          print("Heading West")  
      }  

Output:  

      Heading North  

## 11. Inheritance  

In object-oriented programming, inheritance is a fundamental concept that allows you to create a new class based on an existing class. The new class, known as the subclass, inherits the existing class, known as the superclass, and can also add new properties and methods of its own. Subclasses can be created in Swift by using the "class" keyword and the colon ":" symbol.  

Inheritance in Swift supports the following features:  

Access Control: You can restrict the visibility of the superclass's properties and methods by using access control modifiers such as private, internal, fileprivate, and public.  

Overriding: Using the override keyword, you can override the superclass's properties and methods in the subclass. This lets you maintain the functionality of the superclass while still allowing the subclass to have unique behavior.  

Polymorphism: Anywhere a superclass object is expected, a subclass object may be used. One of the main advantages of inheritance is a phenomenon known as polymorphism.  

Superclass Initialization: A subclass must call the init() method of the superclass before initializing any of its properties. The super.init() method can be utilized for this. The superclass and subclass can both make use of designated and convenient initializers.  

Multiple Inheritance: A subclass may only inherit from one superclass because Swift does not support multiple inheritance. However, protocols can be used to achieve comparable functionality.  

Example:  

      class Vehicle {  
          var speed: Double  

          init(speed: Double) {  
              self.speed = speed  
          }  

          func accelerate() {  
              speed += 10  
          }  
      }  

      class Car: Vehicle {  
          var numberOfWheels: Int  

          init(speed: Double, numberOfWheels: Int) {  
              self.numberOfWheels = numberOfWheels  
              super.init(speed: speed)  
          }  

      }  
      let vehicle = Vehicle(speed: 50)  
      vehicle.accelerate()  
      print(vehicle.speed)  

      let car = Car(speed: 30, numberOfWheels: 4)  
      car.accelerate()  
      print(car.speed)  
      print(car.numberOfWheels)  

Output:  

      60.0  
      40.0  
      4  

## Challenges  

Swift and C both have enumerations, but they differ slightly from one another. I therefore had some trouble comprehending that idea.  

## References  

W3 Schools (https://www.w3schools.in/swift)  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/inheritance/  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/enumerations  
