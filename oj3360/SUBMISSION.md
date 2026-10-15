# Problem Solving Submission

This file must be written by the student in their own words.

Use this template only for OJ problems that are marked as learning-log required.

Do not ask AI to write this file for you. AI may help check grammar, formatting, or clarity after you have written your own content.

If AI was used for this learning-log-required problem, also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
3360
```

OJ submission ID, if submitted:

```text
683423
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
so the input will be in 3 lines. the 1st line have W H M N, W and H is the size of the bread, M is how many vertical knives and N is how many horizontal knives. the 2nd line is the X position of the M vertical knives and the 3rd line is the Y position of the N horizontal knives
the knives cut the bread into small pieces, every piece have its own area (width x height)
the output will be 2 numbers in 1 line, the biggest area and the 2nd biggest area of the pieces after cut. the bigger one go first, and it can be the same number if 2 pieces have the same area
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
Step 1: input W H M N then map it to int. then input the X line and Y line, and add 0 and W into the X list, add 0 and H into the Y list (so the edge of the bread is counted too)
Step 2: find the width of each strip by x[i+1] - x[i] and the height of each strip by y[i+1] - y[i], then sort both lists from big to small
Step 3: w1 w2 are the 2 biggest widths and h1 h2 are the 2 biggest heights. the biggest area is w1*h1
Step 4: the 2nd biggest area is max(w1*h2, w2*h1) because the other pieces can't be bigger than these
Step 5: print the biggest area then the 2nd biggest area
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
to check that my idea work with the example first. here the 2nd area come from w2*h1 (6*5)
```

Input:

```text
20 12 3 4
2 10 14
1 6 8 10
```

Expected output:

```text
40 30
```

Actual output:

```text
40 30
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
widths are 2 and 8, heights are 3 and 7. here the 2nd area is w1*h2 (8*3) bigger than w2*h1 (2*7), so I test that max() work for both cases
```

Input:

```text
10 10 1 1
2
3
```

Expected output:

```text
56 24
```

Actual output:

```text
56 24
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
the smallest case, bread is cut into 4 pieces that have same size. checks that the code not crash when there are only 2 widths and 2 heights
```

Input:

```text
2 2 1 1
1
1
```

Expected output:

```text
1 1
```

Actual output:

```text
1 1
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
