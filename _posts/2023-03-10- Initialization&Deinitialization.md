## 12. Initialization  

Initialization is the process of setting up a class, structure, or enumeration instance for use in the Swift programming language. Swift's initialization process is essential to ensuring that objects are correctly initialized and ready for use.  

Swift has two different categories of initializers: designated initializers and convenience initializers.  

### Designated Initializers:  

The primary initializer for a class is a designated initializer. It must call the designated initializer of the superclass to ensure that the entire class hierarchy is properly initialized. It is responsible for initializing all properties in a class. The init keyword is used to define a designated initializer.  

Syntax:  

      class Student {  
          var name: String  
          var Id: Int  

          init(name: String, age: Int) {  
              self.name = name  
              self.Id = age  
          }  
      }  

### Convenience Initializers:  

The term "convenience initializer" refers to a secondary initializer that offers an additional method for initializing an object. In order to ensure that the object is fully initialized, it must call a designated initializer of the same class. The convenience init keyword in Swift defines an initializer for ease of use.  

Syntax:  

      class Student {  
          var name: String  
          var Id: Int  

          init(name: String, Id: Int) {  
              self.name = name  
              self.Id = Id  
          }  

          convenience init(name: String) {  
              self.init(name: name, Id: 0)  
          }  
      }  

Example of Initialization:  

      //Designated Initializer  
      class Student{  
          var name: String  
          var Id: Int  

          init(name: String, Id: Int) {  
              self.name = name  
              self.Id = Id  
          }  
      }  

      let s = Student(name: "Mortal", Id: 304)  
      print(s.name)   
      print(s.Id)  

      //Convenience Initializer  
      class Student1{  
          var name: String  
          var Id: Int  

          init(name: String, Id: Int) {  
              self.name = name  
              self.Id = Id  
          }  

          convenience init(name: String) {  
              self.init(name: name, Id: 432)  
          }  
      }  

      let s1 = Student1(name: "Viper")  
      print(s1.name)  
      print(s1.Id)  

Output:  

      Mortal  
      304  
      Viper  
      432  

## 13. Deinitialization  

Deinitialization is the process of clearing out and releasing the resources used by an instance of a class, structure, or enumeration when it is no longer required. It is the opposite of initialization, which sets an instance's initial values to make it ready for use.  

Swift's memory management system automatically performs deinitialization when an object is no longer in use. The object's deinit method, which is defined using the deinit keyword, is called by the system.  

A unique method called deinit is automatically invoked just before a class instance is deallocated from memory. It is used to carry out any necessary cleanup, including releasing memory, closing open files, and unregistering observers.  

Example:  

      class Student {  
          var name: String  

          init(name: String) {  
              self.name = name  
              print("\(name) is initialized")  
          }  

          deinit {  
              print("\(name) is deinitialized")  
          }  
      }  

      var myInstance: Student? = Student(name: "Mortal")  

      myInstance = nil  

Output:  

      Mortal is initialized  
      Mortal is deinitialized  

## Challenges  

Initializers come in two distinct categories, which makes understanding them a little challenging.  

## References  

W3 Schools (https://www.w3schools.in/swift)  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/initialization  

https://docs.swift.org/swift-book/documentation/the-swift-programming-language/deinitialization  
