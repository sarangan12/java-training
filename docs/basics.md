## How is a Java program executed?
A Java program is written as a simple text file and ends with a .java extension. Now, this program is compiled and converted to a .class file. This file will be in bytecode format. This class file will be executed on the Java Virtual Machine. 

## Why is Java platform independent?
A Java program is compiled to a class file format. This class file is not executed directly on the physical machine. It is executed on the virtual machine which resides over the physical machine. Each platform has its own virtual machine implementation. But, all of those implementation could understand the class file's bytecode and will be able to execute the Java program. Thus, a Java program written once could be executed on any platform. So, Java is platform independent. 

## What are some of the properties of Java?
Java programs have the following properties:
    1. Object Oriented
    2. Encapsulation
    3. Abstraction
    4. Inheritance
    5. Polymorphism
    6. Platform Independent

## What is JVM?
JVM stands for Java Virtual Machine. The compiled Java programs, i.e. class files in bytecode format, are executed on the Java Virtual Machine. 

## What is ClassLoader?
ClassLoader is a component of JVM which is used to load the classes. There are different types of class loaders such as Bootstrap classloader, Extension classloader, System classloader, Plugin classloader.

## What is JRE?
JRE stands for Java Runtime Environment. This provides the environment for the Java programs to execute. This consists of:
    1. Java Virtual Machine
    2. Set of Libraries to be used for execution of Java programs. 

## What is JDK?
JDK stands for Java Development Kit. This JDK consists 
    1. Java development tools such as javac (Java Compiler)
    2. Java Runtime environment. 
This is required only for 'development' of Java programs. 

## What is the difference between JDK, JRE & JVM? 
JDK is the development kit used for development and required only by developers. JRE is the Java Runtime environment. JVM is the Java Virtual Machine.
    JDK -> Java Development Tools + JRE
    JRE -> JVM + Libraries
    