# Lab Report 4

## Logging Into ieng6:

![Step 1](step1)

`<up> <enter>`

These commands go up into my terminal history and log into ieng6.
  
## Cloning the Fork of the Repository From the Github account:
  
![Step 2](step2)
  
`git <space> clone <ctrl+v> <enter>`

These commands clone the lab7 repository.

## Run the Tests, Demonstrating That They Fail:

![Step 3](step3)

`cd <space> lab7 <enter>`

`bash test.sh <enter>`

These commands change into the lab7 directory and run the test.sh tests.

## Edit the Code File to Fix the Failing Test:

![Step 4](step4)

vim ListExamples.java <enter>

`x i 2 <esc> :wq <enter>`

The first set of commands runs vim and then when vim opened up, my cursor was already on the 1 of the index1 so I pressed x to delete it. Then I pressed i to enter insert mode and esc after to exit out of it. :wq was to save and quit vim.

## Run the Tests, Demonstrating That They Now Succeed:

![Step 5](step5)

`<up> <up> <up> <enter>`

This set of commands goes into the terminal history of when I first ran the test and then runs it.

## Commit and Push the Resulting Change to Your Github Account:

pic here

`git add ListExamples.java`

`git commit -m "success"`

`git push`

The first command adds ListExamples into a list of files that will be committed. Then the next command actual commits the changes. The last command then pushes the changes onto the git hub account.


