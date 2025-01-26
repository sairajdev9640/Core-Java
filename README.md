Strings:

Why are strings immutable in java?
How intern() works?
How many objects are created in Strings using string literals and new operator?
How string constant pool works?
Difference between equals and == operator?
Difference between string , string buffer and string builder.
Object:

Why is wrapper class required?
Methods of Object class?
Does java gives importance to primitive data types?
Is Java pass by value or pass by reference?
Oops

Types of oops
Composition vs Aggregation vs Association?
Function overloading vs overriding
Difference between Abstract class and Interface?
Can private method or static methods be overridden in Java?
Can main() method be overloaded?
Can Abstract class have main method?
Serialisation

What is Serialisation and Deserialisation?
Use of transient keyword?
Is it possible to serialise a class if its super class is not serialisable ?Can the class be still serialised and deserialised?
Answer: yes provided that non-serialisable super class has no args constructor which is involved at deserialisation to initialise the super class.

4. Can Uninitialised non serialised , non transient fields still be tolerated?Answer: yes

Cloning

What is marker interface?
What is shallow copy and Deep copy?
Exception

Difference between Error and Exception?
Checked vs Unchecked Exception?
Create custom Exception?
What is Runtime exception ?
How does JVM handle Exception?
Difference between Final, Finalise and Finally?
Super class of all exceptions?
Is throwable an interface?
When Finally block doesn’t get executed?
Can subclass throw higher checked exception than base class?
Can we throw an unchecked exception in child class if parent class doesn’t throw any exception?
Difference between throw and throws()
Usage of Enum

Why to use Enum?
Garbage collection

How does Garbage collection in Java works?
Collection

Array vs ArrayList?
ArrayList vs LinkedList? When to use which collection?
Fail Safe vs Fail Fast Iterators?
What is concurrent modification exception?
Internal working of HashMap
Java8 changes to HashMap
Why HashMap contains null key?
Is it Mandatory to have key immutable in HashMap?
Why to override equals() and hashcode() method?
HashSet vs LinkedHashSet vs TreeSet
What is the Internal Datastructure in TreeMap? How the elements are sorted?
HashMap vs ConcurrentHashMap
Comparable vs Comparator
What is blocking Queue?
What is Vector? When to use it?
MultiThreading

MultiThreading vs MultiProcessing vs MultiProgramming vs MultiTasking?
Life cycle of a Thread
Extends vs Runnable
yield() vs sleep() vs join() ?
wait() vs sleep() ?
why is join() method used?
Can we Override start() method in Thread?
Can we Override run() method?
Can we start the thread twice?
What is IllegalThreadStateException?
What happens if run() method is called without start()?
Why do we use ThreadPool?
What is Race Condition?
What is Synchronisation?Types of Synchronisation?
Object Level Locking vs Class Level Locking?
If there is 2 synchronised methods m1 and m2 in a class, can 2 different threads t1 and t2 call different methods(m1,m2) respectively on same object of class c at same time ?
Answer — No. Only 1 Thread can hold the lock on a object of a class.However the other non synchronised methods can be called on same object.
If a class has a synchronised method and non synchronised method, can multiple threads execute non synchronised methods?
Answer: yes. If a class has a synchronised method and non synchronised method , multiple threads can access non synchronised methods.
Can 2 threads call 2 different static synchronised methods of same class?
Answer : The static synchronised methods of same class always block each other as 1 lock per class exists. So no 2 static synchronised methods can execute at the same time.
Does static synchronised methods block a non synchronised methods?
Answer: No. The thread executing static synchronised method holds a lock on the class and the executing the non static synchronised method holds lock on the object on which the method has been called, these 2 locks are different and these threads dont block eachother.
Can Constructors be synchronised?
What is DeadLock?
What is Inter thread communication?Explain wait(),notify() and notifyall()?
What is IllegalMonitorStateException?
Which class does wait(),notify() and notifyall() method belong?
Explain few Thread class methods?is Sleep() a method in Thread class or Object class?
Producer Consumer Problem in Java?
Volatile vs Synchronised?
What are Atomic variables?
Concurrency

runnable vs callable ?
What is Future Object?
What is CompletableFuture?
Use of Done() , IsCancelled() and Cancel() method of Future Object?
Explain ThreadLocal class
What is CountDownLatch?
What is CyclicBarrier?
What is ReEntrant lock?
ExecutorService.submit() vs Executor.execute()?
Different types of ThreadExecutor Services?
Explain how FixedThreadPool executor works?
Java 8

Interface8 changes
What is Functional Interface? why do we need it?
Difference between Collection and Stream
What is Terminal Operator vs Intermediate operators?
What is Optional?
Flatmap vs Map?
Difference between Parallel sort vs sort
Difference between Predicate vs BiPredicate?
How Diamond problem is solved in Java8?
Other

Difference between JDK,JRE and JVM
What is Immutable class?
What are solid principles?
Difference between ClassNotFound vs NoClassDefError?
What is Singleton Design pattern?Explain ThreadSafe Singleton and Bill Pugh Singleton ?
How to break Singleton?
Explain few features in each Java versions starting from Java8
