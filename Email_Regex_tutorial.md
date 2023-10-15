# Email Regex Tutorial; Computer Science for JavaScript

This is a tutorial that explains how an expression, or regex, functions by breaking down each part of the expression and describing what it does; more importantly the tutorial mostly `focuses on the regex expression below`.

Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
> **Important**: The above regular expression can be used to verify that a user enters a valid email.


## Summary

A **regex**, which is short for **regular expression**, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

### Quantifiers

In **Regex** Quantifiers are used to quantify how many times a part of your regular expression should be repeated. 

When you want to repeat something in a regex search, whether it is an individual character, a character class or a sub-expression; Use a quantifier after it to specify how many times it should be repeated.

In the Email expression focused, there are four **Quantifiers** 

* `^n   `	-    Matches any string with n at the beginning of it
* `n+   `	-    Matches any string that contains at least one n
* `n{X,Y} `-	 Matches any string that contains a sequence of X to Y n's
* `n$   `	-    Matches any string with n at the end of it

### Grouping Constructs


In regular expressions (regex), **grouping constructs** are used to group together characters, subpatterns, or expressions. They serve several purposes:

* Parentheses () are the most common grouping construct. `For example, (abc)+ captures and references repetitions of "abc" in a string.`

    * 1st Capturing Group is `([a-z0-9_\.-]+)`
    * 2nd Capturing Group `([\da-z\.-]+)`
    * 3rd Capturing Group `([a-z\.]{2,6})`

### Bracket Expressions

Bracket expressions in regular expressions (regex) are used to define a character class, which matches any single character from the characters listed within the brackets. For example,  `[0-9] matches any digit`.

* Matching characters(white) present in the list in 1st Group Construct **`[`a-z0-9`_\.-]`**
    * `a-z` matches a single character in the range between a and z `(case sensitive)`
    * `0-9` matches a single character in the range between 0 and 9 `(case sensitive)`


### Character Classes

Character classes in regular expressions (regex) are a way to represent a group of characters with a single character class symbol. For example: `\w matches any word character (letters, digits, or underscore).`

* Matching a single characters(white) present in the list in 1st Group Construct **`[a-z0-9`_\\.-`]`**
    * `_ `matches the character _ literally `(case sensitive)`
    * `\.` matches the character . literally `(case sensitive)`
    * `-` matches the character - literally `(case sensitive)`
<br>
<br>
* Matching a single characters(white) present in the list in 2st Group Construct **`[\da-z`\\.-`]`*
    * `\.` matches the character . literally `(case sensitive)`
    * `-` matches the character - literally `(case sensitive)`
<br>
<br>
* Matching a single characters(white) present in the list in 3rd Group Construct **`[a-z`\\.`]`*
    * `\.` matches the character . literally `(case sensitive)`

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

## Resource
[how to create a gist](https://help.github.com/en/github/writing-on-github/creating-gists)
[video on how to use gists](https://www.youtube.com/watch?v=wc2NlcWjQHw).
