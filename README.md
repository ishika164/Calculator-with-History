# 🧮 Calculator with History

A simple command-line Python project that functions as a basic calculator and saves calculation history in a `.txt` file for later use. You can also clear the history or view previous calculations.

---

## 🎯 Project Objective

To build a Python-based calculator that not only performs basic arithmetic operations but also stores, displays, and clears the calculation history using file handling.

---

## 🧠 Concepts Used

| Concept         | Why We Need It                                                                 |
|----------------|----------------------------------------------------------------------------------|
| `input()`       | To get the user’s calculation or command                                       |
| Functions       | To organize code (calculating, showing history, clearing, etc.)               |
| Conditionals    | To decide between calculation, history, clear, or exit                        |
| File Handling   | To save/load/clear history in a `.txt` file                                   |
| Loops (`while`) | To keep the program running until the user exits                              |
| Basic Math      | For calculator operations: `+`, `-`, `*`, `/`                                  |

---

## 📝 Pseudocode

1. START the program

2. DEFINE the name of the history file (e.g., "history.txt")

3. LOOP forever (while True):

   a) ASK the user to enter a calculation (like 8 + 5)
   
   OR a command (history, clear, exit)

   b) IF user enters "exit":
   
      i. PRINT a goodbye message
   
      ii. BREAK the loop

   c) IF user enters "history":
   
      i. TRY to open the history file for reading
   
      ii. IF file exists and is not empty, PRINT each line (calculation)
   
      iii. IF file doesn’t exist or is empty, PRINT "No history found"
   
      iv. CONTINUE to the next loop

   d) IF user enters "clear":
   
      i. OPEN the history file and overwrite it with nothing (empty it)
   
      ii. PRINT "History cleared"
   
      iii. CONTINUE to the next loop

   e) OTHERWISE (assume user entered a calculation):
   
      i. TRY to parse the input to get numbers and the operator
   
      - (Split input by space, e.g., "8 + 5")
   
      ii. IF input is not valid, PRINT "Invalid input" and CONTINUE
   
      iii. PERFORM the calculation using if/elif:
   
      - + → add
   
      - - → subtract
   
      - * → multiply
   
      -  / → divide (check for divide-by-zero)
   
      iv. SHOW the result to the user
   
      v. WRITE the calculation and result to the history file
   
      - e.g., "8 + 5 = 13"

5. END the program

---

## 🛠️ Tech Stack

- **Language:** Python
- **IDE:** VS Code 
- **File Handling:** `.txt` file for storing history

---

## 🌱 What I Learned

- Taking user input and parsing it
- Performing arithmetic calculations with conditions
- Using `if-elif-else` for logic flow
- Implementing infinite loops (`while True`)
- Creating and managing files using Python's built-in `open()` method
- Writing clean pseudocode and converting it to real code

---

## 🔰 Project Level

**Beginner Friendly** 💡  
This project is suitable for anyone who has just started learning Python and wants to practice basic input handling, loops, conditionals, and file operations.

---

