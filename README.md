# Regex Filing

This short Regex file will act as a tutorial on how to use and understand a "regular expression" (regex).

## Summary

Over the course summary of this Regex I will be covering the usecase of "Emails". Regex is a great tool to implement into your code
to help retrieve certain information from its source aswell as providing validity in your work. The content below will gloss over each element
in relation to Regular Expression.

* Example of Email Regular Expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

    Anchors in relation to Regex act as both the start and end of the line of code you wish to search for, syntax can vary depending on this search element.

    /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/
    in the above code the /^ and $/ as they are the start and end points for the entire Regex.

### Quantifiers

    Quantifiers are symbols that specify the required number of times your chosen characters must appear for a successful match or validation. Example Below.

    /^([a-z0-9_\.-]+)@([\da-z\.-]+).([a-z.]{2,6})$/
    In the above regex line where a quanrifier is being used. in the case of a-z0-9_\.- it is stating that a minimum of 1 of these are required before the @ symbol is implemented (example - car789@). 
    The second part ([\da-z\.-]+) must also follow the same constraints of digits, letters, hyphens, periods.

### Grouping Constructs

    In Regex the syntax used for grouping are rounded brackets (), any code within these brackets has to adhere to the constraints before continuing.

     /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

### Bracket Expressions

    In this scenario bracket expressions are used to enclose the characters you wish to match with your code. An example of this would be for abcd i would use [abcd], or any of those characters would be [a-d] or if i wanted those letters excluded and allow all others except those i would implement [^abcd] or [^a-d].

    /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

### Character Classes

    Character class just refers to the chosen characters you are searching for when using regex, whatever is withing square brackets becomes your character array.

    /^([a-z0-9_\.-]+)@([\da-z\.-]+).([a-z\.]{2,6})$/
    EG: [a-z0-9_\.-]

### The OR Operator

    Email regex doesnt contain this operation but an example of this would be the verticle lines as used in javascript coding " | ".

    EG: [a-z|0-8]
    the above examples requires letters a-z or the numbers 0-8.

### Character Escapes

    In relation to character escapes these are refrencing the backslashes "\" within the regex, it is used to rid special characters such as periods and/or dashes.

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
    
## Author

 GitHub - [Hyne-OS1](https://github.com/Hyne-OS1/)

## License

MIT License

Copyright (c) 2024 Hyne-OS1

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
