# TutorialEx
Regex expression are useful tool that offer an efficient way to process large blocks of text within code. It follows a pattern of using a regex to find a specific pattern within a larger string. Finding a pattern is a very common task and regex is a very powerful tool that can be used to accomplish this task.




## Summary
Put simply regex stands for regular expression. This is a sequence of characters defining a certain search pattern that can help match or locate text. This allows for easier management and is often used for validation purposes. Regex can also be utilized to find patterns of characters withing strings. Below is a list of regex components that will be defined for the purpose of understanding it's purpose. I'll be utilizing parts of this expression to help explain the process further /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-f\.]{2,6})$/



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

Anchors are in the family of regex tokens and don't match any characters. Their purpose is to assert a specific detail about the matching process. The below are regex anchors:
- ^ Start of string
- $ End of string


### Quantifiers

A quantifier uses regex to match sequences of text. Some examples could be characters, groups, or character classes. These text quantifiers must be present in the input sting for a match to be generated through the quantifier. An example would include { n } which matches the previous element exactly n amount of times. Another example would be * which matches the prior element 0 or more times. One additional example would be +? that matches the previous element 1 or more times and as few times as it possibly can.
 

### OR Operator
These are usually used to match characters and expressions on on or both sides of the OR operator, labeled as |. The or operator tells regex engine to use whatever expression on either side of the operator it wants. Both results will be produced as the desired outcome.
 

### Character Classes
Character classes are basically used to match one specific character within a set of additional characters. This generally means that they will help shorten a search for characters by utilizing keywords. \w matches any word character, \W matches any non-word character, \s & \S matches any white-space or non-white-space character and \d matches any decimal digit. You can use these to create character ranges some examples would be [a-z] or [0-9]. One last example would be [^a-z] which would match any character that is not a lowercase letter and characters would be case-sensitive in this group.


### Flags
There are 6 flags in regex, two of which are most important. One of them being g which is a global search that does not return after the first match and i which is a case-insensitive search. Flags can also be put together or combined within a single regex and are denoted at the end of a pattern. 


### Grouping and Capturing
Grouping, Capturing Grouping, and Capturing is used most while identifying one or multiple subexpressions. These can also be used to capture substrings of an input. They also match a subexpression repeated withing an input string. However, they retrieve individual subexpressions and process them separately from the text that is being matched. A common example of grouping and capturing is from validating an email input. For example /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. After breaking this down it reveals ^ is used to identify the start of the regex email address, .-@ characters are used to find literal characters, and the {2,7} is the range of character length needed.


### Bracket Expressions
These expressions utilize brackets [ ] to find lists of characters. By using a - inside the brackets it will create a range like 0-8 or whatever your desired range is. The main purpose of the expressions are to help developers identify the specific hex code that is generally associated with css color codes. A common example would be [0-9a-f] which would match any hexadecimal number. In this example the brackets are being used to show the finding of ranges 0-9 and a-f.


### Greedy and Lazy Match
Greedy and Lazy match are two different ways quantifiers can be utilized. Greedy match will match the longest possible string and is the default. Lazy match will match the shortest possible string. This can be helpful depending on if you are looking to find a long or short string. The Greedy match will look for the longest number of characters that follow < and the lazy search will utilize a ? and look for the shortest possible string.


### Boundaries
These are quite similar to anchors in that they are used to assert a specific detail about the matching process. For example = is used to assert that the character before it is the same as the character after it. The ^ is used to assert that the character before it is the start of the string and the $ is used to assert that the character after it is the end of the string.


### Back-references
These allow a prior matched subexpression to be used in the current regex. This is useful when you want to use a previously matched subexpression in a new regex. For example, the regex /(a)(b)(c)/ would match the string abc. If you wanted to match the string abcbc you would need to use the back reference to match the second b. This can be done by using the regex /(a)(b)(c)/ and the back reference /(b)(c)/.


### Look-ahead and Look-behind
These are used to assert a specific detail within the matching process. look-ahead is used to find that the next character is the same as the character after it. look-behind is used to find that the previous character is the same as the character before it. For example, the regex look-ahead example /(?=a)/ would match the character a if it is the first character in the string. The regex look-behind example /(?<=a)/ would match the character a if it is the last character in the string.


> Github: [David Ramm](https://github.com/Dramm1)

> E-mail: [davidkramm53@gmail.com](mailto:David)