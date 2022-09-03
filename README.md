# RandomPasswordGenerator-py

This project is about developing a password generator program that generates a random password which necessary includes 4 types of constraints in the generated password it much includes an upper and a lowercase letter, not just that but also numbers and symbols, this guarantee that the generated password have a great security 

In this document python language version 3.0 was, and for developing the program  Jupiter Notebook was used 

The modules that was used in this document was (Random, and String). Moreover, the concept of infinite loop was used so the program won’t stop after displaying the output and automatically re-run while loop was used for that . also (Try and Except) was used to prevent the program from crashing if it received the wrong input 

//////////////////////////////////////////////////////////////////////////////////////////////////////////////

2-	ALGORITHM

Step 1	Start
Step 2	Declare variable passwordPool including all printable string
Step 3	Display greeting to user 
Step 4	Start an infinite loop
Step 5	Get the passwordLength from the user 
Step 6	If the length of the passwordLength is not numeric 
    Display warning message that it should be numeric and go to step (5)
If the passwordLength is numeric 
   Continue to step 7
Step 7	If   the passwordLength is between 8 and 16 digits
     Create a random password based on the number of digits 
If the passwordLength out of the mentioned range 
     Display warning to the customer regarding the password length
     constraint and go back to (step 5)
Step 8	Stop

//////////////////////////////////////////////////////////////////////////////////////////////////////////////
4-	PSEUDOCODE
BEGIN
INITIALIZE passwordPool = (all sets of punctuation, digits, Upper_letters, Lower_letters ).
PRINT ‘Greeting to the user’
WHILE True :
	TRY:
READ passwordLength 
CAST passwordLength to Integer
IF passwordLength >7 AND passwordLength <17
CALCULATE password = Random((random(passwordPool[Digits],passwordLength // 4), random(passwordPool[Upper_Letters], passwordLength // 4),random(passwordPool[Lower_Letters], passwordLength // 4), random(passwordPool[punctuation],( passwordLength // 4+ passwordLength %4), passwordLenght)
ELSE
            DISPLAY “That the password should be numeric”
CATCH:
	DISPLAY “That only numbers are accepted as inputs*
END
//////////////////////////////////////////////////////////////////////////////////////////////////////////////

7-	CONCLUSION
After doing this project, I have learned many interesting things regarding to the python, by saying that I doesn’t only mean writing code, the scope is much broader where I’ve learned  
1-	What is Pseudocode, not only that but by searching for it on the internet, I understood the importance of it, furthermore I understood how many companies could take it as a red flag if you started to write the code right away without starting the pseudocode, the journey of learning how to do it from scratch and how to think for a solution for the problem you’re facing or a program you are writing was fun and it added so much to the way I think for solving problems

2-	Moreover, doing flowchart was fun to be honest as visualization part is my favorite part by doing flow chart I was introduced to the usage of MICROSOFT VISIO which became easier to work on after doing by flowchart

3-	Before doing that project, I was having a false understanding of the difference between an algorithm and code as I used to think that they are the same thing, however I can now understand that in the algorithm its better to avoid writing in codding syntax, as we should write in plain English 

4-	Writing the code was bit challenging but worth it, as I was trying to built the program using clean code to be easy to read, understood, or even modified, I went through many stages for reaching that code where at first I used the recursion function so it would call it self after the display of output, but I found out that removing the function and using the infinite while would be more logical, also for the random variables I found that rather having for variables for the 4 conditions it would be better to have only one variable and slice it, as if it is  a stratified sampling method
