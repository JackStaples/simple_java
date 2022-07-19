# Primitives

[Home](../index.md)

Java has eight **primitive data types**

| Data Type | Size(bits) | Range | Default Value |
| --- | --- | --- | --- |
| [byte](#byte) | 8 | -128 to 127 | 0 |
| [short](#short) | 16 | -32,768 to 32,767 | 0 |
| [int](#int) | 32 | -2,147,483,648 to 2,147,483,647 | 0 |
| [long](#long) | 64 | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | 0L |
| [float](#float) | 32 | 6 to 7 decimal digits | 0.0f |
| [double](#double) | 64 | 15 decimal digits | 0.0d |
| [boolean](#boolean) | 1 | *true* or *false* | false |
| [char](#char) | 2 | Unicode characters | '\u0000' |

## byte

```java
byte bytey = 100;
```

## short

```java
short shorty = 1_000;
```

## int

```java
int inty = 100_000_000;
```

## long

```java
# A long value should end with the L (or l) distinguisher
long long = 42l;
# ints can also be stored, but dont do this
long long = 2147483647;
# it will no longer compile when you exceed the maximum int value; this next line breaks!
long long = 2147483648;
# its simple to fix though, just use L (or l)
long long = 2147483648L;
```

## float

```java
# a float should usually end with an f
float floaty = 1.234f;
```

## double

```java
# doubles can be specified with a d (or D), but its not necessary as this is the default
double doubly = 1.2345678;
double moreDoubly = 1.2345678D;
```

## boolean

```java
# boolean is easy, it only has two possible values
boolean truthy = true;
boolean falsy = false;
```

## char

```java
char chary = 'A';
# since char is an integer representing a character it can also be assigned numbers
char aLittleChary = 65;
# these two chars are equal
```
