# java-interfaces

source: http://tutorials.jenkov.com/java/interfaces.html

# Creating an interface
    <code>
      public interface MyInterface {
        public String hello = "Hello";

        public void sayHello();
      }
    </code>

# Call it
    <code>
      System.out.println(MyInterface.hello);

    </code>

or like this: 

    <code> 
      MyInterface myInterface = new MyInterfaceImpl();

      myInterface.sayHello();
    </code>

# Implementation
    <code>
      public class MyInterfaceImpl implements MyInterface {
        public void sayHello() {
            System.out.println(MyInterface.hello);
        }
      }
    </code>
