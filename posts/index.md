
# Print:

###### Usage: 
`print("Text/Numbers Here")`
`print(1+1)`
`print(*Variable Name*)`

`print ("Hello World")`      
Displays Hello World in the terminal

###### Pro tip: Python Has A In-Built Calculator If You Are Lazy

`print (“21+2 equals to”, 21 + 2)`
Displays 21+2 equals to (the answer of 21 + 2) 

You can use brackets for calculations like in real life calculations like:

`print ((1000*3)+790)`
Plus is +
Minus is -
Times is x
Divide is /
Equal is == **MUST BE TWO EQUALS!!!**

Advanced Code

edison = 250
print ("pro", "level", edison*3) = displays pro level 750
print (pro, "level", edison*3)    = displays skilled level 750 (pro is a variable set to the text “skilled”)

Booleans (True or False):
>>> print (bool(2+2 == 4))
True (answer is correct
>>> print (bool(20+20 == 30))  =  checks if 20 + 20 is 30
False (answer is incorrect)


# IF Statements

**Example**
world = 256
if (128+128 == world):
    print (“Hello World”)
else:
    print (“Bye World”)                   

Data Types:
Integer – Any non-decimal numbers
Boolean – True/False
Floating Point – Decimal numbers
String – Text

Input:
hello = input (“Hello, how are you doing today? “)
Can have more than one input like:
name = input (“What is your name? “)
favouritefood = input (“What is your favourite food? “)
Then:
print (hello) – will print the input you put in hello
You can use everything we learnt above here too, like:
print (“Hello, nice to meet you”, (name))
Guess the number minigame (puts what we learnt to use):
My own testing version:
n = random.randint (1,20)

guess = input ("Guess a number from 1-20 ")

if (guess == n):
    print ("You got it")
else:
    print ("Nope, try again")


Updated version (with teacher’s help):
count = 0

import random

number = random.randint(1,20)

while (True):
    guess = input("Guess a random number between 1-20 ")
    if (guess.isdigit() == True):
       print("It is a number!")
    if (int(guess) == int(number)):
        print ("Congratulations, you are right!")
        break;
    else:
        print ("Wrong... try again.")
        count = (count+1)
        print ("You have tried", count, "times.")



If/Else Statements:
 
Loops:
While Loop (from game code): 
guess = “not a number”
while(guess != number):

Another is For Loop
Functions:
To run your code in a more orderly manner.
Define:
def division(first, second)
def edison(first, second, third)
Use:
output = division(number, 2)
