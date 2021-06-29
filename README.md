# Regex Explanation

This is simple explanation that gives a brief scenario of how email validation works with regular expression.This is simple explanation that gives a brief scenario of how email validation works with regular expression.


## What is regex?

To sum it up, regex also known as regular expressions are patterns used in a expression, in this case it is javascript, to
find a specific combination in a sentence or paragraph. A regex always will start
with literal that contains a / and ends with /. Like example below. 👇 
```bash
  let regex = /ab+c/;
```

## How does regex work?

What makes regex the way it is because of how certain special character actually 
performs a specific search. For example if you were to use

```bash
  let regex = / \d /
```

it would search the numbers in a given string. So in A1, the returned 
result would be 1. Now there are a lot of special characters used in regex but 
we are going to focus on the ones used in email validation. 

## How does email validation work?

The way email validation for regex works is that it doesn't detect if
the email is a valid one but to make sure that the correct syntax was 
entered that makes it an email. The most basic email validating structure is

```bash
  function validateEmail (email) {
    return /^\S+@\S+\.\S+$/.test(email);
  }
```

The function above basically tells the computer that we are looking for a 
structure like 👇 

```bash
  _@_._
```
If you were to type a regular email for example test@.com, then 
validation would be true. 

Lets break it down even further and see what exactly each special character is saying.

The expression begins with ^ which means that this is our beginning input. 
Next we see that our expression contains a [ ... ] which finds any character 
inside the bracket. Inside the bracket we have another ^ with \S. 

\S will
look for everything thats not under a white space. The + means that they must match everything
before as much as possible. (refers to greedy quantifiers). 

The special character . is more of a wildcard and will match for anything in that string. Finally
we have $ as our ending input. If you were to combine everything, it will do your 
basic email validation. Now this of course means that you would need to adjust the expression to 
match different scenarios with more special characters. Refer to this link for more info: 
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Cheatsheet

## TLDR..
If you really want a super basic explanation... 

Basically you have a string of code that looks for a string of text or number with / -input your special characters- /. 

## Authors

- [@NIASKA / Alan](https://github.com/NIASKAA)

  
## Feedback

If you have any feedback, please reach out to us at mkman751@yahoo.com

  
