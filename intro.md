
gradle

Java

It is the most used and popular backend programming lang.

What makes Java different is JVM.

Compiling a program creates a code that may run differently if the computers it's run on are different. This is not an issue for Java because of JVM.

JVM acts like a middle layer that can run code on any computer.

Java is extremely famous for desktop and business software developers.

What you can do with java-

Mobile application development, website development, database connectivity, image processing, GUI based programs, networking.

Companies that use java-

Airbnb, Uber, pin interest, linked in, Groupon, eBay, Evernote, Fitbit, HubSpot.

Spring-

spring is an enterprise Java framework. Most popular Java EE framework. It is an open-source java platform.

Spring boot-

It is used to create web application but can also be used from command-line applications. it is an open-source framework used to create microservices. it is a java based spring framework module that provides RAD(rapid application development).

JSF(Java server faces)-

it is the standard component-oriented UI framework for the Java EE platform. it is an MVC web framework that focuses on building user interfaces. in this, we are building component-based web interfaces.

maven

We can use maven to build docker for java web services

A maven is a build tool for enterprise java projects. it is an automation tool. it is a great project management tool that is based on POM. used for project build, dependency and documentation.

Java web service-

web service is a communication b/w client and server applications that are using the HTTP protocol. The JWS can be accessed by .NEt and PHP.

Use maven to build docker for java web services

Use an ArrayList for storing and accessing data, and LinkedList to manipulate data.

https://docs.oracle.com/javase/8/docs/api/

    setup
	Download and install the latest JDK from the official Oracle website.
	https://www.oracle.com/in/java/technologies/downloads/#jdk23-windows

JIT compiller

First, the Java source code (.java) conversion to byte code (.class) occurs with the help of the javac compiler.

Then, the .class files are loaded at run time by JVM and with the help of an interpreter, these are converted to machine understandable code.

JIT compiler is a part of JVM. When the JIT compiler is enabled, the JVM analyzes the method calls in the .class files and compiles them to get more efficient and native code. It also ensures that the prioritized method calls are optimized.

Once the above step is done, the JVM executes the optimized code directly instead of interpreting the code again. This increases the performance and speed of the execution.

.equals

This method is used for checking the equality of contents between two objects as per the specified business logic.

==

This operator is used for comparing addresses (or references), i.e checks if both the objects are pointing to the same memory location.

Stubby is the remote procedure call (RPC) mechanism widely used for communication between services in Google's distributed systems.

define and compile a service interface, including how to define parameters and application error codes
implement and test a simple server in both blocking (synchronous) and non-blocking (asynchronous) styles
implement a simple client in both blocking (synchronous) and non-blocking (asynchronous) styles, and test it using a mocking library

https://google.aip.dev/

gRPC is a high-performance, open-source RPC framework maintained by Google. gRPC is used for communication between services within Google's production infrastructure as well as across various deployment scenarios ranging from mobile to cloud.

gRPC consists of runtime libraries that provide client- and server-side functionality.

spanner database - gvp
Spanner is a distributed SQL database management and storage service developed by Google.

https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model

JUnit - unit testing

gRPC-Web nodejs

dapper tool

https://github.com/jbloch/effective-java-3e-source-code
effective java joshua bloch

concurrency and collections API

fundamental libraries:
java.lang, java.util, and java.io, and
subpackages such as java.util.concurrent and java.util.function.

Lambdas Items
Streams Items
Optionals Item
Default methods in interfaces Item
try-with-resources Item
@SafeVarargs Item
Modules Item

java versions -7

Official Release Name Nickname
JDK 1.0.x Java 1.0
JDK 1.1.x Java 1.1
Java 2 Platform, Standard Edition, v1.2 Java 2
Java 2 Platform, Standard Edition, v1.3 Java 3
Java 2 Platform, Standard Edition, v1.4 Java 4
Java 2 Platform, Standard Edition, v5.0 Java 5
Java Platform, Standard Edition 6 Java 6
Java Platform, Standard Edition 7 Java 7
Java Platform, Standard Edition 8 Java 8
Java Platform, Standard Edition 9 Java 9

