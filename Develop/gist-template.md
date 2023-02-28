# Phone Number Regex Tutorial

Introductory paragraph (replace this with your text)

## Summary

Regex means "regular expression". A regex is an expression that can be used to search different patterns in text. Regex are extremely useful in programming as they can be used to filter, search, find, and replace text. This tutorial will focus on the following regex; `/(?:(\+1?)[ -]?)?\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})/g`. This regex is used to search and match different patterns of phone number entry and can be useful for a multitude of purposes, such as phone number input validity.

## Table of Contents

- [Phone Number Regex Tutorial](#phone-number-regex-tutorial)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [OR Operator](#or-operator)
    - [Character Classes](#character-classes)
    - [Flags](#flags)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Greedy and Lazy Match](#greedy-and-lazy-match)
    - [Boundaries](#boundaries)
    - [Back-references](#back-references)
    - [Look-ahead and Look-behind](#look-ahead-and-look-behind)
  - [Author](#author)

## Regex Components

### Anchors

Anchors search for text at the beginning and end of a string. The operators are `^` and `$`. However, these are not used in this regex.

### Quantifiers

There are several quantifiers used in this regex. This uses `{}` to define a set of 3 digits followed by another set of 3 digits followed lastly by a set of 4 digits. This also uses `?` to match numbers that may start with the country code `+1`, an area code of a set of 3 digits, or any set that may be followed by a space or a `-`. This way, the regex can find the phone number in many popular phone number entry formats.

### OR Operator

This regex uses `[]` as an OR operator to capture spaces or `-`.

### Character Classes

This entire regex uses `\d` in order to find digits for the phone number.

### Flags

The only flag necessary for this regex is `g`. This way, we can find multiple sets of numbers in the document we are searching.

### Grouping and Capturing

This regex makes use of `()` to capture the digits in the phone number, but avoids capturing characters that are not needed (such as the country code or spaces and hyphens).

### Bracket Expressions

This regex makes use of `[]` to find any spaces or `-` in the phone number sequence, but does not capture those characters.

### Greedy and Lazy Match

The only greedy operator used in this regex is the `{}` to define and capture a set of 3 digits.

### Boundaries

There are no boundaries used in this regex.

### Back-references

There are no back-references used in this regex.

### Look-ahead and Look-behind

There are no look-ahead or look-behind operators used in this regex.

## Author

The author, Ethan Gayton, is currently undergoing a full-stack boot camp in order to pursue his desired career path. For any questions or comments please contact him at his github profile linked [here](https://github.com/Ethikry).
