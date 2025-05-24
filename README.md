# Speller – CS50 Problem Set 5

This project implements a **spell checker** in C. It reads in a dictionary, then checks each word of a given text file to identify potential misspellings.

## 📌 Description

The program loads a large dictionary file (e.g., `dictionaries/large`) into a **hash table**, then scans an input text file to compare each word against the dictionary.

It measures and reports:
- Number of misspelled words
- Number of words in dictionary
- Number of words in text
- Time taken to load, check, and unload

## 💻 How to Run

1. **Compile the program:**
   ```markdown
   make speller
2. **Run with a dictionary and a text file:**
   ```pgsql
   ./speller dictionaries/large texts/lalaland.txt
3. **Sample Output:**
   ```markdown
   MISSPELLED WORDS
    spagetti
    beutiful
    laraland
    
    WORDS MISSPELLED: 3
    WORDS IN DICTIONARY: 143091
    WORDS IN TEXT: 465
    TIME IN load: 0.03
    TIME IN check: 0.02
    TIME IN size: 0.00
    TIME IN unload: 0.01
    TIME IN TOTAL: 0.06

## 📎 Files

- `dictionary.c` – contains logic for loading, checking, and unloading dictionary
- `speller.c` – handles the main flow of the spell-checker
- `Makefile` – build instructions
- `dictionary.h` – function declarations

## 🧠 Concepts Practiced

- Hash tables
- Pointers and memory management
- File I/O in C
- Performance benchmarking
- Handling large data structures

---

This project was completed as part of [CS50x](https://cs50.harvard.edu/x) to explore data structures, memory, and performance in C.
