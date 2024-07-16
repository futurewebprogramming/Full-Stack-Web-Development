# Lecture - 07  Functions

## Sass String Functions
The string functions are used to manipulate and get information about strings.

Sass strings are 1-based. The first character in a string is at index 1, not 0.

The following table lists all string functions in Sass:

Function	Description & Example
quote(string)	Adds quotes to string, and returns the result.

Example:
```scss
quote(Hello world!)
Result: "Hello world!"
str-index(string, substring)	Returns the index of the first occurrence of the substring within string.
```
Example:
```scss
str-index("Hello world!", "H")
Result: 1
str-insert(string, insert, index)	Returns string with insert inserted at the specified index position.
```
Example:
```scss 
str-insert("Hello world!", " wonderful", 6)
Result: "Hello wonderful world!"
str-length(string)	Returns the length of string (in characters).
```
Example:
```scss
str-length("Hello world!")
Result: 12
str-slice(string, start, end)	Extracts characters from string; start at start and end at end, and returns the slice.
```
Example:
```scss
str-slice("Hello world!", 2, 5)
Result: "ello"
to-lower-case(string)	Returns a copy of string converted to lower case.
```
Example:
```scss
-lower-case("Hello World!")
Result: "hello world!"
to-upper-case(string)	Returns a copy of string converted to upper case.
```
Example:
```scss
to-upper-case("Hello World!")
Result: "HELLO WORLD!"
unique-id()	Returns a unique randomly generated unquoted string (guaranteed to be unique within the current sass session).
```
Example:
```scss
unique-id()
Result: tyghefnsv
unquote(string)	Removes quotes around string (if any), and returns the result.

```
Example:
```scss
unquote("Hello world!")
Result: Hello world!

```


# Sass Numeric Functions

The numeric functions are used to manipulate numeric values.

The following table lists all numeric functions in Sass:

Function	Description & Example
abs(number)	Returns the absolute value of number.

Example:
```scss 
abs(15)
Result: 15
abs(-15)
Result: 15
ceil(number)	Rounds number up to the nearest integer.
```

Example:
```scss
ceil(15.20)
Result: 16
comparable(num1, num2)	Returns whether num1 and num2 are comparable.

```

Example:
```scss
comparable(15px, 10px)
Result: true
comparable(20mm, 1cm)
Result: true
comparable(35px, 2em)
Result: false
floor(number)	Rounds number down to the nearest integer.

```

Example:
```scss
floor(15.80)
Result: 15
max(number...)	Returns the highest value of several numbers.

```


Example:
```scss
max(5, 7, 9, 0, -3, -7)
Result: 9
min(number...)	Returns the lowest value of several numbers.

```

Example:
```scss
min(5, 7, 9, 0, -3, -7)
Result: -7
percentage(number)	Converts number to a percentage (multiplies the number with 100).

```

Example:

```scss
percentage(1.2)
Result: 120
random()	Returns a random number between 0 and 1.

```

Example:
```scss
random()
Result: 0.45673
random(number)	Returns a random integer between 1 and number.


```

Example:

```scss
random(6)
Result: 4
round(number)	Rounds number to the nearest integer.

```

Example:
```scss
round(15.20)
Result: 15
round(15.80)
Result: 16
```


# Sass List Functions

The list functions are used to access values in a list, combine lists, and add items to lists.

Sass lists are immutable (they cannot change). So, the list functions that return a list, will return a new list, and not change the original list.

Sass lists are 1-based. The first list item in a list is at index 1, not 0.

The following table lists all list functions in Sass:

Function	Description & Example
```scss
(list, value, [separator])	Adds a single value to the end of the list. separator can be auto, comma, or space. auto is default.

```
Example:

```scss
append((a b c), d)
Result: a b c d
append((a b c), (d), comma)
Result: a, b, c, d
index(list, value)	Returns the index position for the value in list.

```

Example:

```scss
index(a b c, b)
Result: 2
index(a b c, f)
Result: null
is-bracketed(list)	Checks whether the list has square brackets.

```

Example:
```scss
is-bracketed([a b c])
Result: true
is-bracketed(a b c)
Result: false
join(list1, list2, [separator, bracketed])	Appends list2 to the end of list1. separator can be auto, comma, or space. auto is default (will use the separator in the first list). bracketed can be auto, true, or false. auto is default.

```

Example:
```scss
join(a b c, d e f)
Result: a b c d e f
join((a b c), (d e f), comma)
Result: a, b, c, d, e, f
join(a b c, d e f, $bracketed: true)
Result: [a b c d e f]
length(list)	Returns the length of the list.
```


Example:

```scss
length(a b c)
Result: 3
list-separator(list)	Returns the list separator used, as a string. Can be either space or comma.

```

Example:
```scss
list-separator(a b c)
Result: "space"
list-separator(a, b, c)
Result: "comma"
nth(list, n)	Returns the nth element in the list.

```

Example:
```scss
nth(a b c, 3)
Result: c
set-nth(list, n, value)	Sets the nth list element to the value specified.

```

Example:
```scss
set-nth(a b c, 2, x)
Result: a x c
zip(lists)	Combines lists into a single multidimensional list.

```

Example:
```scss
zip(1px 2px 3px, solid dashed dotted, red green blue)
Result: 1px solid red, 2px dashed green, 3px dotted blue
Sass List Functions
Sass List Functions
The list functions are used to access values in a list, combine lists, and add items to lists.

```

Sass lists are immutable (they cannot change). So, the list functions that return a list, will return a new list, and not change the original list.

Sass lists are 1-based. The first list item in a list is at index 1, not 0.

The following table lists all list functions in Sass:

Function	Description & Example
append(list, value, [separator])	Adds a single value to the end of the list. separator can be auto, comma, or space. auto is default.


Example:
```scss
append((a b c), d)
Result: a b c d
append((a b c), (d), comma)
Result: a, b, c, d
index(list, value)	Returns the index position for the value in list.

```

Example:
```scss

index(a b c, b)
Result: 2
index(a b c, f)
Result: null
is-bracketed(list)	Checks whether the list has square brackets.
```

Example:
```scss
is-bracketed([a b c])
Result: true
is-bracketed(a b c)
Result: false
join(list1, list2, [separator, bracketed])	Appends list2 to the end of list1. separator can be auto, comma, or space. auto is default (will use the separator in the first list). bracketed can be auto, true, or false. auto is default.

```

Example:
```scss
join(a b c, d e f)
Result: a b c d e f
join((a b c), (d e f), comma)
Result: a, b, c, d, e, f
join(a b c, d e f, $bracketed: true)
Result: [a b c d e f]
length(list)	Returns the length of the list.
```
Example:
```scss
length(a b c)
Result: 3
list-separator(list)	Returns the list separator used, as a string. Can be either space or comma.

```

Example:
```scss
list-separator(a b c)
Result: "space"
list-separator(a, b, c)
Result: "comma"
nth(list, n)	Returns the nth element in the list.
```
Example:
```scss
nth(a b c, 3)
Result: c
set-nth(list, n, value)	Sets the nth list element to the value specified.
```

Example:
```scss
set-nth(a b c, 2, x)
Result: a x c
zip(lists)	Combines lists into a single multidimensional list.

```

Example:
```scss
zip(1px 2px 3px, solid dashed dotted, red green blue)
Result: 1px solid red, 2px dashed green, 3px dotted blue
```



