# RegEx Tutorial (Matching an email) 

Within this is a tutorial on how to use regex to match an email using the email regex: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. Fundamentally RegEx is useful for validating matching a hex value, matching a url, an html tag, and in this case an Email. I.E. should you have a form on your website in your app that gives a user a prompt to input an email address, it'd be wise to want to use this regex to validate it before it's sent to the app. Validating the email reduces the number of undeliverable emails sent back to the client. 

## Summary

"A regex, which is short for regeular, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string , or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. (README.md) " The tutorial below eases you through the components of a regex and how it's applied to match an email & the hex value. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
The Anchors of the expression begin with "^" which starts the string and the "$" is what ends the string. 
### Quantifiers
The quantifier "+" connects the user's email name + email service + .com. {2,6} is also a quantifier which allows a match range of 2-6 characters for this set: [a-z]
### Grouping Constructs
Capturing group 1: [a-z0-9_.-] -- matches the user's email name
Capturing group 2: ([\da-z.-]+) -- matches the email service
Capturing group 3: ([a-z.]{2,6}) -- captures the .com
### Bracket Expressions
[a-z0-9_.-] -- matching any letter a-z is case sensitive. It also matches a character 0-9 and matches the characters "_", "-", and "."
[\da-z.-] -- matching a single digit from 0-9, any character a-z (case sensitive), and the characters "." and "-".
[a-z.] -- matching any character a-z (case sensitive) and the character "."
### Character Classes
[\da-z.-] -- matching a single digit from 0-9, any character a-z (case sensitive), and the characters "." and "-".

## Author

Contact Info: GitHub: migueldavilajr Email: migueldavilajr@gmail.com
