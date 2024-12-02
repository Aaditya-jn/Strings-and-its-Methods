# Strings-and-its-Methods

```
~Collection of text in python are called Strings. String methods are used to manipulate strings. String is a data-type used to represent text.
 IF WE WERE TO FIND THE TYPE OF A DATA TYPE LIKE HERE IN STRINGS, WE TYPE:
>>>type("Hello") 
<class 'str'>  DATA TYPE IS PRINTED WHICH IS STRING ALSO DENOTED BY str.

Strings have three properties that you’ll explore in the coming sec-tions:

1. Strings contain characters, which are individual letters or sym-bols.
2. Strings have a length, which is the number of characters contained in the string.      (LENGTH FUNCTION)
3. Characters in a string appear in a sequence, meaning each char-acter has a numbered position in the string.    (INDEXING)

```

```
~STRING LITERALS- SUPPOSE WE CREATE A VARIABLE name AND ASSIGN IT A VALUE:   name = "Aaditya". THE VALUE ASSIGNED IS THR STRING LITERAL. IT TELLS THAT
THE STRING IS LITERALLY WRITTEN ON OUR CODE RESPECTIVLEY

~THE QUOATATION MARKS WE USE ARE CALLED DELIMETRES. PYTHON ENSURES THAT WHILE WRITING A STRING, THE STARTING DELIMETRE AND THE ENDING DELIMETRE ARE OF THE SAME TYPE. FOR EX:

intro = "I am a boy. 'living in indore'. I study in college ".
HERE ABOVE WE USED TWO QUOATATION MARKS OR DELIMETRES AND WE ENSURED THAT THERE IS NO CONFUSION FOR THE PYTHON TO DETECT THE STARTING AND ENDING DELIMETRES.
~IF WE TRY TO USE DOUBLE QUOATES AND SINGLE QUOTES TOGETHER BUT WRONGLY PLACED THEN PYTHON WILL THROW A SYNTAX ERROR.

```

```
DETERMINING THE LENGTH OF A STRING- LENGTH OF A STRING IS CALCULATED BY THE len() FUNCTION. It gives the length of the string INCLUDING BLANK SPACES
AS WELL. for ex-
>>>print(len("Be Happy")) . IT COUNTS THE BLANK SPACES AS WELL.
8

We can also do like this:
>>>name = "Aaditya Jain"
>>>len_name = len(name)
>>>print(len_name)
12


MULTILINE STRINGS- PYTHON BOOK RECOMMENDS OF NOT MORE THAN 79 THE LENGTH OF A LINE
TO TACKLE THIS WE USE BACKSLASHES(/) OR """  """ TRIPLE QUOTES TO ENCLOSE THE BIG STRING IN IT

if variable's name is paragraph and then we do print(paragraph) then all the strings or characters will be printed excluding the backslashes becoz they are escape sequence characters. They are special.

```

```
PRACTICE QUESTIONS:

1. Print a string that uses double quotation marks inside the string.

>>>print("I study in acropolis college. It is a very good college")
I study in acropolis college. It is a very good college


2. Print a string that uses an apostrophe inside the string.

>>>print('I am a boy')
I am a boy

```

```
STRING CONCATENATION- TWO STRINGS CAN BE JOINED BY USING THE + OPERATOR.
>>>string1 = abra
>>>string2 = cadabra

>>>magic_string = string1 + string2
>>>print(magic_string)
abracadabra              NOTICE THAT THE STRINGS ARE JOINED WITHOUT ANY BLANK SPACES OR WHITESPACES BETWEEN THEM. TO ADD A BLANK SPACE:


>>>magic_word = string1 + " " + string2
>>>print(magic_word)
abra cadabra

```

```
STRING INDEXING- Each character in a string has a numbered position called INDEX.

>>>fruit = "pomegranate"
>>>print(fruit[4])
g

>>>veggies = "lady finger"
>>>print(veggies[11])

AN INDEX ERROR ARISES WHERE IT IS SAYING THAT STRING INDEX IS OUT OF RANGE.

```

