# ASLite 0.1

ASLite is a simple C++ console program that displays **ASCII art representations of the alphabet**.  
This project is designed as a learning tool to practice and support communication between people who use ASL and those who do not, while also making the experience engaging and fun.
The program serves as a learning resource to encourage practice and connection between people who use ASL and those who are learning, with an emphasis on accessibility and fun.
---

## ✨ Features

The program offers three interactive modes:

1. **Translate Mode**  
   - Enter any word and see each letter displayed in ASCII art.  
   - Type `0` to exit this mode.

2. **Training Mode**  
   - Enter a single letter (A–Z) or digit (0–9).  
   - The program prints the ASCII art for that character.  
   - Useful for practicing recognition of individual letters.

3. **Guess Game Mode**  
   - The program randomly shows a letter in ASCII art.  
   - Your task is to guess which letter it is.  
   - Type `0` to exit the game.  
   - Note: In this mode, the program hides the header (`--- Letter X ---`) so the answer is not revealed.

4. **Exit**  
   - Quit the program.

---

## 🛠️ How It Works

- **ASCII Art File**  
  The program loads characters from a file named `asl_ascii_alphabet.txt`.  
  Each letter block in the file must start with `#` followed by the letter.
  Then the ASCII art lines for that letter follow until the next `#`.

- **Core Functions**
- `loadAlphabetFromFile`: Reads the ASCII art file and stores each letter’s lines in a 2D array.
- `printWord`: Prints letters vertically, one after another.  
  - The `showHeader` parameter controls whether the header (`--- Letter X ---`) is displayed.

- **Main Menu**  
The program runs in a loop (`do { ... } while`) until the user chooses option 4 (Exit).  
Each menu option calls the appropriate function.

---
