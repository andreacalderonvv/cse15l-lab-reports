# Lab Report 5
---

## Student EdStem Post:
---
**What enviroment are you using (computer, operating system, web browser, terminal/editir, and so on)?**

I am on windows on Visual Studio Code using terminal commands.


**Detail the sympton you're seeing. Be specific; include both what you're seeing and what you expect to see instead. Screenshots are great, copy pasted terminal output is also great. Avoid saying 
"it doesn't work".**

The symptom I am seeing is that my bash file keeps going to the else and prints:

File not found.

I expected this file to be able to compile and then run the tests. This is an image of the wrong output.

  
![Image](buggy)
  

**Detail the failure-inducing input and context. that might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran.
 Do your best to provide as much context as you can.**

The current command I am running that produces this error is:

`bash grade.sh`

I ran that command so that I can run the bash file so the test cases on TestBug.java compile, I also checked that the file exists. I am not sure what else to do. Can I get some guidance?

## TA Response
---

Hello, since you have confirmed that the file exists, why don't you try checking if you are in the same directory as the file you want to compile? Try an `ls` or `pwd` command to check your location. Add a command to change directories in your bash file if needed. :)

## What the Student Got:

![Image](goodOutput)

The bug was that the student was not in the proper directory when trying to compile through the bash file. Though the file existed, it did not exist in the directory the bash file was trying to compile in.

## Reflection
---

In the second quarter I really enjoyed running bash scripts and learning the syntax of it. It made me feel grateful about coding in java compared to bash. I do find the bash scripts useful and convenient. Before this class I never knew they existed. I will definitely be implementing these in my future projects.
