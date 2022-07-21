
# Hello World

| [Home](../../index.md) | [Section](./index.md) |

___
The simplest Java program one can write looks something like this:

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```

There's a lot going on in just a few lines of code, but lets breakdown the key elements.

## class

In Java there is a set of reserved words that each have a special meaning. These are called **keywords**, and they cannot be used for anything else.

```class``` is a keyword that creates a new class. This is important to know because every line of Java code must live in a class.

## main(String[] args)

When Java code is running, it runs on something called the Java Virtual Machine (often just called the JVM for short).

The JVM needs a place to start when it begins running code. Thats where main(String[] args) comes in. It is the X that marks the spot for the JVM to begin executing code.

## System.out.println()

Now that the JVM can find our code, we want it to do something.

```System``` is a class that comes built-in to Java for us to use. In this case we are using it to print a line of code out.

The output from our program above looks like this:

```shell
Hello World!
```

## Compiling

Generally speaking, Java is a compiled languages. This means that before we can run our code, it is transformed by Java into something called **bytecode**. In turn, that is what the JVM runs.

We can do this easily using the command line.

Lets say we saved our above example in a file called 'HelloWorld.java'. We could run this command from the command line to compile it:

```powershell
javac .\HelloWorld.java
```

After running this the directory containing 'HelloWorld.java' should now contain a new file called 'HelloWorld.class'. That file is the compiled bytecode.

We can now run our code with this command:

```powershell
java .\HelloWorld
```

Note that we do not include the .class suffix.

We've now executed our code! In the command line you should see this output:

```powershell
Hello World
```

## Summary

All code in Java must be inside classes, which are declared using the aptly named **class** keyword.

Java compiles the code we write into bytecode. The **javac** command line tool does this. It is then run on the **Java Virtual Machine (JVM)**.

When the JVM executes our code, it starts from the code in **main(String[] args)**.
