CORE-JAVA-INTERVIEW-QUEATIONS
---

**Strings:**

1. Why are strings immutable in Java?
2. How does `intern()` work?
3. How many objects are created in Strings using string literals and the new operator?
4. How does the string constant pool work?
5. What is the difference between `equals()` and `==` operator?
6. What is the difference between `String`, `StringBuffer`, and `StringBuilder`?

---

**Object:**

7. Why is the wrapper class required?
8. What are the methods of the `Object` class?
9. Does Java give importance to primitive data types?
10. Is Java pass-by-value or pass-by-reference?

---

**OOPs:**

11. What are the types of OOPs?
12. What is the difference between Composition, Aggregation, and Association?
13. What is the difference between function overloading and overriding?
14. What is the difference between an Abstract class and an Interface?
15. Can private or static methods be overridden in Java?
16. Can the `main()` method be overloaded?
17. Can an Abstract class have a `main` method?

---

**Serialization:**

18. What is Serialization and Deserialization?
19. What is the use of the `transient` keyword?
20. Is it possible to serialize a class if its superclass is not serializable? Can the class still be serialized and deserialized?
21. Can uninitialized non-serialized, non-transient fields still be tolerated?

---

**Cloning:**

22. What is a marker interface?
23. What is the difference between shallow copy and deep copy?

---

**Exception:**

24. What is the difference between an `Error` and an `Exception`?
25. What is the difference between checked and unchecked exceptions?
26. How can you create a custom exception?
27. What is a Runtime exception?
28. How does JVM handle exceptions?
29. What is the difference between `final`, `finalize`, and `finally`?
30. What is the superclass of all exceptions?
31. Is `Throwable` an interface?
32. When doesn't the `finally` block get executed?
33. Can a subclass throw a higher checked exception than the base class?
34. Can we throw an unchecked exception in a child class if the parent class doesn’t throw any exception?
35. What is the difference between `throw` and `throws()`?
36. What is the usage of `Enum`?
37. Why should we use `Enum`?
38. How does Garbage Collection work in Java?

---

**Collection:**

39. What is the difference between an Array and an `ArrayList`?
40. What is the difference between `ArrayList` and `LinkedList`? When should each be used?
41. What is the difference between Fail-Safe and Fail-Fast iterators?
42. What is a ConcurrentModificationException?
43. What is the internal working of `HashMap`?
44. What are the Java 8 changes to `HashMap`?
45. Why can a `HashMap` contain a null key?
46. Is it mandatory to have immutable keys in a `HashMap`?
47. Why should you override the `equals()` and `hashCode()` methods?
48. What is the difference between `HashSet`, `LinkedHashSet`, and `TreeSet`?
49. What is the internal data structure of a `TreeMap`? How are the elements sorted?
50. What is the difference between `HashMap` and `ConcurrentHashMap`?
51. What is the difference between `Comparable` and `Comparator`?
52. What is a blocking queue?
53. What is a `Vector`? When should it be used?

---

**Multithreading:**

54. What is the difference between Multithreading, Multiprocessing, Multiprogramming, and Multitasking?
55. What is the life cycle of a thread?
56. What is the difference between `extends Thread` and `implements Runnable`?
57. What is the difference between `yield()`, `sleep()`, and `join()`?
58. What is the difference between `wait()` and `sleep()`?
59. Why is the `join()` method used?
60. Can we override the `start()` method in a thread?
61. Can we override the `run()` method?
62. Can we start a thread twice?
63. What is an `IllegalThreadStateException`?
64. What happens if the `run()` method is called without calling `start()`?
65. Why do we use a `ThreadPool`?
66. What is a race condition?
67. What is synchronization? What are the types of synchronization?
68. What is the difference between object-level locking and class-level locking?
69. If there are 2 synchronized methods `m1` and `m2` in a class, can two different threads `t1` and `t2` call different methods (`m1`, `m2`) on the same object at the same time?
70. If a class has a synchronized method and a non-synchronized method, can multiple threads execute the non-synchronized methods?
71. Can two threads call two different static synchronized methods of the same class?
72. Does static synchronized methods block non-synchronized methods?
73. Can constructors be synchronized?
74. What is a deadlock?
75. What is inter-thread communication? Explain `wait()`, `notify()`, and `notifyAll()`.
76. What is an `IllegalMonitorStateException`?
77. Which class do `wait()`, `notify()`, and `notifyAll()` belong to?
78. Explain a few `Thread` class methods. Is `sleep()` a method in the `Thread` class or the `Object` class?
79. What is the Producer-Consumer problem in Java?
80. What is the difference between `volatile` and `synchronized`?
81. What are atomic variables?

---

**Concurrency:**

82. What is the difference between `Runnable` and `Callable`?
83. What is a `Future` object?
84. What is a `CompletableFuture`?
85. What is the use of the `done()`, `isCancelled()`, and `cancel()` methods of a `Future` object?
86. What is the `ThreadLocal` class?
87. What is a `CountDownLatch`?
88. What is a `CyclicBarrier`?
89. What is a `ReentrantLock`?
90. What is the difference between `ExecutorService.submit()` and `Executor.execute()`?
91. What are the different types of `ThreadExecutor` services?
92. Explain how a `FixedThreadPool` executor works.

---

**Java 8:**

93. What are the changes to interfaces in Java 8?
94. What is a functional interface? Why do we need it?
95. What is the difference between `Collection` and `Stream`?
96. What are terminal operators vs intermediate operators in Streams?
97. What is `Optional`?
98. What is the difference between `flatMap` and `map`?
99. What is the difference between parallel sort and regular sort?
100. What is the difference between `Predicate` and `BiPredicate`?
101. How is the Diamond problem solved in Java 8?

---

**Other:**

102. What is the difference between JDK, JRE, and JVM?
103. What is an immutable class?
104. What are the SOLID principles?
105. What is the difference between `ClassNotFoundException` and `NoClassDefFoundError`?
106. What is the Singleton Design pattern? Explain Thread-Safe Singleton and Bill Pugh Singleton. How can you break Singleton?
107. Explain the features in each Java version starting from Java 8.

---