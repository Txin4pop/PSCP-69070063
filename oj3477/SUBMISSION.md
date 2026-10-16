# Problem Solving Submission

This file must be written by the student in their own words.

Use this template only for OJ problems that are marked as learning-log required.

Do not ask AI to write this file for you. AI may help check grammar, formatting, or clarity after you have written your own content.

If AI was used for this learning-log-required problem, also complete `ai_reflection.md`.

---

## 1. OJ Information

OJ problem number/title:

```text
3477
```

OJ submission ID, if submitted:

```text
687615
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
so the input will be in 2 parts. the first part is many lines of ingredients, and we keep reading until we see the word "Cook". the second part is many lines of tastes, and we keep reading until we see the word "End".

the chef has a list of 11 ingredients that are allowed (Pad Thai Sauce, Tofu, Pickle Turnip, Shrimp, Bean Sprouts, Noodle, Chives, Lime, Egg, Oil, Peanuts). the chef wants exactly these 3 tastes: Sweet, Sour, Salty.

the output is only 1 line, what the chef says:
- if there is any ingredient that is not in the list (even if the others are complete or not) then print "This is not Pad Thai!!!"
- else if the ingredients are not complete (some of the 11 are missing) then print "This is bad!" (the chef doesn't care about the taste)
- else if the ingredients are complete but the taste is not exactly Sweet, Sour, Salty (missing one or has another taste) then print "Not Bad..."
- else (ingredients complete and taste is exactly the 3) then print "Delicious!"
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
Step 1: make a set of the 11 allowed ingredients and a set of the 3 required tastes.
Step 2: use a while loop to input a line, strip it, and stop if it is "Cook", otherwise add it into the ingredient set (set so duplicates don't matter).
Step 3: do the same with another while loop for tastes, stop at "End", and add each line into the taste set.
Step 4: check the ingredients first. if the ingredient set is not a subset of the allowed set (has an outsider) then print "This is not Pad Thai!!!"
Step 5: else if the ingredient set is not equal to the allowed set (something missing) then print "This is bad!"
Step 6: else if the taste set is not equal to {Sweet, Sour, Salty} then print "Not Bad..."
Step 7: else print "Delicious!"
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
this is the normal best case. all 11 ingredients and exactly the 3 tastes, so it checks that the program can reach the last branch
```

Input:

```text
Pad Thai Sauce
Tofu
Pickle Turnip
Shrimp
Bean Sprouts
Noodle
Chives
Lime
Egg
Oil
Peanuts
Cook
Sweet
Sour
Salty
End
```

Expected output:

```text
Delicious!
```

Actual output:

```text
Delicious!
```

Result:

```text
Pass
```

### Test Case 2

Why I chose this case:

```text
Peanuts is missing but the taste is complete. i want to check that the chef ignores the taste when the ingredients are not complete
```

Input:

```text
Pad Thai Sauce
Tofu
Pickle Turnip
Shrimp
Bean Sprouts
Noodle
Chives
Lime
Egg
Oil
Cook
Sweet
Sour
Salty
End
```

Expected output:

```text
This is bad!
```

Actual output:

```text
This is bad!
```

Result:

```text
Pass
```

### Test Case 3

Why I chose this case:

```text
Garlic is not in the list
```

Input:

```text
Pad Thai Sauce
Tofu
Garlic
Shrimp
Cook
Sweet
Sour
Salty
End
```

Expected output:

```text
This is not Pad Thai!!!
```

Actual output:

```text
This is not Pad Thai!!!
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
| I wrote this submission in my own words. |Yes |
| I understand my final code. | Yes|
| I recorded the real OJ status. | Yes|
| I did not copy AI-generated text directly into this file. | Yes|
| I did not copy code from another person. | Yes|
| If I received human help, I disclosed it in this file. | Yes|
| I submitted the final code to the OJ by myself. | Yes|
