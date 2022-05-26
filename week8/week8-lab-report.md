# Week 8 Lab Report

## Two Repository Links
### my repository:
[myRespository](https://github.com/Barakar13/markdown-parser) or https://github.com/Barakar13/markdown-parser
### reviewed repository:
[reviewRepository](https://github.com/gabrielseventhucsd25/markdown-parser) or https://github.com/gabrielseventhucsd25/markdown-parser

## Snippet1 - `backtickTest13`
### Expected Output
![snippet1](snippet1.png)
Expected Link list:[`google.com, google.com, ucsd.edu]
### Code in `MarkdownParseTest.java`
![testCode1](testCode1.png)
### JUnit Output in My Code
![myCodeResult](myRunningResult1.png)
### JUnit Output in reviewed Code
![reviewedCodeResult](otherRunningResult1.png)

## Snippet2 - `bracketTest14`
### Expected Output
![snippet2](snippet2.png)
Expected Link list:[a.com, a.com(()), example.com]
### Code in `MarkdownParseTest.java`
![testCode2](testCode2.png)
### JUnit Output in My Code
![myCodeResult](myRunningResult2.png)
### JUnit Output in reviewed Code
![reviewedCodeResult](otherRunningResult2.png)

## Snippet3 - `longTextTest15`
### Expected Output
![snippet3](snippet3.png)
Expected Link list:[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]
### Code in `MarkdownParseTest.java`
![testCode3](testCode3.png)
### JUnit Output in My Code
![myCodeResult](myRunningResult3.png)
### JUnit Output in reviewed Code
![reviewedCodeResult](otherRunningResult3.png)

## Answer the following questions 
## Snippet 1
### Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks?
Yes， I have two small changes to make my program work in the snippet 1. Firstly, I should add a condition to determine whether the sign before [ is  `. If so, I should run a loop from [ to ] to check whether there is another sign among them. Secondly, when I search the first [], I should add a condition in a loop to find whether there is next ]( before the next[.

## Snippet 2
### Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets?
Yes, I should also make two changes. when I search the first [], I should add a condition in a loop to find whether there is next ]( before the next[.Secondly, when I check index of closeParen, I should add a loop to keep looking for the next ), which doesn't have （ before itself, and break the loop when I find the last reasonable (.

## Snippet 3
### Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses?
No, when there is space line among [], the link format won't work because string input doesn't check a space line. To fix it, we need to change the String input into a file name and run scan to check next line. If there is a space line, we should mark it and when we get link, if there is a space line between [], we will continue the while loop to look for the next []. Also, we also need to add a if condition to check whether the next ) doesn't ( before. If so, we should continue the while loop.
