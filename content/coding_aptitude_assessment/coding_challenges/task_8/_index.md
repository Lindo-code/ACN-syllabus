---
_db_id: 762
content_type: project
flavours:
- any_language
prerequisites:
  hard:
  - coding_aptitude_assessment/coding_challenges/introduction
  - coding_aptitude_assessment/coding_challenges/how_to_name_files
protect_main_branch: false
tags:
- ncit-project
ready: true
submission_type: repo
title: 'Coding aptitude assessment challenge: Task 8'
---

Make a function to convert a number representing minutes into hours and minutes. It should **return** a string showing the number(s) of hours and minutes.

Pay very close attention to the format of the string that is returned:

- `task8(71)` should return `1 hour, 11 minutes`
- `task8(133)` should return `2 hours, 13 minutes`
- `task8(1)` should return `0 hours, 1 minute`

**Most people get this question wrong!**

Coders are precise so it is important to focus here. The output should show the number of hours and minutes, and it should make proper use of singulars and plurals.

## Check your understanding

- how is this similar to task 4? What lessons are you re-using here?
- can you think of different numbers you can pass into your function in order to test that it is working? Eg, what should `task8(0)` do? Does it do the right thing?
- imagine you were checking to see if someone else's code worked. What numbers would you pass in? What should the output be? Can you test your own code in the same way?
- when should the word "minute" be used? When should the word "minutes" be used?
- how about "hour" and "hours"