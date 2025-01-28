**1.Diffirances Between Abstract class And Interface?**


**Abstract Class:**

Can contain both abstract methods (methods without implementation) and concrete methods (methods with implementation).

A class can inherit only one abstract class because Java and C# do not support multiple inheritance for classes.

Can have constructors. This allows the abstract class to initialize fields or perform setup operations when a subclass is instantiated.

Can have instance variables (fields) with any access modifier (private, protected, etc.), and can even have constants (with the final keyword).

**Interface**

Can only contain abstract methods (in most languages, until Java 8, where it can have default methods and static methods).

A class can implement multiple interfaces. This is a way to achieve multiple inheritance of behavior.

Cannot have constructors. Interfaces cannot have any implementation or state initialization code.

All fields in an interface are implicitly public, static, and final (i.e., constants). You cannot have instance variables in an interface.

Methods in an interface are implicitly public. They cannot have other access modifiers.

    // Abstract Class
    abstract class Animal {
    // Concrete method with implementation
    public void eat() {
    System.out.println("This animal is eating.");
    }

    // Abstract method (must be implemented by subclasses)
    public abstract void sound();
}

    // Subclass that extends the abstract class
    class Dog extends Animal {
    // Provide implementation for the abstract method
    public void sound() {
    System.out.println("Bark");
    }
    }

    public class Main {
    public static void main(String[] args) {
    Dog dog = new Dog();
    dog.eat(); // Call concrete method from Animal
    dog.sound(); // Call the implemented method in Dog
    }
    }

**2. Interface Example**


    // Interface
    interface Flyable {
    // Abstract method (no implementation)
    void fly();
    }

    // Class implementing the interface
    class Bird implements Flyable {
    // Provide implementation for the abstract method
    public void fly() {
    System.out.println("The bird is flying.");
    }
    }

    public class Main {
    public static void main(String[] args) {
    Bird bird = new Bird();
    bird.fly(); // Call the implemented method in Bird
    }
}

    // Abstract class
    abstract class Animal {
    public void eat() {
    System.out.println("This animal is eating.");
    }

    public abstract void sound();
}

    // Interface
    interface Flyable {
    void fly();
}

// Class implementing both abstract class and interface

    class Eagle extends Animal implements Flyable {
    public void sound() {
    System.out.println("Screech");
    }

    public void fly() {
        System.out.println("The eagle is flying.");
    }
    }

    public class Main {
    public static void main(String[] args) {
    Eagle eagle = new Eagle();
    eagle.eat();  // Call concrete method from Animal
    eagle.sound(); // Call implemented method in Eagle
    eagle.fly();   // Call implemented method from Flyable
    }
    }
