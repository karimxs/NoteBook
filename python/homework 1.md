Part 1: The Basics of Variables

1. What is a variable?
	In Python, a variable works more like a sticky note (label) than a box. When you create a variable (e.g. x = 5), the computer creates the value 5 in memory, then "sticks" a note with the name x to it. If you later write x = 10, the computer will simply take the note x and stick it to a new value (10).

2. What are variables called?
	(Iron rules) For the code to work, variable names must follow a number of "legal" rules:

Letters, numbers, and underscores: The name can only contain these (e.g. my_var_1).

It is not allowed to start with a number: The name var1 is valid, but 1var generates an error.

Case Sensitivity: The variable age is completely different from the variable Age.

Reserved words: You can't use words that already have a meaning in Python (like if, for, True).

Recommendation: It's common to use an underscore to separate words (Snake Case), for example: first_name.

3. What is "Dynamic Typing"?
This means that Python automatically recognizes the type of the data, and you don't need to declare it in advance. Also, because a variable is just a "sticky note", you can pass it from one data type to another without crashing the computer. So, it's perfectly fine to write x = 10 (a number) and then immediately write x = "Ten" (a word). The note just moved to another place.

Part 2: Understanding Data Types

4. What are the 4 primitive (basic) data types?
These are the building blocks of data in Python:

int (integer): Real-world example - number of students in a class (there can't be 20.5 students).

float (decimal number): Real world example - the price of a product in a store (e.g. 19.99 NIS) or weight.

str (String): Real world example - your name, or residential address (text).

bool (Boolean): Real world example - is the light in the room on? (yes/no, true/false).

5. What is the difference between Integer and Float?
An Integer is a whole number without a decimal point (e.g. 5). A Float is a number that includes a decimal point (e.g. 5.0 or 3.14). Python sometimes converts 5 to 5.0 (from int to float) when we perform arithmetic operations such as division, to maintain maximum precision (e.g. 5 / 2 = 2.5).
+1

6. What are Strings?
Strings are simply text. We must put quotes (single or double) around the text to tell Python that it is a number. Textual, not a code command or variable name. If we "join" two strings together with a plus sign, like "Hello" + "World", Python will simply paste them together and produce the string "HelloWorld".

Part 3: Handling Data

7. What is Type Casting?
This is the process of changing a data type from one type to another. If we received the number 10 from the user, but it was stored as text ("10"), we cannot perform arithmetic operations on it. To convert it to a real number, we use the int() conversion function. For example: real_number = int("10").

8. What are Booleans? Booleans are a data type that can only take one of two states: True or False. They help the computer make decisions (for example: Is the password correct? If True, let the user log in). The uppercase "T" and "F" are critical because Python is case sensitive. to uppercase letters. The words true or false in lowercase letters simply will not be recognized by it and will cause an error.

9. How do you check what type a variable is? If you get lost in the code and want to ask Python "What data type does this variable currently hold?", you use the built-in function type().
For example: print(type(x)) will print the type of the variable to the screen