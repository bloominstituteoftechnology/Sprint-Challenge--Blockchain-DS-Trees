# Sprint Challenge: Data Structures

In this sprint, you've been introduced into the fascinating and complicated world of blockchain.  You've also learned about a new type of data structure, trees, and how to traverse them.  

This Sprint Challenge will asses you understanding of blockchain by giving you the chance to compete with your fellow students to mine coins using a new Proof of Work Algorithm.

You'll also use your new-found knowledge of trees to optimize a working, but slow solution to a problem.  

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your Challenge score is a measure of your ability to work independently using the material covered throughout this sprint. You need to demonstrate proficiency in the concepts and objectives that were introduced and that you practiced in the preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your TL and Instructor in your cohort help channel on Slack. Your submitted work reflects your proficiency in the concepts and topics that were covered this week.

You have three hours to complete this Sprint Challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and it also helps your project manager to more thoroughly assess your work.

### Minimum Viable Product

#### [Blockchain](https://github.com/LambdaSchool/Sprint-Challenge--Hash-BC/tree/master/blockchain)

## Interview Questions

During your challenge, you will be pulled aside by a PM for a 5 minute interview. During this interview, you will be asked to discuss the following:

* Explain how a blockchain is structured.  What are the blocks, what are the chain?  How is the data organized?
* Explain how proof of work functions.  How does it operate.  How does this protect the chain from attack.  What kind of attack is possible?
* Explain how a breadth first -AND- a depth first traversal works on a tree.  Use the annotation tools in zoom to whiteboard each traversal on the tree below:

![Image of a Heap in Tree form](https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Max-Heap.svg/501px-Max-Heap.svg.png)

#### Runtime Optimization

***!Important!*** If you are running this using PowerShell by clicking on the green play button, you will get an error that `names1.txt` is not found.  To resolve this, run it, get the error, then `cd` into the `names` directory in the `python` terminal that opens in VSCode.

Navigate into the `names` directory. Here you will find two text files containing 10,000 names each, along with a program `names.py` that compares the two files and prints out duplicate name entries. Try running the code with `python3 names.py`. Be patient because it might take a while: approximately six seconds on my laptop. What is the runtime complexity of this code?

Six seconds is an eternity so you've been tasked with speeding up the code. Can you get the runtime to under a second? Under one hundredth of a second?

*You may not use the built in Python list or set for this problem*

(Hint: You might try importing a data structure you built during the week)


### Rubric

| OBJECTIVE                                                                                                                                      | TASK                 | 1 \- DOES NOT MEET Expectations                                                                                              | 2 \- MEETS Expectations                                                                                                                                        | 3 \- EXCEEDS Expectations                                                                                                                                        | SCORE |
|------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
| \_Student should be able to construct a binary search tree class that can perform basic operations with O\(log n\) runtime\.\_                 | Runtime Optimization | Student does NOT correctly identify the runtime of the starter code in name\.py and optimize it to run in under 6 seconds    | Student correctly identifies the runtime of the starter code in name\.py and optimizes it to run in under 6 seconds, with a solution of O\(n log n\) or better | Student does BOTH correctly identify the runtime of the starter code in name\.py and optimizes it to run in under 6 seconds, with a solution of O\(n\) or better |
| \_Student should be able to complete a Depth First Traversal and a Breadth First Traversal of a tree\.\_                                       | Interview Question   | The student fully explains two or fewer of the bulleted items in the solution repo\. | The student fully explains at least 3 of the items in the bulleted list\.                                | The student fully explains 4 or more items from the bulleted list\.           |
| \_Student should be able to diagram and code a simple blockchain, utilizing a cryptographic hash\_                                             | Interview Question   | The student fully explains two or fewer of the bulleted items in the solution repo\. | The student fully explains at least 3 of the items in the bulleted list\.                                | The student fully explains 4 or more items from the bulleted list\.           |
| \_Student should be able to utilize a Proof of Work process to protect a blockchain from attack\_                                              | Blockchain Problem   | The student is unable to mine a coin before the end of lunch\.                                                               | The student was able to mine a coin before the end of lunch\.                                                                                                  | The student presented a unique solution that was able to mine more than 100 coins before the end of lunch\.                                                      |
| \_Student should be able to build a protocol to allow nodes in a blockchain network to communicate to share blocks and determine consensus\.\_ | Interview Question   | The student fully explains two or fewer of the bulleted items in the solution repo\. | The student fully explains at least 3 of the items in the bulleted list\.                                | The student fully explains 4 or more items from the bulleted list\.           |


#### Passing the Sprint
Score ranges for a 1, 2, and 3 are shown in the rubric above. For a student to have _passed_ a sprint challenge, they need to earn an **average of at least 2** for all items on the rubric.
