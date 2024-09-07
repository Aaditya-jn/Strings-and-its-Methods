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

STRINGS ARE IMMUTABLE MEANS WE CANNOT CHANGE THEM ONCE WE HAVE CREATED THEM. IF WE JUST ONLY WANT TO CHANGE OR ALTER THE STRING WE CAN USE CONCATENATION AND SLICING TOGETHER:

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
.starswitch()            ENSURES THE STARTING CHARACTER OF THE STRING.
.endswitch()             ENSURES THE ENDING CHARACTER OF THE STRING.

>>>name = "TonyStark"
>>>name.startwitch("To")
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
















































