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
long longy = 42l;
long longyq = 2147483648L;
```

### float

A float is a decimal value, and should always end with a f.

```java
float floaty = 1.234f;
```

### double

doubles can be specified with a d (or D), but its not necessary as they are the default for numeric decimal values.

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
// these two chars are equal
char chary = 'A';
char aLittleChary = 65;
```

## Literals

When a number is written out in the code, it is a literal.

For example, the number '100' below is a literal value:

```java
int literal = 100;
```

They can also use bases other than base 10

```java
// hexidecimal - 0x prefix
int hex = 0xBB;
// Octal - 0 prefix
int oct = 034;
// Binary - 0b prefix
int bin = 0b10;
```

### Types of Literals

#### Numerics

The byte, short, int, and long types hold numbers without any decimal places. These integral values are Java's numeric literals.

Numeric literals are all signed, meaning they reserve one bit to indicate if the number is positive or negative.

#### Floating Point

The float and double primitives represent floating point (decimal) values.

If a decimal is present in a numeric literal the compiler will assume it is a double unless it is marked with an F (or f).

#### String and Character literals

String (covered later) and char literals encode Unicode characters. Unicode values can be specified using the Unicode escape character \u followed by the encoding for the value.

```java
char example = '\u0108' // Ĉ
```

Always use 'single quotes' for char literals.

### Underscores for Formatting

As you saw in a few examples above, underscore '_' characters can be used in numeric literals to make them easier to read.

```java
short shorty = 1_000;
int inty = 100_000_000;
long longy 100_000_000_000_000L;
```

#### Illegal Underscore Usage

Underscores cannot go at the beginning, or the end, of a literal:

```java
int thisBreaks = _100_000_000;
int thisBreaksToo = 100_000_000_;
```

Right after, or right before, a decimal point:

```java
double thisBreaks = 12._123;
double thisBreaksToo = 12_.123;
```

Right before an F or L suffix:

```java
float thisBreaks = 42_f;
float thisBreaksToo = 42_L;
```

Finally, they cannot be used in a base prefix:

```java
int thisBreaks 0_x34;
```

#### Legal Underscore Usage

It is possible, but a little ugly, to have multiple underscores in a row:

```java
int legalButGross = 1_____________1; // 11
```

You can also use them in non-base 10 literals:

```java
int hex = 0xB_B;
```

## Summary

Java has 8 different primitives:

byte, short, int, long, float, double, char, and boolean.

When primitives are assigned a value, a number or character is written directly in the code to specify its value. Those numbers or characters are called literals.

- The numeric literals are byte, short, int, and long
- The floating point literals are float and double
- The character literal is char
- Finally, the boolean literal is simply true or false

Numeric literals can have underscores in them to help with formatting.
