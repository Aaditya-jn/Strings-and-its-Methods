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

3. Print a string that spans multiple lines, with whitespace preserved.










