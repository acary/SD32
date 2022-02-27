[comment]: # (This presentation was made with markdown-slides)
[comment]: # (This is a CommonMark compliant comment. It will not be included in the presentation.)
[comment]: # (Compile this presentation with the command below)
[comment]: # (mdslides presentation.md --include media)

[comment]: # (Set the theme:)
[comment]: # (THEME = white)
[comment]: # (CODE_THEME = base16/zenburn)
[comment]: # (The list of themes is at https://revealjs.com/themes/)
[comment]: # (The list of code themes is at https://highlightjs.org/)

[comment]: # "You can also use quotes instead of parenthesis"
[comment]: # "THEME = white"

[comment]: # (Pass optional settings to reveal.js:)
[comment]: # (controls: true)
[comment]: # (keyboard: true)
[comment]: # (markdown: { smartypants: true })
[comment]: # (hash: false)
[comment]: # (respondToHashChanges: false)
[comment]: # (Other settings are documented at https://revealjs.com/config/)

SD32 | Skill Distillery | February 19, 2022

# SD32

Topics by week

[comment]: # (!!!)

# Week 1

[comment]: # (!!!)

# Day 1

[comment]: # (!!!)

### Data types

```
int
double
char
boolean
String
```

### Default values

`boolean` : `false`

[comment]: # (!!!)

***Variables***: declaration, assignment

***Literals***: constant value

[comment]: # (!!!)

### Class

```
class Name {...}
```

[comment]: # (!!!)

## Main method:

```
public static void main(String[] args) {...}
```

[comment]: # (!!!)

# Day 2

[comment]: # (!!!)

## Assignment

(variable) `=` (value or expression)

[comment]: # (!!!)

## Operators

Equality

```
==
!=
```

Conditional

```
&&
||
```

[comment]: # (!!!)

### Screen input

***Scanner***

```
import java.util.Scanner;
Scanner sc = new Scanner(System.in);
```

### Screen output

```
System.out.print()
System.out.println()
```

[comment]: # (!!!)

# Day 3

[comment]: # (!!!)

## Expression

Evaluates to a single value

[comment]: # (!!!)

Operators:

`=, +=, -=, *=, %=`

Arithmetic:

`+, -, *, %, ==`

Auto-Increment:

`++, --`

[comment]: # (!!!)

## Eclipse IDE

- navigation
- shortcuts

[comment]: # (!!!)

## Control flow

```
if (condition) {..}
else if (condition) {...}
else {...}
```

[comment]: # (!!!)

## String comparison

`.equals`

`fName.equals(lName)`

[comment]: # (!!!)

# Day 4

[comment]: # (!!!)

***Boolean***:

`true` or `false`

***Ternary operator***:

`condition ? true : false`

[comment]: # (!!!)

***Switch***:

```
switch (onVariable) {
case 1: ...;
default: ...}
```

[comment]: # (!!!)

***While***:
- `while (boolean condition) {...}`

***Do-while***:
- `do {...} while (condition)`

[comment]: # (!!!)

## Pair Programming

- Driver
- Navigator

[comment]: # (!!!)

## Methods:

`methodName() {...}`

[comment]: # (!!!)

## For loops:

`for (int i = 0; i <= 10; i++) {...}`

[comment]: # (!!!)

***Break***:

- `break` escapes loop

***Continue***:

- `continue` passes control to next iteration

[comment]: # (!!!)

# Day 5

[comment]: # (!!!)

## Number systems:

- binary (base2)
- octal (base8)
- decimal (base10)
- hexadecimal (base16)

[comment]: # (!!!)

## printf():

- print formatted strings

[comment]: # (!!!)

### More on Data types

Switch and data types

Casting data types:
- implicit, explicit conversions
- `(int)`

[comment]: # (!!!)

# Day 6

[comment]: # (!!!)

***Scaler***: hold one value

***Arrays***: collection of multiple values (same data type)

[comment]: # (!!!)

## Arrays

Operator: []

```
int arrayOfInts[];
int[] arrayOfInts;
```

[comment]: # (!!!)

## Array Shortcut

```
String[] weekday = {"Monday", "Tuesday", "Wednesday", "Thursday", "Friday"};
char[] classGrades = {'A', 'B', 'C', 'A', 'B', 'C'};
double[] avgMonthPrecip = {123.45, 321.54, 54.45};
```

[comment]: # (!!!)

## Instantiate

`new` keyword

```
String[] weekdays = new String[7]; // 0..6
char grades[] = new char[6]; // 0..5
```

[comment]: # (!!!)

## Default values

```
int: 0
double: 0.0
char: \u0000
boolean: false
objects: null
```

[comment]: # (!!!)

## Objects

- `static`: belong to class, not instance

[comment]: # (!!!)

## Strings

```
.equals(String anotherString)
.equalsIgnoreCase(String anotherString)
.charAt(int index)
.toLowerCase()
.toUpperCase()
```

[comment]: # (!!!)

# Day 7

[comment]: # (!!!)

### Class Instantiation

```
NameGenerator nameGen = new NameGenerator();
String newFirstName = nameGen.generateFirstName(firstName);
```

[comment]: # (!!!)

### Character Array

`char[] charsInName = name.toUpperCase().toCharArray();`

[comment]: # (!!!)

### Modulo

`generatedName = names[index % names.length];`

[comment]: # (!!!)

### For Each Loop

```
int[] odds = {1, 3, 5, 7}
for (int num : odds) {
    System.out.println(num);
}

String[] strings = new String[4];
for (String s : strings) {
    System.out.prin(s + " ");
}
```

[comment]: # (!!!)

## Break and Continue

- break: breaks out of loop
- continue: proceeds to next iteration

[comment]: # (!!!)

# Advanced Arrays

[comment]: # (!!!)

## Two-dimensional arrays

- [row][column]
- `int[][] arr2d = new int[5][5];`

[comment]: # (!!!)

## For each

```
char[] board[] = new char[3][]
for (char[] row : board) {
    for (char element : row) {
        System.out.print(element);
    }
    System.out.println();
}
```

[comment]: # (!!!)

Creation shortcuts

```
String[] lz = {"Robert", "Jimmy", "John"};
String[] im = {"Bruce", "Nicko", "Janick"};
String[] gnr = {"Axel", "Slash", "Izzy"};
String[][] = {lz, im, gnr};
```

[comment]: # (!!!)

Creation shortcuts

```
String[][] legends = {
  {"Robert", "Jimmy", "John"},
  {"Bruce", "Nicko", "Janick"},
  {"Axel", "Slash", "Izzy"};
};
```

[comment]: # (!!!)

## Varargs

- must be last parameter in method

`public static void main(String... stringArr) {...}`

[comment]: # (!!!)

### Varargs

```
public void doIt(int... ints) {
    for (int i = 0; i < ints.length; i++) {
        System.out.println(ints[i]);
    }
}
```

[comment]: # (!!!)

# Appendices

[comment]: # (!!!)

# Eclipse shortcuts

- Autosuggest: `CTRL + Space`
- Format: `CMD + Shift + F`
- Import automatically: `CMD + Shift + O`
- Run program: `CMD + Shift + Fn + F11`

[comment]: # (!!!)

# Eclipse shortcuts

- Delete line: `CMD + D`
- Move line up: `Option + Up/Down arrow`
- Duplicate line: `CMD + Option + Up/Down arrow`

[comment]: # (!!!)

# Git shortcuts

- Initialize: `git init`
- Add: `git add .`
- Commit: `git commit -m "commit message"`
- Push: `git push`

[comment]: # (!!!)
