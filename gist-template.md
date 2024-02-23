# Hex Value Regex Tutorial

Regex (or Regular Expressions) are used to decipher and qualify a search of text. These expressions use various componants to define the search, whether it is a literal search or a meta character search that defines the type of character the user is looking for. These regular expressions are broken down into definable componants that help navigate text. 

## Summary

In this tutorial we will disect then different componants of a Hex Value Regex. A Hex Value Regex defines the characters that can be used to look up a hex color. This can be used in everyday coding to require nessisary chartacters and alert the user if what is entered in not valid. We will be taking a look at the following regx:

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

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

* Anchors define the start and the begining of the regular expression that will be used in the search. Firstly, a rejex is consitered a literal, so the entire expression is wrapped in slashes `/`. The anchors are the next componants within the literal. The character `^` defines the start of the expression, while `$` defines the end.

### Quantifiers

* Quantifiers are the componants of the regex that set the limits to the search. Quanitfiers are usually defined within curl brakets `{}`. Symbols like `*` `+` and `?` all define specific search parameters in a more generic sence. In our hex value regex we see both a `{}` value and the `?` sypmbol. The curly brakets specify a specific range (eg. between 2 and 27), and the `?` sypmbol requires a match of zero or one time.

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
