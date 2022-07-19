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
long long = 2147483648L;
```

### float

float and double are used for floating point (decimal) values. A float should end with a f.

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

## Working with literals

### Literals

When a number is written out in the code, it is a literal.

For example, the number '100' below is a literal value:

```java
int literal = 100;
```

They can also use bases other than base 10

```java
# hexidecimal - 0x prefix
int hex = 0xBB;
# Octal - 0 prefix
int oct = 034;
# Binary - 0b prefix
int bin = 0b10;
```

### Underscores

As you saw in a few examples above, underscore(_) characters can be used in numeric literals to make them easier to read.

```java
short shorty = 1_000;
int inty = 100_000_000;
long longy 100_000_000_000_000L;
```

#### Underscores can go anywhere except in a literal, except

at the beginning, or the end, of a literal:

```java
int illegalInt1 = _100_000_000; // BREAKS!
int illegalInt2 = 100_000_000_; // BREAKS!
```

right after, or right before, a decimal point:

```java
double illegalDouble1 = 12._123; // BREAKS!
double illegalDouble2 = 12_.123; // BREAKS!
```

It is legal to use multiple undescores in row

```java
int legalButGross = 1_____________1; // 11
```