```
STRING SLICING- SUPPOSE WE DO NOT WANT TO PRINT THE STRING FULL, ie WE WANT SOME PART OF IT ONLY THEN WE USE STRING SLICING.

>>>print(fruit[0:5])
pomeg                            fruit[0:5] MEANS INDEX FROM 0 to 4 CHARACTERS WILL BE PRINTED. THE CHARACTERS PRINTED AFTER SLICING IS CALLED A SLICE.

STRINGS ARE IMMUTABLE MEANS WE CANNOT CHANGE THEM ONCE WE HAVE CREATED THEM. IF WE JUST ONLY WANT TO CHANGE OR ALTER THE STRING WE CAN USE CONCATENATION AND SLICING TOGETHER: IF WE WANT TO ALTER A STRING, WE MUST CREATE AN
ENTIRELY NEW STRING.

>>>word = "goal"
>>>word = "f" + word[1:len(word)]
>>>print(word)
foal

```

```
PRACTICE QUESTIONS:

1. Create a string and print its length using the len() function.

>>>college = "Acropolis"
>>>len_college = len(college)
>>>print(len_college)
9

2. Create two strings, concatenate them, and print the resulting string.

>>>name1 = "Aaditya"
>>>name2 = "Jain"

>>>new_name = name1 + name2
>>>print(new_name)
AadityaJain


3. Create two strings and use concatenation to add a space in-between them. Then print the result.

>>>new_naam = name1 + " " + name2
>>>print(new_naam)
Aaditya Jain


4. Print the string "zing" by using slice notation on the string "bazinga" to specify the correct range of characters.

>>>my_word = "bazinga"
>>>my_word = my_word[2:6]
>>>print(my_word)
zing

```

```
STRINGS COME WITH SPECIAL BUNDLE METHODS CALLED STRING METHODS. THEY ARE IN HUGE QUANTITY BUT WE WILL ONLY
LEARN A FEW, THESE METHODS ARE BENEFICIAL TO MANIPULATE STRINGS.

To convert all the letters or upper case letters of string to lower case, we use .lower() method
THIS IS APPLIED AT THE END OF THE STRING.

>>>"My Name IS AADitya JaIn".lower()
'my name is aaditya jain'

WE CAN ALSO USE THIS METHOD LIKE BELOW:

>>>intro = "My Name IS AADitya JaIn"
>>>print(intro.lower())
my name is aaditya jain

SIMILARLY THERE IS ANOTHER METHOD TO CONVERT ALL LOWER CASE LETTERS TO UPPER CASE WHICH IS .upper()

>>>print(intro.upper())
MY NAME IS AADITYA JAIN

WHITESPACE METHOD- WHITESPACE IS SOMETHING THAT IS PRINTED AS A BLANK SPACE

THERE ARE THREE METHODS TO REMOVE WHITESPACE
.rstrip()   REMOVES WHITESPACE FROM RIGHT SIDE OF THE STRING.
.lstrip()   REMOVES WHITESPACE FROM LEFT SIDE OF THE STRING.
.strip()    REMOVES WHITESPACE FROM RIGHT AND LEFT SIDE  OF THE STRING.

TWO MORE STRING METHODS:
.startswith()            ENSURES THE STARTING CHARACTER OF THE STRING.
.endswith()             ENSURES THE ENDING CHARACTER OF THE STRING.

>>>name = "TonyStark"
>>>name.startswith("To")
True

>>>name.endswith("ks")
False

```

