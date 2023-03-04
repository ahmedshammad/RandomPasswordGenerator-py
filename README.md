# Random Password Generator

The Random Password Generator is a Python program that generates a random password that meets four constraints: it must include at least one uppercase letter, one lowercase letter, one number, and one symbol. This ensures that the generated password is secure and difficult to guess.

The program was developed using Python version 3.0 and Jupiter Notebook. The program uses the Random and String modules in Python. An infinite loop is used to keep the program running until the user is satisfied with the generated password. The Try and Except statement is used to prevent the program from crashing if the user enters the wrong input.
Algorithm

    Begin
    Declare the variable passwordPool, which includes all printable strings.
    Display a greeting message to the user.
    Start an infinite loop.
    Get the password length from the user.
    If the length of the password is not numeric, display a warning message to the user and go back to step 5.
    If the password length is numeric, continue to step 7.
    If the password length is between 8 and 16 digits, create a random password based on the number of digits.
    If the password length is not within the specified range, display a warning message to the user and go back to step 5.
    Stop.

Pseudocode

vbnet

BEGIN
    INITIALIZE passwordPool = (all sets of punctuation, digits, Upper_letters, Lower_letters).
    PRINT 'Welcome to the Random Password Generator!'
    WHILE True:
        TRY:
            READ passwordLength
            CAST passwordLength to Integer
            IF passwordLength > 7 AND passwordLength < 17:
                CALCULATE password = Random((
                    random(passwordPool[Digits],passwordLength // 4), 
                    random(passwordPool[Upper_Letters], passwordLength // 4),
                    random(passwordPool[Lower_Letters], passwordLength // 4),
                    random(passwordPool[Punctuation], passwordLength // 4 + passwordLength % 4), 
                    passwordLength))
                PRINT 'Your random password is:', password
                BREAK
            ELSE:
                DISPLAY 'Password length should be between 8 and 16 digits.'
        CATCH:
            DISPLAY 'Please enter only numeric values.'
END
