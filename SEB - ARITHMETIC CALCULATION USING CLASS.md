# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

### AIM  
To write a Python program using a class to perform modulo and floor division operations based on user choice, using if, elif, and else statements.

### ALGORITHM
Start the program.

Define a class named SEC.

Inside the class, define:

A method setvalues(self, a, b) to assign values to a and b.

A method rem(self) to perform modulo (a % b) operation.

A method div(self) to perform floor division (a // b) operation.

Create an object of class SEC.

Take input for two numbers from the user.

Call setvalues() with the user inputs.

Use a loop to repeatedly prompt for a choice:

If the choice is 1, call rem() and display the result.

If the choice is 2, call div() and display the result.

If the choice is 0, display "Exiting!" and break the loop.

For any other input, display "Invalid choice".

End the program.

✅ Python Program
python
Copy
Edit
# Exp.No:XX - Modulo and Floor Division using Class and if..elif..

class SEC:
    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def rem(self):
        print("Result: ", self.a % self.b)

    def div(self):
        print("Result: ", self.a // self.b)

# Main program
obj = SEC()

# Getting values
a = int(input())
b = int(input())
obj.setvalues(a, b)

while True:
    choice = int(input())
    if choice == 1:
        obj.rem()
    elif choice == 2:
        obj.div()
    elif choice == 0:
        print("Exiting!")
        break
    else:
        print("Invalid choice")
This program will continuously ask the user for operations until they choose 0 to exit.

Would you like this extended to include exception handling (e.g., division by zero)?

### PROGRAM
class SEC:
    def __init__(self):
        self.a=int(input())
        self.b=int(input())
    def calculation(self):
        while True:
            c=int(input())
            if c==1:
                print("Result: ",self.a%self.b)
            elif c==2:
                print("Result: ",self.a//self.b)
            elif c==0:
                print("Exiting!")
                break
            else:
                print("Invalid choice")
c=SEC()
c.calculation()

### OUTPUT
![image](https://github.com/user-attachments/assets/ee4d07c0-122e-4984-9f39-ff016fb4479e)

### RESULT
Thus,a Python program using a class to perform modulo and floor division operations based on user choice, using if, elif, and else statements was implemented and successfully executed.
