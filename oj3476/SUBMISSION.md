# Problem Solving Submission

This file must be written by the student in their own words.

Use this template only for OJ problems that are marked as learning-log required.

Do not ask AI to write this file for you. AI may help check grammar, formatting, or clarity after you have written your own content.

If AI was used for this learning-log-required problem, also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
3476
```

OJ submission ID, if submitted:

```text
683664
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
so the input will be n lines, the first line is n, then n lines that each have 1 dict that look like {"name" : "Cat05"} so key is the name of the cat or fox and value is the number that have Cat or Fox in front
the output will be the total of cat, the total of fox, then print the name and number of every cat and then every fox, sort by the number
if Cat01 is not in the input then it is Garfield and if Fox01 is not in the input then it is Fubuki but if the name Garfield or Fubuki is already used by someone else then dont add it because the name cant repeat
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
Step 1: input n then loop n times, for each line use strip and strip('{}') then split(':') to get name and number, then remove the quote with strip and put it in dict d with the number as key and name as value
Step 2: use setdefault or check if 'Cat01' not in d and 'Garfield' not in d.values() then d['Cat01'] = 'Garfield', do the same with 'Fox01' and 'Fubuki'
Step 3: make cats list from the key that startswith 'Cat' and foxes list from the key that startswith 'Fox' then sort with int(k[3:]) so Cat10 is after Cat02
Step 4: print 'Cat :' and len(cats), print 'Fox :' and len(foxes), then loop cats and foxes and print name : number
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
same as my frist plan
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
because Garfield is already the name of Fox06, so we cant add Garfield to Cat01 (no repeat name), the cat count stay 3
```

Input:

```text
7
{"Fubuki" : "Fox05"}
{"Shiro" : "Fox01"}
{"Garfield" : "Fox06"}
{"Kin" : "Cat05"}
{"Okayu" : "Cat03"}
{"Kuro" : "Fox02"}
{"Tom" : "Cat07"}
```

Expected output:

```text
Cat : 3
Fox : 4
Okayu : Cat03
Kin : Cat05
Tom : Cat07
Shiro : Fox01
Kuro : Fox02
Fubuki : Fox05
Garfield : Fox06
```

Actual output:

```text
Cat : 3
Fox : 4
Okayu : Cat03
Kin : Cat05
Tom : Cat07
Shiro : Fox01
Kuro : Fox02
Fubuki : Fox05
Garfield : Fox06
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
to check that the program do NOT add Garfield and Fubuki when Cat01 and Fox01 already have a name
```

Input:

```text
3
{"Mimi" : "Cat01"}
{"Kitsune" : "Fox01"}
{"Luna" : "Cat02"}
```

Expected output:

```text
Cat : 2
Fox : 1
Mimi : Cat01
Luna : Cat02
Kitsune : Fox01
```

Actual output:

```text
Cat : 2
Fox : 1
Mimi : Cat01
Luna : Cat02
Kitsune : Fox01
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
because it has Cat10 and Cat02, if i sort as string Cat10 will come before Cat02 so it is wrong, this test check that i sort by int(k[3:]). It also have no fox in the input at all so Fubuki is added alone
```

Input:

```text
2
{"Tom" : "Cat10"}
{"Chi" : "Cat02"}
```

Expected output:

```text
Cat : 3
Fox : 1
Garfield : Cat01
Chi : Cat02
Tom : Cat10
Fubuki : Fox01
```

Actual output:

```text
Cat : 3
Fox : 1
Garfield : Cat01
Chi : Cat02
Tom : Cat10
Fubuki : Fox01
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
