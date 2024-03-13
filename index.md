# Lab Report 5 - Putting it All Together (Week 9)
## Part 1 – Debugging Scenario
## Original Post: 
Hello, 
I’m experiencing an issue when trying to reverse an array of integers in Java. 
My method reverseInPlace is supposed to reverse the array in place, but the output isn’t what I expected. Initially, I thought my loop or swap logic might be the issue, but I'm not sure what's wrong.
Here's the part of the code that's giving me trouble:
* Error code

![Images](errorcode.png)
* Error of output

![Images](erroroutput.png)

I expected to see `[4, 3, 2, 1]`, but that's not what's happening. Any thoughts on what might be causing this and how I can fix it?
## Response from TA:
Hi,

The logic in your reverseInPlace method seems to have a common mistake. 
You are trying to swap the elements within the same loop, which is causing the first half of the array to overwrite the second half.
To better understand what's happening during each iteration, can you add print statements after the assignment inside your loop? 
This will show us the state of the array at each step and help us pinpoint the error.

## Follow UP:
Thanks to your advice, I added print statements and discovered the problem! The array was being modified during the iteration,
which led to incorrect results. I have revised the method as follows:
* New method:

![Images](correctcode.png)

* New output:

![Images](correctoutput.png)

Now, when I run the program with the same input array, it correctly outputs the reversed array `[4, 3, 2, 1]`. Thanks again for your help!

## File and Directory Structure: 
