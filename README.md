Description

This program validates whether a given input number satisfies specific conditions using a Regular Expression (Regex) pattern matching approach. The program first checks whether the input is a valid six-digit number within the range 100000 to 999999. This is done using the regex pattern [1-9]\d{5}, which ensures that the number starts with a digit from 1 to 9 followed by exactly five digits. After validating the range condition, the program checks for the presence of alternating repetitive digit pairs in the number. An alternating repetitive digit pair occurs when the same digit repeats with exactly one digit between them, such as in 121 or 343. This is detected using the lookahead assertion regex pattern (\d)(?=\d\1). The program counts the number of such repetitive pairs and ensures that fewer than two pairs exist. If both conditions are satisfied, the program returns True; otherwise, it returns False. This solution avoids manual iteration and nested loops by using efficient regex operations, making the implementation simple, readable, and optimized for validation tasks.

Algorithm

Step 1: Read the input number as a string.
Step 2: Check whether the number matches the six-digit valid range using regex.
Step 3: Detect alternating repetitive digit pairs using lookahead regex.
Step 4: Count the number of detected repetitive pairs.
Step 5: If the count is less than two and range condition is satisfied, print True.
Step 6: Otherwise, print False.
