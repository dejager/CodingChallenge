# CodingChallenge
Challenge: Print the number of **[JUMPROPE]** prefixed lines in an access.log

Write a function that accepts a path to a log file in the bundle, and returns how many lines start with “**[JUMPROPE]**”. The log file could be as large as 10GB, but may also not exist.

## Sample input and output
- If the log contains 100,000,000 lines and seven start with “**[JUMPROPE]**” your function should return 7.
- If the file does not exist, cannot be loaded, or contains zero lines starting with “**[JUMPROPE]**” your function should return 0.

## Hints
- **Hint #1:** You can use the contentsOfFile initializer for strings, but that's not very efficient.
- **Hint #2:** `FileHandle` is your friend, here. It can open a file and reads chunks of a size you specify.
- **Hint #3:** `FileHandle` doesn’t care about line breaks, so it will read as much data as you ask it too. It’s up to you to find the line breaks inside the chunk you read.
- **Hint #4:** Feel free to use Google, Apple Documentation, or other online resources.
