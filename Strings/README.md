1.Why are strings immutable in java?

Safety: When a string can't be changed, it prevents(stops) unexpected modifications that could break your program.


     public class StringSafetyDemo {
      public static void method1(String data) {
     / Attempt to modify the string inside the method
      data = data + " Modified";
     System.out.println("Inside method1: " + data);
    } 

    public static void main(String[] args) {
        String originalString = "Original Data";
        
        // Pass the string to a method
        method1(originalString);
        
        // Original string remains unchanged
        System.out.println("Outside method: " + originalString);
    }


Memory Efficiency: Java can reuse the same string in multiple places without worrying about one part of the code accidentally changing it.

Hashcode Stability: Unchangeable strings mean their unique identifier (hashcode) always stays the same, which is helpful for storing and finding data quickly.

Thread Protection: In programs running multiple tasks at once, immutable strings ensure no unexpected changes happen when different parts of the program are working simultaneously.(did not create the unnecessary threads)

2.How intern() works?


In Java, the intern() method is used to manage strings more efficiently by leveraging the string pool. Here's an explanation of how it works:

What is the String Pool?
The string pool is a special memory area in the Java heap where string literals are stored. It ensures that identical string literals are stored only once, reducing memory usage.

2.How intern() Works

Definition: The intern() method of the String class checks whether the string exists in the string pool. If it does, it returns the reference to that string. If not, it adds the string to the pool and returns the reference to the newly added string.

Syntax:
String internedString = string.intern();
Process:

If the string is already present in the pool, intern() returns the reference from the pool.
If the string is not present, it adds the string to the pool and returns the reference.
Usage:

It ensures that two strings with the same content share the same memory reference, allowing comparison with ==.

        public class StringInternExample {
        public static void main(String[] args) {
        String str1 = new String("Hello");
        String str2 = "Hello"; 
        // Without intern()
        System.out.println(str1 == str2); // Output: false

        // With intern()
        String str3 = str1.intern();
        System.out.println(str3 == str2); // Output: true
    }
}

3.What is String,StringBuilder,StringBuffer ?

StringBuffer provides built-in thread safety, while StringBuilder requires explicit synchronization if used in a multi-threaded environment.

StringBuffer,mutable,synchronized (which is why it is slow instead of stringBuilder,using )

        public class StringBufferSynchronization {
        public static void main(String[] args) {
        StringBuffer sbf = new StringBuffer("Hello");

        // Create multiple threads that modify the StringBuffer
        Thread thread1 = new Thread(() -> {
            synchronized (sbf) {
                sbf.append(" World");
                System.out.println(Thread.currentThread().getName() + " updated: " + sbf);
            }
        });

        Thread thread2 = new Thread(() -> {
            synchronized (sbf) {
                sbf.append(" Everyone");
                System.out.println(Thread.currentThread().getName() + " updated: " + sbf);
            }
        });

        // Start the threads
        thread1.start();
        thread2.start();

        // Wait for threads to finish
        try {
            thread1.join();
            thread2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        System.out.println("Final StringBuffer content: " + sbf);
    }
}


