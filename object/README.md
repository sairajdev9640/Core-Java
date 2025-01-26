1.Why is wrapper class required?

Here’s an example demonstrating the use of wrapper classes in different scenarios:

1. Using Wrapper Class in Collections
   Collections like ArrayList require objects, not primitives. Wrapper classes are used to work with primitives.


            import java.util.ArrayList;
            import java.util.List;

        public class WrapperExample {
            public static void main(String[] args) {
            // Creating a list of Integer (Wrapper class for int)
        List<Integer> numbers = new ArrayList<>();

        // Adding primitive int values (Autoboxing)
        numbers.add(10);
        numbers.add(20);
        numbers.add(30);

        // Retrieving values (Unboxing)
        int firstNumber = numbers.get(0);

        System.out.println("First number: " + firstNumber); // Output: First number: 10
        System.out.println("All numbers: " + numbers);      // Output: All numbers: [10, 20, 30]
    }
}
2. Parsing and Utility Methods
   Wrapper classes provide methods to convert strings to numbers and perform utility functions.

java
Copy
Edit
public class WrapperUtility {
public static void main(String[] args) {
String numberStr = "123";

        // Converting String to primitive int using Wrapper class
        int number = Integer.parseInt(numberStr);

        // Converting int to binary string
        String binaryString = Integer.toBinaryString(number);

        System.out.println("Parsed number: " + number);       // Output: Parsed number: 123
        System.out.println("Binary representation: " + binaryString); // Output: Binary representation: 1111011
    }
}
3. Nullability
   Primitives cannot hold null, but wrapper classes can.

java
Copy
Edit
public class WrapperNullability {
public static void main(String[] args) {
Integer nullableValue = null; // Wrapper class allows null

        if (nullableValue == null) {
            System.out.println("Value is null");
        } else {
            System.out.println("Value: " + nullableValue);
        }

        // Output: Value is null
    }
}

4. Autoboxing and Unboxing
   Wrapper classes enable automatic conversion between primitives and objects.

       public class AutoBoxingUnboxing {
       public static void main(String[] args) {
       Integer boxedValue = 100; // Autoboxing: int to Integer
       int unboxedValue = boxedValue; // Unboxing: Integer to int

        System.out.println("Boxed value: " + boxedValue);   // Output: Boxed value: 100
        System.out.println("Unboxed value: " + unboxedValue); // Output: Unboxed value: 100
    }
}
5. Comparison Using Wrapper Classes
   Wrapper classes provide methods for comparison, unlike primitives.

       public class WrapperComparison {
       public static void main(String[] args) {
       Integer value1 = 50;
       Integer value2 = 100;

        int comparison = value1.compareTo(value2);

        if (comparison < 0) {
            System.out.println("value1 is less than value2");
        } else if (comparison == 0) {
            System.out.println("value1 is equal to value2");
        } else {
            System.out.println("value1 is greater than value2");
        }

        // Output: value1 is less than value2
   }
   }


