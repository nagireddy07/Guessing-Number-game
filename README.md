
The Java program described above is a simple console-based guessing game where the user tries to guess a randomly generated number between 1 and 10. The program provides feedback on whether the user's guess is too high or too low, and it continues to prompt for guesses until the correct number is guessed. It also keeps track of the number of attempts the user makes to guess the correct number.

Detailed Steps and Components:
Imports and Initialization:

The program imports the Scanner class from the java.util package to handle user input.
It imports the Random class from the java.util package to generate a random number.
An instance of Scanner is created to read input from the console.
An instance of Random is created to generate a random number.
Random Number Generation:

The program generates a random number between 1 and 10 using the Random object. This is done using the nextInt(10) + 1 method, where nextInt(10) generates a number from 0 to 9, and adding 1 shifts the range to 1 to 10.
User Interaction:

The program welcomes the user and informs them about the game.
It enters a while loop that continues until the user guesses the correct number.
Inside the loop, the program prompts the user to enter their guess using System.out.print and reads the input using scanner.nextInt().
Guess Evaluation and Feedback:

After reading the user's guess, the program increments the attempts counter to keep track of the number of guesses.
It compares the user's guess to the randomly generated number:
If the guess is less than the random number, it prints "Too low! Try again."
If the guess is greater than the random number, it prints "Too high! Try again."
If the guess is equal to the random number, it prints a congratulatory message and the number of attempts taken to guess the number correctly.
Loop Termination:

The loop continues to prompt for guesses and provide feedback until the user guesses the correct number.
When the correct number is guessed, the loop terminates, and the program displays the total number of attempts.
Program Termination:

After the correct guess and final message, the program closes the Scanner object using scanner.close() to free up resources.
