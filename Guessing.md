flowchart TD
    Start([Start]) --> InputNumber["Input: User enters a guess"]
    InputNumber --> CheckGuess["Check: Is the guess correct?"]
    CheckGuess -- Yes --> EndGame["End: The user guessed correctly"]
    CheckGuess -- No --> Hint["Provide hint: Too high or Too low"]
    Hint --> Retry["User retries"]
    Retry --> InputNumber
    EndGame --> End([End])

    Description of the Guessing Game Process:
Start: The game initializes, and the system generates a random number within a specified range (e.g., 1-100).
Input Number: The user is prompted to input their guess.
Edge Case: If the input is not a number, an error message is displayed, and the user is prompted to try again.
Edge Case: If the input is out of the range, an error message is displayed, and the user is prompted to try again.
Check Guess: The system checks if the guessed number matches the random number.
Yes: If the guess is correct, the game ends, and a success message is shown.
No: If the guess is incorrect, the system provides a hint (either "too high" or "too low").
Retry: The user is prompted to guess again, and the process repeats until the correct guess is made.
End: Once the correct guess is made, the game ends\
git add Guessing.md
git commit -m "Added flowchart and description for the guessing game"
git push
