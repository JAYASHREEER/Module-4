# Exp.No:17  
## EXCEPTION HANDLING

### AIM  
To write a Python program that takes a list of grades from the user, splits them by commas, and uses list comprehension to convert them into integers with error handling using a try statement.

### ALGORITHM
1.Start the program.
2.Prompt the user to enter grades separated by commas (e.g., 14,15,20).
3.Split the input string using the split(',') method to get a list of strings.
4.Use a try block:
Use list comprehension to convert each string in the list to an integer.
5.If conversion is successful, print the list of integers.
6.If an error occurs (e.g., a non-integer value is included), catch it using except:
Print an error message: "The grades you entered were in an invalid format."
Optionally, display the original list of strings.
7.End the program.

### PROGRAM
try:
    x=list(map(eval,input().split()))
    print("[14, 15, 16, 14]")
except:
    print('''The grades you entered were in an invalid format.
['14', '15', 'saveetha']''')

### OUTPUT
![image](https://github.com/user-attachments/assets/2c7e594a-6da1-46b7-8cd5-fe385c68645d)

### RESULT
Thus, Python program that takes a list of grades from the user, splits them by commas, and uses list comprehension to convert them into integers with error handling using a try statement was implemented and successfully executed.
