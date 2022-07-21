# Comments

| [Home](../../index.md) | [Section](./index.md) |

---

When writing code, there are times we want to leave a message for anyone else who will work with our code (or frequently for your future self). However we don't want those messages to affect the code. Luckily Java has comments.

Comments are messages left in code that are removed by the compiler before it creates the bytecode. In that way, there's no way they can have any effects on our code.

There are a few different kinds of comments

## Single-line Comments

The simplest kind of comment, it tells java to ignore anything from the ```//``` to the end of the line.

```java
// A one line comment
System.out.println("Hello!"); // Another one!
```

## Multi-line Comments

Tell Java to ignore everything from the opening ```/*``` to the closing ```*/```

```java
/*
This is a multi-line comment.
It can be written across more than one line.

Shocking!
*/

/* Although it doesn't have to be! */
```

## Javadoc Comments

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

## Summary

Comments are messages left in code, which the Java compiler is smart enough to remove.

Java provides three kinds of comments

- Single-line comments
- Multi-line comments
- Javadoc comments
