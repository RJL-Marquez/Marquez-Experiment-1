# Marquez Experiment #1
## 1. ALPHABET SOUP PROBLEM

 Create a function that takes a string and returns a string with its letters in alphabetical order.
 ```python
#Alphabet Soup Problem
#Creating Input Interface
words = input("Enter your word to be sorted: ")

#Using 'def' to define a function in preparation for sorting
def alphabet_soup(words):

#Using the 'sorted' function to arrange the letters alphabetically
#Using the 'join' function to merge all elements into one string after sorting
    i = ''.join(sorted(words))
    return i

#Assigning the function to a variable
out = alphabet_soup(words)

#Output
print(out)

#End of code
```
## 2. EMOTICON PROBLEM

Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:
 ```python
#Emoticon Problem
#Creating Input Interference
sentence = input("Enter text: ")

#Split the words into separate strings using '.split'
i = sentence.split(' ')

#Create a dictionary to have a key:value pairs for emoticon conversion
emoji_coverter = {
        "smile":":)",
        "grin":":D",
        "sad":":((",
        "mad":">:("
        }

#Initializing a blank variable in preparation for the for-loop
converted = ""

#Using for-loop reinstate the statement but with a converted emoticon
for word in i:
    converted += emoji_coverter.get(word, word) + " "

#Output
print(converted)
    
#End of code
```
## 3. UNPACKING LIST PROBLEM

Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

 ```python
##Unpacking List Problem
#Create a placeholder for the number list
numberlist = []

#Create an interval variable for for-loop
x=0

#Create a for-loop for users to input their numbers
while True:
    number = int(input("Enter a number: "))
    numberlist.append(number)
    
#The loop will constantly add integers to the list
    x=x+1
    
#User have the freedom to choose whether to add more numbers or stop   
    choice = input("Add more number? (y/n): ")
    if choice.casefold() == 'n':
        break

#Assigning the first and last number from the list into separate variables
first=numberlist[0]
last=numberlist[x-1]

#Deleting the first and the last number from the list
del numberlist [0]
del numberlist [x-2]

#Output
print("first: ", first, "\t middle: ", numberlist, "\t      last: ", last)

#End of code
```
