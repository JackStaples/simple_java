# Basics

[Home](../index.md)

## Hello World

The simplest Java program one can write looks something like this:

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```

There's a lot going on in just a few lines of code, but lets breakdown the key elements.

### class

In Java there is a set of reserved words that each have a special meaning. These are called **keywords**, and they cannot be used for anything else.

```class``` is a keyword that declares, not so surprisingly, a new class. This is important to know because every line of Java code must live in a class.

### main(String[] args)

When Java code is running, it runs on something called the Java Virtual Machine (often just called the JVM for short).

The JVM needs a place to start when it begins running code. Thats where main(String[] args) comes in. It is the X that marks the spot for the JVM to begin executing code.

### System.out.println()

Now that the JVM can find our code, we want it to do something.

```System``` is a class that comes built-in to Java for us to use. In this case we are using it to print a line of code out.

The output from our program above looks like this:

```shell
Hello World!
```

## Compiling

Generally speaking, Java is a compiled languages. This means that before the code we write can be run, it is read in and turned into something called **bytecode**. In turn, that is what the JVM runs.

We can do this ourselves using the command line.

Lets say we saved our above example in a file called 'HelloWorld.java'. We could run this command from the command line to compile it:

```powershell
javac .\HelloWorld.java
```

After running this the directory containing 'HelloWorld.java' should now contain a new file called 'HelloWorld.class'. That file is the compiled bytecode.

We can now run our code with this command:

```powershell
java .\HelloWorld
```

Note that we do not include the .class suffix when running.

We've now executed our code! In the command line you should see this output:

```powershell
Hello World
```

## Comments

When writing code, there are times we want to leave a message for anyone else who will work with our code (or frequently for your future self). However we don't want those messages to affect the code. Luckily Java has comments.

Comments are messages left in code that are removed by the compiler before it creates the bytecode. In that way, there's no way they can have any effects on our code.

There are a few different kinds of comments

### Single-line Comments

The simplest kind of comment, it tells java to ignore anything from the ```//``` to the end of the line.

```java
// A one line comment
System.out.println("Hello!"); // Another one!
```

### Multi-line Comments

Tell Java to ignore everything from the opening ```/*``` to the closing ```*/```

```java
/*
This is a multi-line comment.
It can be written across more than one line.

Shocking!
*/

/* Although it doesn't have to be! */
```

### Javadoc Comments

Java also comes with a tool that lets you automatically generate HTML documentation for your code. It uses the javadoc comments in the code for that documentation

```java
/** 
* Simple class that prints out "Hello World!"
* @author jackstaples
* @version 1.0.0
* @since 2022-07-19
*/
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```

## Variables
