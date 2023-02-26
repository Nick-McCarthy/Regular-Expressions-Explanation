# Email Regular Expression Explanation
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
## Summary
The Regex listed above can be used to validate email addresses. Below you will find basic concepts of regular expressions outlined using the above regex string as an example.
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
Anchors are regex tokens that don't match any characters but that say or assert something about the string or the matching process. The '^' and '$' symbols are anchors, the '^' symbol represents the start of the string, and the '$' symbol represents the end of the string.
'^': start of string
'$': end of string

### Quantifiers
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. The '+' symbol is found within the regex, and it indicates that the regex should match to the preceding pattern one or more times.
<br>
'[\da-z\.-]+': match one or more digits, lowercase letters, dots, or hyphens.

### OR Operator
The "or" operator is represented by the '|', It allows you to specify multiple alternative patterns that can match a given text. There is no or operator within the above regex.

### Character Classes
A character class is a special notation that represents a set of characters. It allows you to match any one of the characters in the set.
<br>
'[a-z0-9_\.-]': any lowercase letter, digit, underscore, dot, or hyphen.
<br>
'[\da-z\.-]': any digit, lowercase letter, dot, or hyphen.
<br>
'[a-z\.]': any lowercase letter or dot.


### Flags
A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way.
There are no flags in the regex listed above.

### Grouping and Capturing
Grouping allows you to group parts of the pattern together. Capturing happens when you save the matched text inside a group for later use.
<br>
'([a-z0-9_\.-]+)': matches one or more lowercase letters, digits, underscores, dots, or hyphens and captures the result in a group.

### Bracket Expressions
Bracket expressions are indicated by square brackets '[]' and can contain a list of characters, ranges of characters, or character classes.
<br>
'[a-z0-9_\.-]': any lowercase letter, digit, underscore, dot, or hyphen.
<br>
'[\da-z\.-]': any digit, lowercase letter, dot, or hyphen.
<br>
'[a-z\.]': any lowercase letter or dot.

### Greedy and Lazy Match
A (greedy match) means match the longest possible string, while a (Lazy match) means match the shortest possible string. For example, the greedy h.+l matches 'hell' in 'hello' but the lazy h.+?l matches 'hel'. the '+' and '*' symbols are greedy by default, meaning they will match as much as possible while still allowing the overall pattern to match. The matches found within the above regular expression are greedy.

### Boundaries
A boundary is a special character or sequence of characters that represents a limit between different parts of a string. A boundary can help you define where a pattern should start or end within a string. The '^' and '$' symbols are technically boundaries (line boundaries).

### Back-references
Back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are specified with backslash and a single digit (e.g. ' \1 '). 

### Look-ahead and Look-behind
Lookahead allows you to add a condition for 'what follows'. Lookbehind allows you to match a pattern only if there’s something before it. There are no look-aheads or look-behinds in the above regex. 

## Author
Nick McCarthy
GitHub Account:
<br>
https://github.com/Nick-McCarthy
