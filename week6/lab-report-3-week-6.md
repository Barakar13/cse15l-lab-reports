# Week 6 Lab Report - Group Choices in Lab 5

## Streamlining ssh Configuration
### Creation and edition of `.ssh/config`
Creation by Git Bash Here:
![creation](configCreation.png)
Edition by Git Bash Here:
![edition](configCreation2.png)
### login my account using `ssh ieng6`
![login](loginResult.png)
### copy a local file into my account using `scp`
I copy the file example.java into my account
![copy](scpResult.png)

## Setup Github Access from ieng6
### Public Key in Github
![publicKey](publicKey.png)
### Public Key and Private Key in User Account
![keys](privateKey.png)
### push a change and running process
I create an example.txt file and push this file to the Github from my account.
![runningProcess](pushResult.png)
![runningProcess2](pushResult2.png)
push new changes without passwords:
![newChanges](pushAutomatically.PNG)
### link to this commit
[example.txt](https://github.com/Barakar13/markdown-parser/commit/6824cd4549234314adda8ec2e4390ad9e525b657)
or
"https://github.com/Barakar13/markdown-parser/commit/6824cd4549234314adda8ec2e4390ad9e525b657"

new commit link: [newCommit](https://github.com/Barakar13/markdown-parser/commit/12746078da8b3ab47a20a943f122bda1042f9d53) or "https://github.com/Barakar13/markdown-parser/commit/12746078da8b3ab47a20a943f122bda1042f9d53"

## Copy whole directories with `scp -r`
### Copy a whole directory to my ieng6 account
![copyResult](copyDirectory.png)
### login my ieng6 account and run tests in the copied directory
![runTest](runTest.png)
### combining `scp`, `;`, and `ssh` to copy the whole directory and run tests
![combination](oneLine1.png)
![combination2](oneLine2.png)

