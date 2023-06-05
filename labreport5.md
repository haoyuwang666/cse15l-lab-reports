# Lab Report 5-Putting it All Together

# Part1: Debugging Scenario
## Original Post of a Debugging question
**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

Macbook,VScode.

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

I am running tests of my ListExample.java merge method on ListExampletests.java . But there was one failure appeared on the terminal about Timeout Exception. 
Here is a screenshot of the output:

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

I am testing my merge method implemented in ListExample.java which is supposed to merge two sorted arraylist into one and with an sorted ascending order. I use command "bash test.sh" to run the shell file.
The contents of my shell file is here:

The test output showed an exception instead of an incorrect result, so I think there might be something wrong about my code but I cannot find it.
Here is my code of ListExample.java and my tests ListExampleTests.java:

## Response from a TA(mimicking by myself)
*Haoyu Wang: Try changing the index1+=1 in your last while loop to index2+=1.*

## Output after fixing bugs according to TA's suggestion
**Screenshot of output after fixing the bug:**

**Description of the bug:** The third while loop in the original code is trying to add the rest of the remaining elements in list2 into the result arraylist. However, this while loop checks whether index2 is smaller than the size of the arraylist. The original code has a line `index+=1;`, this line is incrementing index1 every time the condition is satisfied. So the while loop runs infinitely since index2 stays the same all the time. Instead of incrementing index1, it should increment index2 by `index2+=1;` so that the code will have correct behaviors.

