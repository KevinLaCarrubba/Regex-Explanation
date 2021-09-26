# Matching an Email: Regex Explanation Tutorial

Hey readers ! This is a break down explanation of the regex (`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`) used to match emails. This is a useful tool used for validating emails.

## Summary

I will go over what the `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is used for as well as the anchors, quantifiers, character classes, grouping and bracket expressions.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

The anchors used in this regex are `^` and `$`. The `^` marks the beginning of the regex and the `$` marks the end

### Quantifiers

The first quantifier we will be going over is the `+`. The `+` connects the email name to the email service provider and .com.

The second quantifier we will be going over is `{2,6}`. The `{2,6}` declares a match between 2 and 6 characters of the preceding token which in this case is character set `[a-z\.]`

### Grouping Constructs

In this regex the capturing group `([a-z0-9_\.-]+)` is used to match to the users email name.
The capturing group `([a-z0-9_\.-]+)` is used to match to the users email service provider.
The capturing group `([a-z\.]{2,6})` is used to match to .com

### Bracket Expressions

This regex uses 3 bracket expressions. The first of which is `[a-z0-9_\.-]`. This matches characters from a-z, 0-9, " _ ", " . " and " - ". The second is `[a-z0-9_\.-]`, which is matching chacters from a-z, a single digit from 0-9, " _ " and " . ". The third bracet expression is `[a-z\.]` which is matching characters from a-z as well as " . ".

### Character Classes

This regex includes the character class `\d`. This is used to match a single character digit from 0-9.

## Author

My name is Kevin LaCarrubba. I am currently attending Rutgers Coding Bootcamp in hopes of becoming a full stack developer. Check out my github [@KevinLaCarrubba](https://github.com/KevinLaCarrubba?tab=repositories)