The language supports four kinds of types:
interfaces (including
annotations),
classes (including enums),
arrays,
primitives.

The first three are
known as reference types. Class instances and arrays are objects; primitive values
are not. A class’s members consist of its fields, methods, member classes, and
member interfaces. A method’s signature consists of its name and the types of its
formal parameters; the signature does not include the method’s return type.

In Java 9, a module system was added to the platform. If a library makes use of
the module system, its exported API is the union of the exported APIs of all the
packages exported by the library’s module declaration

Creating and Destroying Objects
Consider static factory methods instead of constructors
One advantage of static factory methods is that, unlike constructors, they
have name.
A second advantage of static factory methods is that, unlike constructors,
they are not required to create a new object each time they’re invoked.
A third advantage of static factory methods is that, unlike constructors,
they can return an object of any subtype of their return type.
A fourth advantage of static factories is that the class of the returned
object can vary from call to call as a function of the input parameters.
A fifth advantage of static factories is that the class of the returned object
need not exist when the class containing the method is written.
Java Database Connectivity API (JDBC).
JDBC doesn’t use ServiceLoader

DriverManager.registerDriver is the
provider registration API, DriverManager.getConnection is the service access
API, and Driver is the service provider interface

The main limitation of providing only static factory methods is that
classes without public or protected constructors cannot be subclassed.
A second shortcoming of static factory methods is that they are hard for
programmers to find.

Javadoc tool

from—A type-conversion method that takes a single parameter and returns a
corresponding instance of this type, for example:
Date d = Date.from(instant);

of—An aggregation method that takes multiple parameters and returns an in￾stance of this type that incorporates them, for example:
Set faceCards = EnumSet.of(JACK, QUEEN, KING);

valueOf—A more verbose alternative to from and of, for example:
BigInteger prime = BigInteger.valueOf(Integer.MAX_VALUE);

instance or getInstance—Returns an instance that is described by its pa￾rameters (if any) but cannot be said to have the same value, for example:
StackWalker luke = StackWalker.getInstance(options);

create or newInstance—Like instance or getInstance, except that the
method guarantees that each call returns a new instance, for example:
Object newArray = Array.newInstance(classObject, arrayLen);

getType—Like getInstance, but used if the factory method is in a different
class. Type is the type of object returned by the factory method, for example:
FileStore fs = Files.getFileStore(path);

newType—Like newInstance, but used if the factory method is in a different
class. Type is the type of object returned by the factory method, for example:
BufferedReader br = Files.newBufferedReader(path);

type—A concise alternative to getType and newType, for example:
List litany = Collections.list(legacyLitany);

The Builder
pattern simulates named optional parameters as found in Python and Scala. The Builder pattern is well suited to class hierarchies.

functional interfaces, lambdas, and method references were added

java -version
javac Main.java -> complile the code
java Main

>javac --release 8 Test.java 

spring boot-
Java 17 or later
Gradle 7.5+ or Maven 3.5+

You can also import the code straight into your IDE:
Spring Tool Suite (STS)
IntelliJ IDEA
VSCode

Spring Boot offers a fast way to build applications. It looks at your classpath and at the beans you have configured, makes reasonable assumptions about what you are missing, and adds those items. With Spring Boot, you can focus more on business features and less on infrastructure.

in this There is no web.xml file, either. This web application is 100% pure Java and you did not have to deal with configuring any plumbing or infrastructure.

https://start.spring.io/

To run the application, run the following command in a terminal window (in the complete) directory:

./gradlew bootRun
If you use Maven, run the following command in a terminal window (in the complete) directory:

./mvnw spring-boot:run

web controller

Build an executable JAR

This Spring tutorial includes basic to advanced topics of Spring Boot, like Basics of Spring Boot, Spring Boot core, Spring Boot REST API, Spring Boot with Microservices, Spring Boot with Kafka, Spring Boot with Database and Data JPA

