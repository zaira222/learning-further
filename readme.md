# Learning Further with Emails 

In this gist I will be focusing on matching an email regex and how it works 
as well as break it down further. Which will help better understand regex as a whole. 

## Summary 

To be able to have user input option to type an email address we would have to have something to  
verify the email address. That is where the matching email regex comes in where verifies what the  
user has provided with the regex which in turn will either verify or reject it.  
For example, in this code snippet `/^([a-z0-9_\.-]+)` the anchor is telling the regex as a whole where  
it starts more specifically in the front of the regex. Depending which character the user inputs. 

* Matching an Email – `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`  

## Table of Contents 

- [Anchors](#anchors) 
- [Quantifiers](#quantifiers) 
- [Character Classes](#character-classes) 
- [Flags](#flags) 
- [Grouping and Capturing](#grouping-and-capturing) 
- [Bracket Expressions](#bracket-expressions) 
- [Greedy and Lazy Match](#greedy-and-lazy-match) 
- [Look-ahead and Look-behind](#look-ahead-and-look-behind) 

 
## Regex Components 

* Matching an Email – `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`  

### Anchors 

Carat `^` is specific to the beginning of the regex. Which would capture the code snippet below depending on the user input. For example, if the user typed code9@yahoo.com then it would start with the letter c. Which is the first letter of the user input.  

Anchor appears in both of these code snippets below. 

`/^([a-z0-9_\.-]+)` 

`@([\da-z\.-]+)` 


### Quantifiers 

In this regex it has three quantifiers `+` which are shown below in the code snippets. Which it would have to match the string 
that was in the regex. 
For example, it would have to match any of specifications that the regex applies like a character a-z or  
number 0-9. With the email code9@yahoo.com it does match the previous characters before the quantifier. 

Quantifiers appear in these code snippets below. 

`([a-z0-9_\.-]+)` 

`([\da-z\.-]+)` 

`{2,6}` 

 
### Character Classes 
Regarding character classes they are considered to be surrounded by []. But, inside of them is what characters we require for the regex to verify the email. 
For example, with the email we have been using it matches the characters because it gives us a range from a-z or 0-9. And the email code9 fits in to the requirements stated above. 

`([a-z0-9_\.-]+)@` 


### Flags 

The flags which deals with the slash `(/)` which in turn when the regex expression comes to an end it is where the flag will appear. Depending on which one was choosen. 


`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`  


### Grouping and Capturing 

With grouping and capturing we will take a look at the first code snippet from below with our email  
code9@yahoo.com. Which the code snippet captures all the characters within the paranthesis with all those  
requirements it would end up being code9 would reference the first code snippet. 

`([a-z0-9_\.-]+)` 

`([\da-z\.-]+)` 

`([a-z\.]{2,6})`  

 
 

### Bracket Expressions 

We will take a look at the first code snippet code below with the bracket expression which it focuses on the string. With the string it is trying to make sure that with the following requirements a-z or 0-9 the user input code9 has matched. With all the letters and numbers used fit the requirement. 


`[a-z0-9_\.-]` 

`[\da-z\.-]` 

`[a-z\.]`  

 
 

### Greedy and Lazy Match 

With this topic it actually goes with quantifiers. The plus sign as well as the curly brackets are considered greedy and lazy match. Once the bracket expressions has been plugged in and the plus sign has matched. 

`([a-z0-9_\.-]+)` 

`([\da-z\.-]+)` 

`{2,6}`  

 
 
 

## Author 

My name is Zaira and  I am currently in a Coding Bootcamp offered by Michigan State. If you have any questions I have provided my github link below. Feel free to reach out to me with any questions or concerns. 

<a class href="https://github.com/zaira222"></a> 

 
 

 