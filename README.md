# ALUNING_2ECEA_PA1
This repository includes Python programs that provide solutions to three (3) problems from Program Assignment 1: Introduction to Python Programming.

---

## 1. ALPHABET SOUP PROBLEM

**Problem:** Create a function that takes a string and returns a string with its letters in alphabetical order.
### Explanation
The task requires rearranging letters of a word in alphabetical order. To do this, the program:
1. Takes user input.
2. Breaks the input word into a list of characters.
3. Uses `.sort()` to arrange characters alphabetically.
4. Joins the characters back into a single string.
5. Prints the new alphabetically ordered word.

```python
#Define a function to arrange letters alphabetically
def alphabet_soup(text):
    char_list = []  # Create an empty list to hold characters
    
    #Step 1: Loop through each letter and add to list
    for letter in text:
        char_list.append(letter)

    #Step 2: Sort the list alphabetically
    char_list.sort()

    #Step 3: Rebuild the sorted list into a string
    result = ""
    for letter in char_list:
        result += letter

    return result  #Return the final alphabetically arranged word

#Step 4: Ask the user to input a word
w = input("Enter a word: ")

#Step 5: Call the function and display the result
sorted_word = alphabet_soup(w)
print(sorted_word)
```

### Explanation
* `char_list.append(letter)` stores each character in a list.
* `.sort()` rearranges the list in ascending (alphabetical) order.
* A new string is built by concatenating the sorted characters.
* The function returns and prints the alphabetically arranged word.

**Example Run:**
```
Input:  yesha  
Output:  aehsy
```

---

## 2. EMOTICON PROBLEM

**Problem:** Create a function that changes specific words into emoticons. Replace the words *smile, grin, sad,* and *mad* with their corresponding emoticons.

### Explanation
This problem demonstrates text substitution using the `.replace()` method. The program:
1. Defines a function `emotify(sentence)`.
2. Uses `.replace()` repeatedly to replace words with their emoticons.
3. Returns the updated sentence.
4. Prints the modified sentence after user input.

```python
#Define a function to replace specific words with emoticons
def emotify(sentence):
    sentence = sentence.replace("smile", ":)")   # Replace "smile" with :)
    sentence = sentence.replace("grin", ":D")    # Replace "grin" with :D
    sentence = sentence.replace("sad", ":(")     # Replace "sad" with :(
    sentence = sentence.replace("mad", ">:(")    # Replace "mad" with >:(
    
    return sentence  # Return the sentence with emoticons

#Ask the user to input a sentence
user_input = input("Enter a sentence: ")

#Call the function and print the result
result = emotify(user_input)
print(result)
```

### Explanation
* `.replace("smile", ":)")` searches for the word "smile" and substitutes it with `:)`.
* Each call updates the string further, replacing other words.
* The final sentence is returned with all substitutions applied.

**Example Run:**
```
Input:  I smile when I grin but feel sad when mad  
Output: I :) when I :D but feel :( when >:(
```

---

## 3. UNPACKING LIST PROBLEM

**Problem:** Unpack the list into three variables: `first`, `middle`, and `last`, with `middle` containing all elements between the first and last. Print all three values.

### Explanation
This problem applies list indexing and slicing. The program:
1. Prompts the user for numbers separated by spaces.
2. Splits the input string into pieces and converts them into integers.
3. Uses indexing and slicing to unpack values:
   * `X[0]` → first element.
   * `X[1:-1]` → middle elements.
   * `X[-1]` → last element.
4. Prints the unpacked values individually.

```python
#Step 1: Ask the user to enter numbers
user_input = input("Enter numbers separated by spaces: ")

#Step 2: Convert input into a list of integers
X = []
for num in user_input.split():
    X.append(int(num))  # Convert each input into an integer and add to list

#Step 3: Unpack the list into first, middle, and last
first = X[0]        # First element
middle = X[1:-1]    # All elements between first and last
last = X[-1]        # Last element

#Step 4: Print the results
print("First Digit:", first)
print("Middle Digits:", middle)
print("Last Digit:", last)
```

### Explanation
* `.split()` breaks the input string into separate numbers.
* `int(num)` ensures that numbers are stored as integers, not strings.
* Indexing and slicing (`X[0]`, `X[1:-1]`, `X[-1]`) separate the first, middle, and last.
* The unpacked values are displayed to the user.

**Example Run:**
```
Input:  3 6 9 12 15  
Output:  
First Digit: 3  
Middle Digits: [6, 9, 12]  
Last Digit: 15
```

---

## Conclusion

Program Assignment 1 provided practice with fundamental Python programming concepts:
1. The **Alphabet Soup Problem** taught how to manipulate strings, sort lists, and rebuild them into strings.
2. The **Emoticon Problem** introduced the use of `.replace()` for simple text substitution.
3. The **Unpacking List Problem** reinforced indexing and slicing of lists.

Overall, this assignment strengthens understanding of **loops, strings, lists, functions, and user input/output**, serving as the foundation for more advanced problem-solving in Python.

---

*Version 3*
