# java-interfaces

source: http://tutorials.jenkov.com/java/interfaces.html

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

      public class MyInterfaceImpl implements MyInterface {
        public void sayHello() {
            System.out.println(MyInterface.hello);
        }
      }
      