```
PRACTICE QUESTIONS:

1. Write a script that converts the following strings to lowercase: "Animals", "Badger", "Honey Bee", "Honeybadger". Print each lowercase string on a separate line.

>>>tuple = ("Animals", "Badger", "Honey Bee", "Honeybadger")
>>>no1 = tuple[0]
>>>no2 = tuple[1]
>>>no3 = tuple[2]
>>>no4 = tuple[3]

>>>print(no1.lower())
>>>print(no2.lower())
>>>print(no3.lower())
>>>print(no4.lower())

animals
badger
honey bee
honeybadger


2. Repeat Exercise 1, but convert each string to uppercase instead of lowercase.

>>>no1 = tuple[0]
>>>no2 = tuple[1]
>>>no3 = tuple[2]
>>>no4 = tuple[3]

>>>print(no1.upper())
>>>print(no2.upper())
>>>print(no3.upper())
>>>print(no4.upper())

ANIMALS
BADGER
HONEY BEE
HONEYBADGER


3. Write a script that removes whitespace from the following strings:
string1 = "    Filet Mignon"
string2 = "Brisket   "
string3 = "   Cheeseburger  "
Print out the strings with the whitespace removed.


print(string1.rstrip())
print(string2.lstrip())
print(string3.strip())

Filet Mignon
Brisket
Cheeseburger


4. Write a script that prints out the result of .startswith("be") on each of the following strings:
string1 = "Becomes"
string2 = "becomes"
string3 = "BEAR"
string4 = "bEautiful"

string1.startswith("be")
string2.startswith("be")
string3.startswith("be")
string4.startswith("be")

False
True
False
False


5. Using the same four strings from Exercise 4, write a script that uses string methods to alter each string so that .startswith("be") returns True for all of them.

string1.lower()
string2 does not need to be altered.
string3.lower()
string4.lower()

TRUE
TRUE
TRUE
TRUE

```

```
INPUTS- IN THIS TOPIC WE WILL LEARN HOW TO GET INPUT FROM THE USER AND DISPLAY BACK IT ON  THE SCREEN USING THE input() FUNCTION.
If we write input() in IDLE then actually nothing happens on front-end but the prompt(>>>) do not get displayed on the another line. IT MEANS THAT WE HAVE TO TYPE SOME TEXT!

>>>input()
<In next line nothing happened but prompt is also not visible>
"Hello"
'Hello'
>>>

THE TEXT WE ENTERED IS REPEATED ON A NEW LINE WITH SINGLE DELIMETRES. THIS IS BECAUSE INPUT FUNCTION RETURNS A TEXT AS A STRING.

>>>input()
5
'5'
>>>

TO BE MORE USER-FRIENDLY TO THE INPUT, WE NEED TO GIVE IT SOME PROMPT(STRING): few examples:

>>>prompt = "Hi, What's your profession?"
>>>user_input = input(prompt)
>>>print("My profession is: ", user_input)
Hi, What's your profession?Prompt engineer
My profession is: Prompt engineer

```

```
PRACTICE QUESTIONS OF INPUTS:

1. Write a script that takes input from the user and displays that input back.

>>>input()
I am 18 years old
'I am 18 years old'
>>>

2. Write a script that takes input from the user and displays the input in lowercase.

>>>language = "FREncH"
>>>input(language.lower())
french

3. Write a script that takes input from the user and displays the number of characters inputted.

>>>work = input("where do you work?")
>>>print(len(work))
where do you work?McKinsey
8
>>>

```

```
CHALLENGE QUESTION:

3.Write a script named first_letter.py that ﬁrst prompts the user for input by using the string "Tell me your password:" The script should
then determine the ﬁrst letter of the user’s input, convert that letter to upper-case, and display it back.

>>>first_letter = input("Tell me your password:")
>>>user_input = first_letter[0]
>>>print("The first letter of the password is " + user_input.lower())

Tell me your password:No
The first letter of the password is n.

```

