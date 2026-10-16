# Problem Solving Submission

This file must be written by the student in their own words.

Use this template only for OJ problems that are marked as learning-log required.

Do not ask AI to write this file for you. AI may help check grammar, formatting, or clarity after you have written your own content.

If AI was used for this learning-log-required problem, also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
3484
```

OJ submission ID, if submitted:

```text
687902
```

OJ status:

```text
Pass
```

Independent time spent on this problem:

```text
15-30 minutes
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
so the first line of input have 2 things, N and P. N is the size of the floor (N*N tiles) and P is the fine for every 1 spot that sounds bad (P can be a decimal).
after that there are N lines, each line have N numbers. each number x (0 to 5) is how many spots on that tile that sounds bad (0 means the tile is perfect).

the output will be N+3 lines
- line 1 to N: print the same row back, then add 2 more numbers at the end of the row, 1st is how many tiles in that row that have x > 0, 2nd is the sum of x in that row
- line N+1: for each column, how many tiles that have x > 0
- line N+2: for each column, the sum of x
- line N+3: total tiles that have x > 0, total sum of x, and the total fine (total sum of x * P) with 2 decimal places
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
Step 1: input N and P in 1 line, split it, then make N = int(float(N)) and P = float(P)
Step 2: make 2 lists col_tiles and col_points that have N zeros, and total_tiles = 0, total_points = 0
Step 3: loop N times to input each row, split it and map it into int, then keep the row in a list called grid
Step 4: loop in every row, for each x in the row, if x > 0 then row_tiles + 1 and col_tiles[j] + 1, then add x to row_points and col_points[j]
Step 5: after finishing a row, print the row, then row_tiles and row_points, and add them into total_tiles and total_points
Step 6: after all rows, print col_tiles, then col_points
Step 7: print total_tiles, total_points and total_points * P with 2 decimal places
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
the same as my first plan
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
this is the main case, it have 0 and many different numbers in different rows and columns, so I can check that the row sum, column sum, and the total are all correct
```

Input:

```text
3 10
0 2 5
1 0 0
3 4 0
```

Expected output:

```text
0 2 5 2 7
1 0 0 1 1
3 4 0 2 7
2 2 1
4 6 5
5 15 150.00
```

Actual output:

```text
0 2 5 2 7
1 0 0 1 1
3 4 0 2 7
2 2 1
4 6 5
5 15 150.00
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
this is the edge case, N = 1 and x = 0, so everything should be 0 and the fine should still print as 0.00
```

Input:

```text
1 5
0
```

Expected output:

```text
0 0 0
0
0
0 0 0.00
```

Actual output:

```text
0 0 0
0
0
0 0 0.00
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
to check the maximum value (x = 5 everywhere) and also to check that P as a decimal (2.5) works and the fine is printed with 2 decimal places
```

Input:

```text
2 2.5
5 5
5 5
```

Expected output:

```text
5 5 2 10
5 5 2 10
2 2
10 10
4 20 50.00
```

Actual output:

```text
5 5 2 10
5 5 2 10
2 2
10 10
4 20 50.00
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
