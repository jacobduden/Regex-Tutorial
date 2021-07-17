# Regex-Tutorial

This is a mini tutorial explaining an example of a regex expression.

## Summary

A regular expression is a sequence of characters that defines a search pattern for a body of text.
An example:
* Matching a URL &ndash; `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

An anchor doesn't match any characters. The purpose behind anchors is to match a position within the text before, or after a specific character. ("^" is for use of the begining of the text)("$" is for use at the end of the text). In the example above, you'll see `/^(https?:\`), indicating that the text coming back requires https?: to be at the begging of the url.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. In the example above, /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]`*)*`, the "*" indicates that it requires 0 or 1 more instance. if it were followed by a number, it would require that many more instances.

### Character Classes

Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits. In our example, `\da-z`, "/d' stands for matching one digit. So our expression requires at least 1 digit/character between a-z.

### Grouping and Capturing

Non-capturing parentheses group the regex so you can apply regex operators, but do not capture anything. Our example, `https?:\/\/`.

### Bracket Expressions

A bracket expression is either a matching list expression or a non-matching list expression. Our example, `[a-z\.]`, matching any character a through z.

## Author

## Jacob duden

* [Author's GitHub](https://github.com/jacobduden)