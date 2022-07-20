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

## Variables

## Comments
