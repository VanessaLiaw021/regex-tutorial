# Regex Tutorial - Matching a Email

Regular expression or regex for short, is a combination of a text string that enables the creation of patterns to match, find, and manage text. Regex can be used for alot of things, such as validating a user input for a form, like signing up or matching a certain requirement on a password, and so much more. For the most part, regex is commonly used more in validating a user input. Whether is email, name, phone number, username, they are can be validated with using regex. Once you understand the symbols and the patterns in regex, then it will be lot easier for you to create your own regex that matches your requirements.

## Summary

In this regex tutorial, I will be explaining how to use regular expression to match an email.
The example regex pattern I will be explaining will be

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 
```

This regex expression is one way to match a email, but there other many different ways a person can match an email in regex, but for this example, we will use the one that is listed above. In this tutorial, I will break down each part and each symbol of the regex above and describing what it does.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

In regex, the patterns need to always be enclosed with a slashed characters (/) since regex is considered a literal. As we can see in the regex below, we can see that it is enclosed with a slashed at the beginning and ending.

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 
```

In this tutorial, I will break down each component of regex by anchors, quantifiers, group constructs, bracket expression, character classes, the OR operator, flags, and character escaptes.

### Anchors

In regex, anchors are consider tokens that doesn't match any characters but it indicate something about the string or the matching method despite not matching any characters. Anchonrs let us know the current position in the string corresponds to a certain location, such as a beginning or ending of a string or line.

```
^ and $
```

To understand anchors a little better, the beginning symbol in regex is ^. The symbol ^ represent the beginning of a string. You must wonder if there is a beginning, there must be an ending symbol, which there is. The symbol that represent the ending of a string is $. 

### Quantifiers

In regex, quantifiers are define as the minimum number of occurrences of a character, group, or character class required to find a match in the input. There are others quantifiers, but the one we focusing on will be the symbol of

```
+ and {}
```

To understand quantifiers a little better, the + symbol is consider a greedy quantifier. It will allow repeats of the previous items one or more. But in this case, the + symbol which will connect the user email name + email service provider + .com after.

As for the quanitifer {2, 6}, it represent the certain range of the characters that user can have. The minimum character would be 2 and the maximum character would be 6. This quantifier is only for this snippet of regex, [a-z\.].

### Grouping Constructs

Group constructs are consider the regex in the (). They represent should be capture in the inputted string. Inside the (), you are allow to add like quantifiers inside the (). For example, as mention before, you can add the symbol + or add a range for your regex.   

```
([a-z0-9_\.-]+) and ([\da-z\.-]+) and ([a-z\.]{2,6})
```

First, we start with this section of regex, ([a-z0-9_\.-]+). This will match the email username. a-z allow letters from a-z. 0-9 allow numbers from 0-9. The _ and - allows underscore and hypen in your email username. 

Next, we start with this section of regex, ([\da-z\.-]+). This will match the email service provider, such as gmail, yahoo, outlook, etc. 

Lastly, we look at ([a-z\.]{2,6}). This will match the top level domain, such as .com, .net., .gov, and etc. As mention before, a-z will allow letters from a-z, but allow the range {2,6} from 2 to 6 characters long.

### Bracket Expressions

### Character Classes

### Character Escapes

## Author

My name is Vanessa Liaw and I am learning regex while I am explaining through this regex tutorial. It help me understand each symbol one by one and other regex component and understanding how to create my own regex. If you find this interesting, take a look at my other projects and view my profile

[Github Repo](https://github.com/VanessaLiaw021)