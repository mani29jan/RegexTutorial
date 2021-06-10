# Title

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

## Summary

The regex you will be describing today is  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

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

## Regex Components

### Anchors
Matches at the start of the string the regex pattern is applied to.
Example- ^ to start, and $ to finish

### Quantifiers
Quantifiers are used to quantify how many times a part of your regular expression should be repeated.
In this example we used {2,6} to make sure the input would be minimum of 2 characters to a maximum of 6 and also added + to make sure there is another sequence to be matched. Both of these are greedy quantifier.

### Character Classes
In this example Character Classes confirms that Javascript classifies the use of any digit from 0-9 by using /d.

### Grouping and Capturing
This example contains three groups, group 1 would be the username of the email [a-z0-9_\.- ], group 2 would be [\da-z\.-] that collects the domain name or the service being used for the email, and group 3 would be [a-z\.]{2,6} that confirms that the email extension ends with .com or .net

### Bracket Expressions
Similarly as the groups in this model, there are additionally 3 bracket expressions. The data in the bracket expressions is opened and shut between these brackets []. This identifies which data is permitted to be matched.

group 1: [a-z0-9_\.- ] - incorporates case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

group 2: [\da-z\.- ] - incorporates all digits, case sensitive characters from a-z, periods and hyphens

group 3: [a-z\.] - incorporates case sensitive characters from a-z and periods.

### Greedy and Lazy Match
In this model we have just utilized greedy quantifiers + and {}, implying that it will permit the match to extend as long as it needs to go. If these quantifiers were lazy quantifiers, they would show up as +? or on the other hand {}?, this will guide the system to make the shortest match.


## Author

This is Manpreet Singh, I created this gist to show an use case of Regex to help understand Regex better for individual like me. Please checkout my github page at https://github.com/mani29jan
