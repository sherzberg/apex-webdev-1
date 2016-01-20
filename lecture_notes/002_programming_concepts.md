# Programming Concepts

### Goals

* Understand basic programming concepts
* Build simple computer programs
* Understand basic PHP syntax

### Exercises

The assessment this week will be to build a library of functions that
will aid in Geometry calculations. For example, we will have some code
that will be able to calculate the area of a circle.

## Execution

There are two main types of programs we will be running:

* Short running scripts
* Long running applications/services

All programs have both inputs and outputs. Inputs are used to change the
the execution and output of the running program. Outputs can be used to show
results or to be inputs to another program.

Create a file called `intro.php` and enter this as its contents:

```php
<?php

echo "Hello!";
?>
```

Now we can execute the script like this:

```bash
$ php intro.php
```

The php script was read in by the php interpreter and executed line by line.
Our `Hello!` should be displayed as output.

## Variables

Variables are used like lookup keys in a table of contents. They are references
to things in the program.

Variable syntax in PHP looks like this:

```php
$x = 5;

$thisIsMyVariable = 99;

$anotherVariable = "value";
```

## Data Types and Operators/Methods/Functions

Data Types are the classification and rules that apply to data.

For example, an `integer` type supports the classification of numeric whole
numbers. You can add, subtract, divide, and multiply integers.

There are many different Types and you can even create your own!

Here are some very common types we will use:

* Strings
* Integers
* Floating point numbers
* Arrays

Operators/methods/functions are the "things" you do to/with types. For another math
example, the `+` operator says you should add two numbers together.

## Boolean Algebra

Boolean algrebra relates to `truthy values` used in algebra. True and False in combinations
make up the boolean algebra notation.

There are three operations:

 - conjuction (and)
 - disjunction (or)
 - negation (not)

Some examples:

 - (true and false and true) == false.
 - (true or false or true) == true.

PHP examples:

```php
echo var_dump(true);
echo var_dump(false);
echo var_dump(false or true);
$first = false;
$second = true;
echo var_dump($first and $second);
```

This is useful, but what if we need to do something based on the result of
boolean algebra?

This is done with something called conditional statements. These come in many
forms in programming languages.

The common ones are:

 - if
 - else if
 - else

PHP examples:
```php
if (true and true) {
    echo "It is true!";
}

if (false) {
    echo "Nope!";
} else {
    echo "Yes!";
}

if (false) {
    echo "No"
} else if (true) {
    echo "Yes";
} else {
    echo "no";
}
```

## Iteration

We have talked about array data types (lists of elements). What if we need to
do something with each item in the array? This is called Iteration or Looping in computer
science.

PHP examples:

```php
$myarray = [0, 1, 2, 3, 4];

foreach ($myarray as $item) {
    echo $item;
}
```

We iterated or looped over the array to print out each one.

Another type of iteration is with a counter:

```php
for ($i=0; $i<10; $i++) {
    echo $i;
}
```

## Functions

Functions can be thought of a reusable blocks of code. They take inputs and provide outputs.

For example the `add` function can take two numbers and returns a single number.

PHP examples:

To declare a function we can simply use the `function` keyword:

```php
function add($first, $second) {
    return $first + $second;
}
```

To use it, it is equaly simple:

```php
echo add(5, 8);

$myVariable = 1;
echo add($myVariable, 9);
```
