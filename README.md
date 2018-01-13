# java-interfaces

# Creating an interface

      public interface MyInterface {
        public String hello = "Hello";

        public void sayHello();
      }

# Call it

      System.out.println(MyInterface.hello);


or like this: 
 
      MyInterface myInterface = new MyInterfaceImpl();

      myInterface.sayHello();
      

# Implementation
## Single
      public class MyInterfaceImpl implements MyInterface {
        public void sayHello() {
            System.out.println(MyInterface.hello);
        }
      }
      
## multiple

      public class MyInterfaceImpl
          implements MyInterface, MyOtherInterface {

          public void sayHello() {
              System.out.println("Hello");
          }

          public void sayGoodbye() {
              System.out.println("Goodbye");
          }
      }
      
source: http://tutorials.jenkov.com/java/interfaces.html
