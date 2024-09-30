flowchart TD 
    Start([Start])--> RandomNumbner[Generate Random Number]
    RandomNumber--> UserInput[Get User Input]
    UserInput--> Decision{Is Guess Correct?}
    Decision --> |Yes| End([End])
    Decision --> |No| CheckGuess{Too High or Too Low}
    CheckGuess --> |Too High| GiveFeedback[Feedback: Too High]--> UserInput
    CheckGuess--> |Too Low| GiveFeedback[Feedback: Too Low]--> UserInput
The "flowchart TD" indicates that this flowchart is going from Top Down. Then the start endicates the beginning of the game, the program begins the guessing game. Then the program generates a random number within a range like 1 to 50. This is the number the user is attempting to guess. It is important to make sure the random number is properly generated each time the game starts to avoid the same number being guessed twice. Next the user will be prompted to give a guess, during this step the input validation is crucial to ensure the guess is in the specific range. An edge case in this part is how to handle non-numeric inputs and numbers that are outside of the valid range should result in error messages or feedback for a valid imput. Then the decision nose checks if the user's guess matches the random number that was generated. If the guess was correct then the game ends and the user wins. But if the guess is incorrect, the game moves to giving feedback based on the guess being too high or too low. This continues until the use guesses the corretc number. The feedback part is a essential part of the user experience because is lets the user know whether their guess was too high or too low, so that they can adjust their number input.
