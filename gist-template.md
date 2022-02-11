# Regex Tutorial: Matching an Email

Email Regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary

The Regex I will be targeting will be an Email Regex, using the information below, we will be able to understand this string of code and its structure.

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
The anchors of the expression begin with "^" which starts the string and the "$" is what ends the string.
### Quantifiers
The quantifier "+" connects the user's email name + email service + .com. {2,6} is also a quantifier which allows a match range of 2-6 characters for this character set: [a-z.].
### Grouping Constructs
Capturing group 1: [a-z0-9_.-] -- matches the user's email name Capturing group 2: ([\da-z.-]+) -- matches the email service Capturing group 3: ([a-z.]{2,6}) -- captures the .com
### Bracket Expressions
[a-z0-9_.-]-- matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."

[\da-z.-] -- matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".

[a-z.] --matching any character a-z (case senstive) and the character "."
### Character Classes
\d and \w are commonly used Character Classes denoting a match for any single character being a digit and a wildcase search respectively . See above Bracket Expression for an example.
### The OR Operator
| symbolizes the OR or 'Alternate' operator which essentially performs a either match whatever's to the left or right of the '|'.
### Flags
/ delimits regular expressions and are commonly seen at the beginning and/or at the end and at times after anchors too. This is used to identify search criteria outside of the Flags to help mark the expression as global (g), insensitive (i) or multi-line (m).
### Character Escapes
\ is a character escape functionality used to strip any special character and turn it into a literal
## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