```
STRINGS AMD ARITHMETIC OPERATORS:

>>>num = "6"
>>>digit = "9"
>>>print(num + digit)
69

Note here that the result expected was 15 but here camee 69!. THERE'S A REASON FOR THAT TOO.
HERE 6 IS NOT A INTEGER, IT IS A STRING BCOZ OF DOUBLE QUOTATION MARKS, SIMILARLY SAME FOR 9 TOO.
HERE ACTUALLY STRING CONCATENATION HAPPENED INVISIBLY BECOZ WE HAVE NOT LEARNT IT WITH NUMBERS MUCH. BUT WITH THISS EXAMPLE WE LEARNED IT.

>>>num = "7"
>>>print(num * 3)
777

HERE 7 IS REAPEATED THREE TIMES NOT THAT 7 * 3. BECOZ 7 HERE IS A STRING

In other words, multiplying a string by an integer n concatenates that string with itself n times.

When the * operator is used with a string on either the left or the right side, it always expects an integer on the
other side. FOR EX:

>>>print("12" * "3")
Traceback (most recent call last):
  File "/usr/lib/python3.12/idlelib/run.py", line 580, in runcode
    exec(code, self.locals)
  File "<pyshell#39>", line 1, in <module>
TypeError: can't multiply sequence by non-int of type 'str'

Python can only concatenate str (not "int") to str.

```

```
TYPECASTING: CONVERTING STRINGS TO NUMBERS AND VICE VERSA. SAME FOR THE FLOAT DATA TYPE ALSO.

To perform arithmetic operations on a string which contains numbers, first we have to convert it to int type from str type by using two
methods, int and float.

>>>print(type(int("12")))
<class 'int'>

>>>int("12.0")
Traceback (most recent call last):
  File "/usr/lib/python3.12/idlelib/run.py", line 580, in runcode
    exec(code, self.locals)
  File "<pyshell#6>", line 1, in <module>
ValueError: invalid literal for int() with base 10: '12.0'

Even though the extra 0 after the decimal place doesn’t add any value to the number, Python won’t change 12.0 into 12 because it would 
result in the loss of precision.

>>>nums = input("Enter your number:", )
>>>user_input = int(nums) * 2
>>>print(user_input)
Enter your number:5
10


>>>fries_value = 80
>>>var = "I want to eat" + fries_value + fries
>>>print(var)
Traceback (most recent call last):
  File "/usr/lib/python3.12/idlelib/run.py", line 580, in runcode
    exec(code, self.locals)
  File "<pyshell#14>", line 1, in <module>
TypeError: can only concatenate str (not "int") to str

BUT TO JUST CORRECT THIS CODE:

>>>fries_value = 80
>>>print("I want to eat" +  str(fries_value)  + "fries")
I want to eat80fries

ALSO BELOW CODE WILL ALSO GIVE THE SAME OUTPUT:
>>>print("I want to eat" +  str(80)  + "fries")

str CAN ALSO HANDLE ARITHMETIC OPERATIONS:

>>>aloo_parathax = 6
>>>aloo_parathay = 2
>>>print("Nah!" +  "Only"  +  str(aloo_parathax - aloo_parathay)  +  "paratha"  +  "left")
Nah!Only4parathaleft

```

```
PRACTICE QUESTIONS OF TYPECASTING:

1. Create a string containing an integer, then convert that string into an actual integer object using int(). Test that your new object is
a number by multiplying it by another number and displaying the result.

>>>strz_int = "5"
>>>print(strz_int * 3)
WE GET THE OUTPUT HERE AS 555, NOW CONVERTING IT TO INT DATA TYPE;

>>>str_intz = int("5")
>>>print(str_intz * 5)
HERE WE GET THE OUTPUT AS 25 WHICH IS OUR REQUIRED OUTPUT.


2. Create a string object and an integer object, then display them side-by-side with a single print statement by using the str() function.

>>>daily_brush = 2
>>>print("I brush"  +  str(2)  +  "times a day")
I brush2times a day


4. Write a script that gets two numbers from the user using the input() function twice, multiplies the numbers together, and
displays the result. If the user enters 2 and 4, your program should print the following text: The product of 2 and 4 is 8.0.

>>>x = int(input("Enter 1st no.:", ))
>>>y = int(input("Enter 2nd no.:", ))

>>>z = float(x * y)
>>>print("The product of 2 and 4 is", z)
The product of 2 and 4 is 8.0

```

