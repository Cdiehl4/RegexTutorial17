# Regex Tutorial: Matching a URL
The purpose of this tutorial is to explain what a regular expression or Regex is and how it is broken down to describe certain functions or other examples.

## Summary

 Regex is short for regular expression which is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string. A breakdown of Regex: Matching a URL is below: /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

## Table of Contents

- [Regex Components]
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components
Each component of this regex has a unique responsibility to make sure that a user enters an email address that begins with an unspecified number of characters preceding the @ symbol, followed by a domain. The elements of this expressions are presented below.

### Anchors
The two principal anchors in this regex expression are the ^ at the beginning and the $ at the end which constitute an exact string match with the components included within the two anchors. The ^ anchor matches any string that begins with the characters that follow the anchor. The $ matches any string that ends with the characters that precede it.

### Quantifiers
Some of the components of capture groups end with a ? or a *, these are the quantifiers. The ? makes a single instance of the character preceding the quantifier optional, whereas the * makes multiple instances of the characters preceding the quantifier optional. Quantifiers are used to define the number of times a given expression may be identified.

### Grouping and Capturing
There are a number of components separated by parentheses (). Parentheses are used in regex to create separate groups of interest. Within each of the groups, there is a regex that we may look at separately to see what is evaluated. This includes:

the initial https component: (https?:\/\/)
the domain name (e.g. www.google, or pets): ([\da-z\.-]+)\.
the top level domain (.com, .gov, etc): ([a-z\.]{2,6})
the file path: ([\/\w \.-]*)* 

### Bracket Expressions
The main OR operator used in the above regex is the []. The expression will match for any characters or character classes included in the brackets.

### Character Classes
The main character classes to consider in the above expression include the \d character class which looks for any digit, and the \w character class that looks for any numerical character.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile) Hi, my name is Christian Diehl. I am a Fullstack Flex Bootcamp Student, I want to continue working on coding and gain experience in the Tech Industry. Here's a link to my Github to see some of my projects. https://github.com/Cdiehl4
