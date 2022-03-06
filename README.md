# regex-tutorial

Regex Tutorial -- Introuducing Hex 

The hexadecimal is a positional numeral system that uses 16 distinct symbols. The symbols are "0"-"9" to represent values 0 to 9 and "A"-"F", or "a"-"f", to represent values 10 to 15. The code that is going to be broke down is /^#?([a-f0-9]{6}|[a-f0-9]{3})$/.



Summary

We are going to be breaking down the hexadecimal system. The hex system, also know as a regular expression, can be used to define a set of characters and return a unique value. One of the most valuable assets of the hex is using for differnt color palettes in our CSS styling. The combination of letter and numbers create differnt color schemes. 

Table of Contents
Anchors
Quantifiers
The OR Operator
Character Classes
Bracket Expressions
Greedy and Lazy
Author


[Anchors]

The expression we are evaluating is 
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

We start with the anchors which are the "^, $."
First the "^" expression represents the begining of a string or a line, while the "$" represents the end of a string. With these characters, we are ensuring that our code with start from begining and go all the way to the end. 

[Quantifers] 


The most common quantifyer we see in this expression is the  curly brackets. The quantifiers search for a match in the previous section of 6 and/or 3 characters. Hex codes as previously mentioned are most commonly used when searching for colors in CSS. Here we are seeing that we are searching for a combination of 6, but can also be shortened to the 3, like an abbreivation. In our expression we also see the "?" This quantifer matches any following characters 0-1 times, also used as a sorting tool.


[The-OR-Operator] 

Here in our expression we are shown "|" Here we are esentially allowing this expression to be broken down into 2. We can break it down into  [a-f0-9]{6} and [a-f0-9]{3}. Our regex will match any of those two expresions. 

[Character-Classes] 

The brackets highlighted here represent the character classes. These represent the range of characters that are to be matched, which is in this case a letter between a and f, and a number between 0 and 9.

[Bracket-Expressions]

The parenthesis are used as the bracket expressions. Brackets are the code we are trying to match after the anchors. Since the individual 6-character and 3-character sets use brackets, parentheses are used to group the section of the expression we are tying to match.


[Greedy-and-Lazy]

Greedy and lazy estentially describe when the expression is considered to be matched. Greedy matches will match all of the possible answers, while lazy matching will stop after finding the first match. In this expression, we are looking for a code that starts with the # character, and then the ? character signifies a lazy match, which will return one set of the following characters.

[Author]

 The author is Bianca Tijerino. In the mist of becoming a full stack web developer!
 https://github.com/btijerino16