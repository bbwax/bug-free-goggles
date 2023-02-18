# A Regex Tutorial: Matching an Email Address
In this tutorial, we will be discussing how to match an email address using regular expressions. The email address we will be matching is represented by the following regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


## Summary

This regular expression matches an email address in the format of 'username@domain.com', where the username can contain letters, digits, underscores, dots, and hyphens, and the domain can contain letters, digits, dots, and hyphens, followed by a period and a top-level domain (TLD) consisting of two to six letters.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

Anchors are used to match the position of the regex within the text. In this email regex, the '^' and '$' anchors are used to match the start and end of the string, respectively. This ensures that the regex matches the entire email address and not just a portion of it.

### Quantifiers

Quantifiers are used to specify how many times a character or group should be matched. In this email regex, the '+' quantifier is used to indicate that the username and domain can contain one or more characters.

### Character Classes

Character classes are used to match a set of characters. In this email regex, the character classes '[a-z0-9_\.-]', '[\da-z\.-]', and '[a-z\.]' are used to match the characters in the username, domain, and TLD, respectively.


### Grouping and Capturing

Grouping and capturing are used to create subpatterns within the regex and extract specific portions of the matched text. In this email regex, there are three groups:

1. '([a-z0-9_\.-]+) ': captures the username
2. '([\da-z\.-]+)' : captures the domain
3. '([a-z\.]{2,6})' : captures the TLD

### Greedy and Lazy Match

Greedy and lazy match are used to specify whether the regex should match the longest or shortest possible string. In this email regex, the '+' quantifiers are greedy and will match the longest possible string.


## Author
BBwax github profile link: https://github.com/bbwax/bug-free-goggles
