# 1 - Functional Interfaces

| [Home](../../index.md) |

---

A functional interface is an interfaces that contains only one method.

For example:

```java
public interface functionalInterface {
    public void doSomething();
}
```

As they only have one method to implement, they are also know as Single Abstract Method (SAM) interfaces.

## Lambda Expressions

Methods are bulky, they require alot of code and need to be attached to objects. Alternatively, lambda expressions can be used. They allow us to create nameless functions that can be passed around in code.