```
F-STRINGS:
REMEMBER THIS EXAMPLE WE HAD DONE:

>>>fries_value = 80
>>>print("I want to eat" +  str(fries_value)  + "fries")
I want to eat80fries

WLL THIS WAS AA GOOD METHOD FOR CONVERTING NUMBERS TO STRINGS AND THEN USE THEM IN SENTENCES.
WE HAVE ANOTHER SHORT METHOD TO DO THIS CALLED F-STRINGS:

Suppose we have a name variable which has a value Tony and two other variables hands and legs.
WE WANT TO CREATE A SENTENCE AS: Tony has 2 hands and 3 legs. WE WILL DO IT LIKE BELOW;

>>>name = "Tony"
>>>hands = 2
>>>legs = 3

>>>f"{name} has {hands} hands and {legs} legs".
'Tony has 2 hands and 3 legs'

>>>n = 3
>>>m = 4
>>>f"{n} times {m} is {n * m}"
'3 times 4 is 12'

```

```
PRACTICE QUESTIONS:

1. Create a float object named weight with the value 0.2, and create a string object named animal with the value "newt". Then use these
objects to print the following string using only string concatenation: 0.2 kg is the weight of the newt.

weight = 0.2
animal = "newt"

print(str(0.2) + " " + "kg" + " " + "is" + " " + "the" + " " + "weight" + " " + "of" + " " + "the" + " " + "newt")
'0.2 kg is the weight of the newt'

2. Display the same string using an f-string.

f"{weight} kg is the weight of the {animal}"
'0.2 kg is the weight of the newt'

```

```
FINDING STRING IN A STRING OR FINDING SUBSTRING:
For this we use .find() . THIS METHOD RETURNS THE INDEX OF THE WORD WE WANT TO FIND.

>>>prompt = "I am a boy"
>>>prompt.find("am")
2

If .find() doesn’t ﬁnd the desired substring, it will return -1 instead.

IF IN A SITUATION, A SUBSTRING OCCURS 2 OR MORE TIMES IN A SENTENCE THEN .find()
RETURNS THE INDEX OF THE SUBSTRING WHICH OCCURS FIRST STARTING FROM BEGINNING.

>>>sentence = "I put a string in a string"
>>>sentence.find("string")
8

.find() ALSO ACCEPTS STRING AS A INPUT. IF WE SEARCH FOR A NUMBER, IT RAISES A TYPERROR. IF WE WANT TO FIND NO.S ALSO THEN:

>>>phone_no = "8765357204"
>>>phone_no.find("0")
8

```

```
PRACTICE QUESTIONS:

1. In one line of code, display the result of trying to .find() the substring "a"
in the string "AAA". The result should be -1.

>>>"AAA".find("a")
-1

2. Replace every occurrence of the character "s" with "x" in the string
"Somebody said something to Samantha.".

>>>"Somebody said something to Samantha.".replace("s", "x")
'Somebody xaid xomething to Samantha.'


3. Write and test a script that accepts user input using the input() function and displays
the result of trying to .find() a particular letter in that input.

str = input("Enter your string :")
print(str.find("d"))

```

```
CHALLENGE QUESTION:

Write a script called translate.py that asks the user for some input
with the following prompt: Enter some text:. Then use the .replace()
method to convert the text entered by the user into “leetspeak” by mak-
ing the following changes to lower-case letters:
• The letter a becomes 4
• The letter b becomes 8
• The letter e becomes 3
• The letter l becomes 1
• The letter o becomes 0
• The letter s becomes 5
• The letter t becomes 7
Your program should then display the resulting string as output. Be-
low is a sample run of the program:

Enter some text: I like to eat eggs and spam.
I 1ik3 70 347 3gg5 4nd 5p4m.


>>>my_text = input("Enter some text: ")

>>>my_text = my_text.replace("a", "4")
>>>my_text = my_text.replace("b", "8")
>>>my_text = my_text.replace("e", "3")
>>>my_text = my_text.replace("l", "1")
>>>my_text = my_text.replace("o", "0")
>>>my_text = my_text.replace("s", "5")
>>>my_text = my_text.replace("t", "7")

>>>print(my_text)
I 1ik3 70 347 3gg5 4nd 5p4m.

```





























































































