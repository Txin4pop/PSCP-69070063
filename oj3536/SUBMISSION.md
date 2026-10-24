# Problem Solving Submission

This file must be written by the student in their own words.

Use this template only for OJ problems that are marked as learning-log required.

Do not ask AI to write this file for you. AI may help check grammar, formatting, or clarity after you have written your own content.

If AI was used for this learning-log-required problem, also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
3536
```

OJ submission ID, if submitted:

```text
695264
```

OJ status:

```text
Pass
```

Independent time spent on this problem:

```text
0-15 minutes
```

Choose one:

```text
0-15 minutes
15-30 minutes
30-60 minutes
1-3 hours
3-6 hours
6-24 hours
1-3 days
4-7 days
1-4 weeks
More than 4 weeks
```

How to count this time:

- Count only the time you actively worked on this problem independently.
- Start counting from when you first read the problem.
- Do not include breaks, meals, classes, sleep, time spent on other problems, or time when you were not working on this problem.
- If you used AI, count only the independent time before your first AI prompt.
- If you asked a friend, TA, or instructor for help, count only the independent time before your first help request.
- If you used both AI and human help, count only the independent time before the first outside help of any kind.
- If you did not use AI or human help, count the time before writing this `submission.md`.
- An estimate is acceptable, but it must be honest.

---

## 2. My Understanding

Write the problem in your own words.

Also explain the input, output, and important constraints.

If you do not fully understand the problem yet, write what you currently understand. Your understanding may be incomplete or incorrect, but you must make a genuine attempt.

```text
so the input will be 1 line with just 1 number n. i have to check if n is a prime number or not. a prime is a number that only has 2 numbers that can divide it evenly, which is 1 and itself. the output will be 1 line, print YES if n is prime and print NO if it is not.
the time limit is 1 second, so if i loop from 1 to n it will only pass 10/20 testcases (O(n)). to pass all 20/20 i need to make it O(n**0.5) and i didn't use import math so i use n ** 0.5 instead of sqrt
```

---

## 3. My First Plan

Write your first plan before getting help from AI, a friend, a TA, an instructor, or before finalizing your code.

If you used AI, write the plan you had before your first AI prompt.

If you asked a friend, TA, or instructor for help, write the plan you had before asking for help.

If you did not use AI or human help, write the plan you had before or while you started coding.

This can be rough. It may be incomplete or different from your final solution.

You may write pseudocode, a flowchart idea, or step-by-step thinking.

```text
Step 1: input the number then use int() to turn it into n
Step 2: check the easy cases first. if n < 2 print NO (1 is not a prime), if n == 2 print YES, if n is even (n % 2 == 0) print NO
Step 3: use a while loop with i starting at 3, loop till i > n ** 0.5 (+1 to be safe) and add 2 to i every loop because we already know even numbers can't divide it
Step 4: in every loop if n % i == 0 then n is not a prime so print NO and stop the loop
Step 5: if the loop ends and nothing divided n then print YES
```

---

## 4. My Final Approach

Briefly explain the final algorithm or method you actually used in your submitted code.

This section is different from Section 3:

- Section 3 is your first plan before AI, human help, or before the final code.
- Section 4 is the final method used in your actual solution.
- If your final approach is the same as your first plan, write that it is the same and briefly explain why.

Do not copy AI's explanation.

Do not copy another person's explanation.

```text
the same as my first plan because it work
```

---

## 5. My Tests

Write at least 3 test cases that you tried or designed by yourself.

Try to choose test cases that are different from each other.

For each test case, explain why you chose it.

If the input or output has many lines, write them inside the text blocks.

### Test Case 1

Why I chose this case:

```text
i chose this because 1 only has 1 divisor (itself) but a prime needs exactly 2
```

Input:

```text
1
```

Expected output:

```text
NO
```

Actual output:

```text
NO
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
i chose this because my code says “even number = NO”, but 2 is the exception
```

Input:

```text
2
```

Expected output:

```text
YES
```

Actual output:

```text
YES
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
i chose this because 49 = 7 x 7, so the only divisor is exactly at root n. if i loop to < root n instead of <= root n will miss 7 and print YES and wrong
```

Input:

```text
49
```

Expected output:

```text
NO
```

Actual output:

```text
NO
```

Result:

```text
Pass
```

---

## 6. AI Use

Did you use AI for this problem?

```text
No
```

If yes, also complete:

```text
ai_reflection.md
```

If you only asked a friend, TA, or instructor and did not use AI, you do not need to complete `ai_reflection.md`.

---

## 7. Human Help / Collaboration

Did you ask a friend, TA, instructor, or another person for help on this problem?

```text
No
```

If yes, briefly explain what kind of help you received.

Allowed examples:

- explanation of the problem statement
- explanation of a programming concept
- hint about the approach
- debugging discussion
- test-case discussion
- help understanding an error message

Not allowed:

- copying another person's code
- submitting another person's solution
- asking another person to write the solution for you
- using another person's OJ submission
- asking another person to submit to the OJ for you

Who helped you?

```text

```

What did they help with?

```text

```

What did you still do by yourself?

```text

```

Did you copy any code from another person?

```text
No
```

---

## 8. Student Declaration

Write `Yes` for each statement.

| Statement | Yes/No |
|---|---|
| I wrote this submission in my own words. | Yes|
| I understand my final code. | Yes|
| I recorded the real OJ status. | Yes|
| I did not copy AI-generated text directly into this file. | Yes|
| I did not copy code from another person. | Yes|
| If I received human help, I disclosed it in this file. | Yes|
| I submitted the final code to the OJ by myself. | Yes|
