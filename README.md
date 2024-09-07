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

STRINGS ARE IMMUTABLE MEANS WE CANNOT CHANGE THEM ONCE WE HAVE CREATED THEM. IF WE JUST ONLY WANT TO CHANGE OR ALTER THE STRING WE CAN USE CONCATENATION AND SLICING BOTH:

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


























