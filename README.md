# CBHW-W17-Regex-Tutorial

Regex ( Regular expressions) is a string of text that allows you to creat patterns that help match, locate and manage combinations in text. 

## Summary

In this tutorial i'll be going through various components regarding regex and how they work with strings and patterns such as this email:
 

emailRegex = \b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}\b

we will go threw every component to shee how they work and why we are utilazing them.
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

Example: emailRegex = \b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,4}\b

### Anchors
Anchors match a position within a string, not a character.they match a position before, after, or between characters.

"^"= Beginning, "$"= End, "\b"= Word boundary, "\B"= Not word boundary 

### Quantifiers

Quantifiers specify how many instances of a character, string, or character class must be present in the input for a match to be found.

"+"= Plus: Matches 1 or more times

"*"= Star: Matches zero or more times

"{n,n}"= Quantifier: Matches the specified quantity {1,3} will match 1 to 3. {3} will match exactly 3. {3,} will match 3 or more.

### Grouping Constructs
Capturing groups create a sub-expression by placing an expression inside matching open and close parentheses.

"()"= Parenthesis aka capturing: Captures everything enclosed within it. It isolates part of the full match and assignes it an ID to be later referred to within the regex.

"\n"= Numeric referenc: Matches the results of a capture group. Example" \1 matches the results of the first capture group & \3 matches the third.

### Bracket Expressions

Bracket expressions are a list of characters and or character classes enclosed in brackets "[]".

this includes examples such as: [abc]= a,b,or c, [a-z]= a through z, and [^abc]= any charcters exept a,b or c. 

### Character Classes
A character class defines a set of characters, any one of which can occur in an input string for a match to succeed. There are a number of predefined character classes and you can also define your own sets.

"[ABC]"= Character set: Match any chracter in the set. 

"[^ABC]"= Negated set: Match any charachter that is not in the set.

"[A-Z]"= Range: Matches a chracter having a character code between the two specifide character inclusive. 

"."= Dot: Matches any chracter exept linebreeaks. equivalent to [^\n\r]

### The OR Operator
they match characters in text strings, such as to define patterns. Examples of Operators include: 

"^"= Matches the beginning of a string.

"$"= Matches the end of a string.

"..."= Captures values in the parentheses.

"[...]"= Matches anything within the brackets.

"[a-z]"= Matches lowercase characters between a and z.

"[0-9]"= Matches any number values between 0 and 9.

"{x}"= The exact number of times to match.

"{x,}"= The minimum number of times to match.

### Flags
Expression flags change how the expression is interpreted. earch parameters are delimeted by two slash characters /.../. there are 6 flags in javascript.

"i"= With this flag the search is case-insensitive: no difference between A and a (see the example below).

"g"= With this flag the search looks for all matches, without it – only the first match is returned.

"m"= Multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m").

"s"= Enables “dotall” mode, that allows a dot . to match newline character \n (covered in the chapter Character classes).

"u"= Enables full Unicode support. The flag enables correct processing of surrogate pairs. More about that in the chapter Unicode: flag "u" and class \p{...}.

"y"= “Sticky” mode: searching at the exact position in the text

### Character Escapes
Escape sequences can be used to insert reserved, special, and unicode characters. All escaped characters begin with the "\" character. here are a few examples of these charcters: 

"\\"= String literal match for \ character.

"\b"= Matches any zero-width word boundary, such as between a letter and a space.

"\B"= Matches any zero-width non-word boundary, such as between two letters or two spaces.

"\cX"= Matches a control character (CTRL + A-Z), where X is the corresponding letter in the alphabet.

"\d"= Matches any digit.

"\D"= Matches any non-digit.

"\f"= Matches a form feed.

## Author
* **Oscar Salgado** - [Git Hub Profile](https://github.com/Plavala)

Hi! My name is Oscar Salgado and I'm a new fullstack web developer! I'm excited to learn so much more!


