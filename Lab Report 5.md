# Lab Report 5
## Part 1: Debugging Scenario
**Original Post:** <br />
**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?** <br />
I'm using a MacBook and writing the code using VScode.<br />
**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.** <br />
I'm done with writing the grader script, but the score part always shows 1/1 even though I have many tests in the TestListExamples.java. I tried to add and delete the test, but it still shows "score: 1/1". The score should change along with the number of tests in the TestListExamples.java. I feel like the problem is the redirection of the output or the counting of the tests.
![Image](beforefix.png)
![Image](manytests.png)
**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**<br />
The command I used is: "bash grade1.sh [Link](https://github.com/ucsd-cse15l-f22/list-methods-corrected)", the url is the repository containing my ListExamples.java. The script grade1.sh is the grader script provided by professor.<br />
**Response From TA:**
In this grader script, we use "grep" to extract the failure information and use the slicing of string to find the number of tests run and number of failures. In the original script, the slicing length is one, which is appropriate when you have single-digit number of tests. Thus, if you use more digit number of tests, the slicing length should change, too.

**Finding the Bug**<br />
I checked the failure counting part of the script, and realized that the script first finds the result line of JUnit, and then extract the number of tests and failures from that line. The slicing length was 1, but the result line of my tests was:
![Image](resultline.png)
So script only extracts the "1" of "12", showing the score as 1/1. The original script looks like:
![Image](before.png)
To fix the bug, I need to change the length of slicing so if can get the number of tests and failures correctly.
