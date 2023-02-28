# Phone Number Regex Tutorial

Welcome to this regex tutorial. This will be a brief description of how the following regex works. The explanation will include the different operator types that are used in the expression, along with a brief summary describing how the regex may be used.

## Summary

Regex means "regular expression". A regex is an expression that can be used to search different patterns in text. Regex are extremely useful in programming as they can be used to filter, search, find, and replace text. This tutorial will focus on the following regex; `/(?:(\+1?)[ -]?)?\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})/g`. This regex is used to search and match different patterns of phone number entry and can be useful for a multitude of purposes, such as phone number input validity.

## Table of Contents

- [Phone Number Regex Tutorial](#phone-number-regex-tutorial)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Quantifiers](#quantifiers)
    - [OR Operator](#or-operator)
    - [Character Classes](#character-classes)
    - [Flags](#flags)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Greedy and Lazy Match](#greedy-and-lazy-match)
  - [Author](#author)

## Regex Components

### Quantifiers

There are several quantifiers used in this regex. This uses `{}` to define a set of 3 digits followed by another set of 3 digits followed lastly by a set of 4 digits. This also uses `?` to match numbers that may start with the country code `+1`, an area code of a set of 3 digits, or any set that may be followed by a space or a `-`. This way, the regex can find the phone number in many popular phone number entry formats. For example, the `\(?(\d{3})\)?[ -]?` section of the regex uses the `\(?` and `\)?` to match the `()` if they are used for the area code, but does not require them. The same goes for the `(\d{3})\)?` and `[ -]?` sections. This means that the area code is not necessary, but the regex will capture it if it exists. The space and `-` are okay if they are present as well, but do not need to be captured since they are not part of the number. Next, the `(\d{3})` section utilizes the `{}` to capture a set of 3 digits and again later in the regex for the string of 4 digits.

### OR Operator

This regex uses `[]` as an OR operator to capture spaces or `-`, as seen in the `[ -]` section of the regex.

### Character Classes

This entire regex uses `\d` in order to find digits for the phone number.

### Flags

The only flag necessary for this regex is `g`. This way, we can find multiple sets of numbers in the document we are searching instead of just the first time it is found.

### Grouping and Capturing

This regex makes use of `()` to capture the digits in the phone number, but avoids capturing characters that are not needed (such as the country code or spaces and hyphens). The regex can be used to change, find, or replace these strings that it has captured.

### Bracket Expressions

This regex makes use of `[]` to find any spaces or `-` in the phone number sequence, but does not capture those characters since they are not needed for the phone number.

### Greedy and Lazy Match

The only greedy operator used in this regex is the `{}` to define and capture a set of 3 digits. This helps to find separate strings if they are broken up with spaces or hyphens, but will still find the full number in any format.

## Author

The author, Ethan Gayton, is currently undergoing a full-stack boot camp in order to pursue his desired career path. For any questions or comments please contact him at his github profile linked [here](https://github.com/Ethikry).
