# ALUNING_2ECEA_PA1
This repository includes Python programs that provide solutions to three (3) problems from Program Assignment 1: Introduction to Python Programming.

---
## 1. ALPHABET SOUP PROBLEM
**Problem:** Create a function that takes a string and returns a string with its letters in alphabetical order <br>
**Code Process:**
1. The program prompts the user to type in a word, which will be stored as a string (w).
2. The string (w) is then converted into a list of characters.
3. The list of characters is sorted alphabetically using the .sort() function.
4. The sorted list is then combined back into a string.
5. Finally, the program prints the result — the word’s letters arranged alphabetically.

**Example:** <br>
input: yesha <br>
output: aehsy

---

## 2. EMOTICON PROBLEM
**Problem:** Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticon: <br> 
**Code Process:**
1. The program defines a function emotify(sentence) that takes a string as input.
2. Inside the function, the sentence is checked for specific words:
   * smile → replaced with :)
   * grin → replaced with :D
   * sad → replaced with :(
   * mad → replaced with >:( <br>(This is done using the .replace() function.)
3. The updated sentence with emoticons is returned by the function.
4. The user is prompted to type in a sentence, which is stored in user_input.
5. The function emotify(user_input) is called, and its result is stored in result.
6. Finally, the program prints the sentence with words replaced by emoticons.

**Example:** <br>
input: i smile bcz of cali <br>
output: i :) bcz of cali

---

## 2. UNPACKING LIST PROBLEM
**Problem:** Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables <br> 
**Code Process:**
1. The program prompts the user to enter numbers separated by spaces, which are stored as a string (user_input).
2. The string is split into individual pieces using .split(), and each piece is converted into an integer. These numbers are stored in a list (X).
3. The list is then unpacked into three parts:
   * first → the first element (X[0])
   * middle → all the elements between the first and last (X[1:-1])
   * last → the last element (X[-1])
4. The program prints each part separately to show the unpacking result.

**Example:** <br>
input: 3 6 9 12 15  <br>
output: <br>
First Digit: 3 <br> Middle Digits: 6, 9, 12 <br> Last Digit: 15
