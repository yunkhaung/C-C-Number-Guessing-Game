# C/C++ -Number-Guessing-Game
Memory Game Overview:
This program implements a memory game using an mbed microcontroller with a USB
interface, LCD display, and keypad connected to a PC Terminal.
Connection Establishment: The workflow scans and connects to the first available COM
port. Opens a communication with a baud rate of 9600 and 8N1 configuration.
Logging: Opens a CSV - gameplay.csv - for logging messages. Logs all the interactions,
both prompts and inputs, along with game events. After every game is finished, one csv file
per game is created in the same directory as the programs.
Gameplay Flow: It asks the user to choose a difficulty level. Difficulty level determines how
long the sequence will appear for; Hard being half a second, Medium being one second and
Easy being two seconds. Controls the gameplay by reading in user input and its validation.
Provides options to replay or exit once the game is over.
Error Handling: Ensures that no invalid input disrupts the flow of the game. Inappropriate
user action shows the corresponding error messages.
