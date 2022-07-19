# Primitives

[Home](../index.md)

## Primitive Data Types

Java has eight primitive data types

| Type | Size(bits) | Range | Default |
| --- | --- | --- | --- |
| [byte](#byte) | 8 | -128 to 127 | 0 |
| [short](#short) | 16 | -32,768 to 32,767 | 0 |
| [int](#int) | 32 | -2,147,483,648 to 2,147,483,647 | 0 |
| [long](#long) | 64 | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | 0L |
| [float](#float) | 32 | 6 to 7 decimal digits | 0.0f |
| [double](#double) | 64 | 15 decimal digits | 0.0d |
| [boolean](#boolean) | 1 | *true* or *false* | false |
| [char](#char) | 2 | Unicode characters | '\u0000' |

### byte

```java
byte bytey = 100;
```

### short

```java
short shorty = 1_000;
```

### int

```java
int inty = 100_000_000;
```

### long

 A long value should end with the L (or l) distinguisher

```java
long long = 42l;
```

ints can also be stored, but dont do this.

```java
long long = 2147483647;
```
it will no longer compile when you exceed the maximum int value; this next line breaks!

```java
long long = 2147483648;
```
its simple to fix though, just make it a long using L (or l)

```
long long = 2147483648L;
```

### float

a float should usually end with an f

```java
float floaty = 1.234f;
```

### double

doubles can be specified with a d (or D), but its not necessary as this is the default

```java
double doubly = 1.2345678;
double moreDoubly = 1.2345678D;
```

### boolean

boolean is easy, it only has two possible values

```java
boolean truthy = true;
boolean falsy = false;
```

### char

since char is an integer representing a character it can also be assigned numbers

```java
# these two chars are equal
char chary = 'A';
char aLittleChary = 65;
```
