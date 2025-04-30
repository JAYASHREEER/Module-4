# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

### PROGRAM
# Exp.No:18 - Frequency of Characters in a File

def count_char_frequency(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()

        freq = {}  # Dictionary to store character frequencies

        for char in content:
            if char in freq:
                freq[char] += 1
            else:
                freq[char] = 1

        print("Character Frequencies:")
        for char, count in freq.items():
            print(f"'{char}': {count}")

    except FileNotFoundError:
        print("The file does not exist. Please check the file name and try again.")

# Main Program
filename = input("Enter the file name: ")
count_char_frequency(filename)

### OUTPUT


### RESULT
Thus, the Python program that reads a file and counts the frequency of each character in it was implemented and successfully executed.

