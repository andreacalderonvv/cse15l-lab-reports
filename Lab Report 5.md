# Lab Report 5
---

## Student EdStem Post:
---
**What enviroment are you using (computer, operating system, web browser, terminal/editir, and so on)?**

I am on windows on Visual Studio Code using terminal commands.


**Detail the sympton you're seeing. Be specific; include both what you're seeing and what you expect to see instead. Screenshots are great, copy pasted terminal output is also great. Avoid saying 
"it doesn't work".**

The symptom I am seeing is that the terminal gives me an error that says:

error: file not found: TestBug.java
Usage: javac <options> <source files>
use --help for a list of possible options

I expected this to compile so then I can actually run the tests. This is an image of the error.

  
pic here
  

**Detail the failure-inducing input and context. that might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran.
 Do your best to provide as much context as you can.**

The current command I am running that produces this error is:

```
javac -cp ".;..\libs\junit-4.13.2.jar;..\libs\hamcrest-2.2.jar" TestBug.java
```

I ran that command so that I can compile the test cases on TestBug.java, I also checked that the file exists. I am not sure what else to do. Can I get some guidance?

## TA Response
---

Hello, since you have confirmed that the file exists, why don't you try checking if you are in the same directory as the file you want to compile? Try an ls or pwd command to check your location. cd if needed. :)

## What the Student Got:

pic here

The bug was that the the student was not in the proper directory. Though the file existed, it did not exist in the directory the student was in.

## Reflection
---

In the second quarter I really enjoyed running bash scripts and learning the syntax of it. It made me feel grateful about coding in java compared to bash. I do find the bash scripts useful and convenient. Before this class I never knew they existed.
