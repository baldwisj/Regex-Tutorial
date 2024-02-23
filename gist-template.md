# Hex Value Regex Tutorial

Regex (or Regular Expressions) are used to decipher and qualify a search of text. These expressions use various components to define the search, whether it is a literal search or a meta character search that defines the type of character the user is looking for. These regular expressions are broken down into definable components that help navigate text. 

## Summary

In this tutorial we will disect then different components of a Hex Value Regex. A Hex Value Regex defines the characters that can be used to look up a hex color. This can be used in everyday coding to require nessisary chartacters and alert the user if what is entered in not valid. We will be taking a look at the following regx:

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

* Anchors define the start and the begining of the regular expression that will be used in the search. Firstly, a rejex is consitered a literal, so the entire expression is wrapped in slashes `/`. The anchors are the next components within the literal. The character `^` defines the start of the expression, while `$` defines the end.

* In the hex value regex above we can see the entire expression wrapped in these anchors: `/^...ext...$/`

### Quantifiers

* Quantifiers are the components of the regex that set the limits to the search. There are four types of quantifiers:
 * The `*` symbol quanifies the search to match the pattern zero or more times.
 * The `+` symbol quanifies the search to match the pattern one ore more times.
 * The `?` symbol quanifies the search to match the pattern zero or one time.
 * The `{}` quanitfiers specify a specific range (eg. between 2 and 27).

* In our regex we see the `?` symbol used. This tells us that everything in the group preceding it will be matched zero or one time.
* We also see two different `{}` expressions, `{6}`and `{3}`. Both of these quantifiers define a rigid number of characters to returned, wither 6 or 3.

### Grouping Constructs

* Grouping constructs are used to isolate certain aspecs of the regex. As the expressions get more complex, this become more nessisary.
Parentheses `()` are used to group constructs within the regex. If, for instance, it is nessisary to find two componants each of which have different parameters, we have to use grouping. For example, if I would like to find one number first from 6 to 9 and another number second from 2 to 8 we could write the expression `/^(([6-9]?)([2-8]?)$/`.

* In our regex we can see almost the entire expression is wrapped in a grouping constraint. In this case, we see `#` outside of the group. This is a literal, meaning this will literally search for the `#` symbol. After that, everything preceding the `?` will be found zero or once and returned after the `#`.

### Bracket Expressions

* In the previous section, you may have noticed the use of `[]`; these are bracket expressions. Bracket expressions are used to define a set of characters that can match any individual character of the set. Use an use these to create a range or list of characters you want met.

* in our hex regex we can see two bracket expressions, both displayed as`[a-f0-9]`. The only difference is the quantifiers are determining different lengths.

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
