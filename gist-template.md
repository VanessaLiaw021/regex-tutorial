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

First, we start with this section of regex, ([a-z0-9_\.-]+). This will match the email username. Next, we start with this section of regex, ([\da-z\.-]+). This will match the email service provider, such as gmail, yahoo, outlook, etc. 
Lastly, we look at ([a-z\.]{2,6}). This will match the top level domain, such as .com, .net., .gov, and etc. In the next section, I will explain the characters in the (), which are known as subexpression.

### Bracket Expressions

As we mention before, this section I will explain that is happening in the (). 

```
([a-z0-9_\.-]+) and ([\da-z\.-]+) and ([a-z\.]{2,6})
```

Let's take a look at the first expression in this regex, ([a-z0-9_\.-]+). As we can see, within the (), we see something call a bracket expression, []. The bracket indicates a set of characters that we're trying to match in the expression. Let's start with the a-z, this can include any characters between a-z in the email. Often, we will also see 0-9, which is similar to a-z, but instead it including any numbers between 0-9. Next, we see a dash (-) and hyphen (_), this mean that in the email address it can include hypen and dash. The   hypen and dash are consider special charcters. Special characters are consider non-alphanumeric charcters.

Now, let take a look at the next expression ([\da-z\.-]+). As we can see, there is another [] in this expression, where it is matching the email service provider, that can include alphabet from a-z. and can include a dash. In the next section, we will learn about the \d and \ .

Lastly, we take a look at ([a-z\.]{2,6}). There is another bracket inside of this expression, but we seen it all. It only will allow alphabet between a-z. Again, I will explain what the \ in the next section called Character Escapes. 

### Character Classes

Now, learning about character classes, which is the expression below, the \d. 

```
\d
```

In this tutorial it is seen in this expression ([\da-z\.-]+) where again it matching the email service provider. The meaning of \d is it matches any digit from 0-9, specifically arabic numeral.  

### Character Escapes



```
\
```

## Author

My name is Vanessa Liaw and I am learning regex while I am explaining through this regex tutorial. It help me understand each symbol one by one and other regex component and understanding how to create my own regex. If you find this interesting, take a look at my other projects and view my profile

[Github Repo](https://github.com/VanessaLiaw021)