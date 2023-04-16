
## Print:

`print()` function is used to display output on the console or in a file

#### Usage: 
```
`print("Text/Numbers Here")` #Prints whatever in the brackets
`print(1+1)` #Prints the answer of 1+1
`print("Variable x is", x)` #Prints out "Variable x is (x variable)"
```

#### Examples
```
print ("Hello World")`
print(1+3) #Prints 4 in console because 1+3 = 4
```

#### Pro Tip: You can use brackets for calculations like in real life

```
print ((1000*3)+790)
```

Plus is +
Minus is -
Times is x
Divide is /
Equal is == **MUST BE TWO EQUALS!!!**

#### Advanced Code

edison = 250
pro = "skilled"
print ("pro", "level", edison*3) - displays pro level 750 
print (pro, "level", edison*3) - displays skilled level 750


## Booleans

-  Boolean Data Type: Booleans are a data type in Python that can have two values: `True` or `False`. 

For example:

```
is_sunny = True
is_raining = False
```



-  Boolean Expressions: Boolean expressions are expressions that evaluate to a Boolean value. 

For example:

```
x = 5
y = 3
is_greater = x > y   # True
is_equal = x == y     # False
```


- Advanced Code utilizing print()

```
print (bool(2+2 == 4)) #checks if 2+2 is 4

Output: True   - 2+2 == 4 is indeed correct

`print (bool(20+20 == 30))`  #checks if 20 + 20 is 30

Output: False   - 20+20 is not 30, outputs false
```


## If Statements

An `if` statement is a conditional statement in programming that allows the program to make decisions based on a certain condition. The basic structure of an `if` statement is:

```
if (condition):
```

The `condition` in the `if` statement is a Boolean expression that evaluates to either `True` or `False`. If the condition is `True`, then the code inside the `if` statement block will be executed. If the condition is `False`, then the code inside the `if` statement block will be skipped.

**Example**

```
world = 256
if (128+128 == world):
    print (“Hello World”)
else:
    print (“Bye World”)    
```               


## Data Types

Data types specify the type of data that can be stored in a variable. 
Common data types in Python includes:

Integer – Any non-decimal numbers
Boolean – True/False
Floating Point – Decimal numbers
String – Text

## Input

The `input()` function in Python is used to accept user input from the keyboard as a string. Here are some short notes and a brief explanation of the `input()` function:

`input()` Function: The `input()` function is a built-in function in Python that reads a line of text from the user and returns it as a string.

- Syntax: The basic syntax of the `input()` function is:

```
input([prompt])
```
   
   The `prompt` argument is optional and is a string that is displayed to the user before waiting for input.
   
- Example: using the `input()` function to accept user input and display it:

```
name = input("Enter your name: ") 
print("Hello, " + name + "!")
````
   
   In this example, the `input()` function is used to prompt the user to enter their name. The input is then tored in the `name` variable, which is used to display a personalized greeting message.

 - Type Conversion: The `input()` function returns a string, so if you need to use the input as a different data type, you need to convert it. For example, to accept a number from the user and use it in a mathematical operation, you can convert the input to an integer using the `int()` function:
   
```
num = int(input("Enter a number: "))
square = num ** 2
print("The square of", num, "is", square)
```
   
   In this example, the `input()` function is used to accept a number from the user as a string. The input is then converted to an integer using the `int()` function, and the square of the number is calculated and displayed.

## Guess the Number Minigame (self challange #1)

```
guess = input ("Guess a number from 1-20 ")

if (guess == n):
    print ("You got it")
else:
    print ("Nope, try again")
```


## Guess the number minigame (teacher's help)

```
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
```



## If/Else Statements:

Python supports the usual logical conditions from mathematics:

- Equals : a == b
- Not Equals: a !- b
- Less than: a < b
- Less than or equal to: a <= b
- Greater than: a > b
- Greater than or equal to: a >= b
- % means remainder

Example Code:

```
i=23

if i%2 == 0:
	print("This is the if block")
	print("i is an even number")
else:
	print("This is the else block")
	print("i is an odd number")
```




## Loops:
While Loop (from game code): 
guess = “not a number”
while(guess != number):


## Functions:
To run your code in a more orderly manner.
Define:
def division(first, second)
def edison(first, second, third)
Use:
output = division(number, 2)


## Array Lists

Array lists are a type of data structure that allow you to store and manipulate a collection of values. In Python, array lists are implemented using the `list` data type.

- Creation: You can create an array list in Python using square brackets and separating the values with commas.

```
fruits = ["apple", "banana", "cherry"]
```
  
- Accessing Elements: You can access individual elements in an array list using their index. In Python, index values start at 0. (Example for the list above: 0 is apple, 1 is banana, 2 is cherry etc.)

```
fruits = ["apple", "banana", "cherry"]
print(fruits[0])   # Output: "apple"
```
   
- Modifying Elements: You can modify individual elements in an array list by assigning a new value to their index.

```
fruits = ["apple", "banana", "cherry"]
fruits[1] = "orange"
print(fruits)   # Output: ["apple", "orange", "cherry"]
```
  
- Adding Elements: You can add new elements to an array list using the `append()` method.

```
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits)   # Output: ["apple", "banana", "cherry", "orange"]
```
  
- Removing Elements: You can remove elements from an array list using the `remove()` method.

```
fruits = ["apple", "banana", "cherry"]
fruits.remove("banana")
print(fruits)   # Output: ["apple", "cherry"]
```

- Length: You can find the number of elements in an array list using the `len()` function.

```
fruits = ["apple", "banana", "cherry"]
print(len(fruits))   # Output: 3
```

- Iterating: You can iterate over the elements of an array list using a `for` loop.

```
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
# Output:
# "apple"
# "banana"
# "cherry"
```