it provides a faster way to set up and an easier, configure, and run both simple and web-based applications. It is a combination of Spring Framework and Embedded Servers. The main goal of Spring Boot is to reduce development, unit test, and integration test time and in Spring Boot, there is no requirement for XML configuration.

Java Persistence Library(JPA).

https://www.programiz.com/java-programming/online-compiler/#google_vignette

1 consider static factory methods instead of constructors
2 2, Consider a builder when faced with many constructor parameters
3 3, Enforce the singleton property with a private constructor or an
enum type
4 4, Enforce noninstantiability with a private constructor
5 6, Avoid creating unnecessary objects
6 7, Eliminate obsolete object references
7 8, Avoid finalizers and cleaners
8 10, Obey the general contract when overriding equals
9 11, Always override hashCode when you override equals
10 12, Always override toString
11 13, Override clone judiciously
12 14, Consider implementing Comparable
13 15, Minimize the accessibility of classes and members
14 16, In public classes, use accessor methods, not public fields
15 17, Minimize mutability
16 18, Favor composition over inheritance
17 19, Design and document for inheritance or else prohibit it

20 Prefer interfaces to abstract classes
19 22, Use interfaces only to define types
20 23, Prefer class hierarchies to tagged classes
21 42, Prefer lambdas to anonymous classes
22 24, Favor static member classes over nonstatic
23 26, Don’t use raw types
24 27, Eliminate unchecked warnings
25 28, Prefer lists to arrays
26 29, Favor generic types
27 30, Favor generic methods
28 31, Use bounded wildcards to increase API flexibility
29 33, Consider typesafe heterogeneous containers
30 34, Use enums instead of int constants
31 35, Use instance fields instead of ordinals
32 36, Use EnumSet instead of bit fields
33 37, Use EnumMap instead of ordinal indexing
34 38, Emulate extensible enums with interfaces
35 39, Prefer annotations to naming patterns
36 40, Consistently use the Override annotation
37 41, Use marker interfaces to define types
38 49, Check parameters for validity
39 50, Make defensive copies when needed
40 51, Design method signatures carefully
41 52, Use overloading judiciously

42 Use varargs judiciously
43 54, Return empty collections or arrays, not nulls
44 56, Write doc comments for all exposed API elements
45 57, Minimize the scope of local variables
46 58, Prefer for-each loops to traditional for loops
47 59, Know and use the libraries
48 60, Avoid float and double if exact answers are required
49 61, Prefer primitive types to boxed primitives
50 62, Avoid strings where other types are more appropriate
51 63, Beware the performance of string concatenation
52 64, Refer to objects by their interfaces
53 65, Prefer interfaces to reflection
54 66, Use native methods judiciously
55 67, Optimize judiciously
56 68, Adhere to generally accepted naming conventions
57 69, Use exceptions only for exceptional conditions
58 70, Use checked exceptions for recoverable conditions and runtime
exceptions for programming errors
59 71, Avoid unnecessary use of checked exceptions
60 72, Favor the use of standard exceptions
61 73, Throw exceptions appropriate to the abstraction
62 74, Document all exceptions thrown by each method
63 75, Include failure-capture information in detail messages
64 76, Strive for failure atomicity
65 77, Don’t ignore exceptions

66, Synchronize access to shared mutable data
67 79, Avoid excessive synchronization
68 80, Prefer executors, tasks, and streams to threads
69 81, Prefer concurrency utilities to wait and notify
70 82, Document thread safety
71 83, Use lazy initialization judiciously
72 84, Don’t depend on the thread scheduler
73 (Retired)
74 85, Prefer alternatives to Java serialization
86, Implement Serializable with great caution
75 85, Prefer alternatives to Java serialization
87, Consider using a custom serialized form
76 85, Prefer alternatives to Java serialization
88, Write readObject methods defensively
77 85, Prefer alternatives to Java serialization
89, For instance control, prefer enum types to readResolve
78 85, Prefer alternatives to Java serialization
90, Consider serialization proxies instead of serialized instances