# Exp.No:19  
## CLASS AND OBJECTS - AREA OF CIRCLE

### AIM  
To write a Python program to take the radius from the user and find the area of a circle using a class and a function.

### ALGORITHM
1.Start the program.
2.Define a class (e.g., Circle).
3.Inside the class, define a function (e.g., calculate_area) to compute the area using the formula:Area=𝜋×radius2
4.Prompt the user to enter the radius.
5.Create an object of the class.
6.Call the function using the object to compute and display the area.
7.End the program.

### PROGRAM
import math
class cse:
    def __init__(self,a):
        self.a=a
    def mech(self):
        m=math.pi*self.a*self.a
        print("Area of circle:",round(m,2))

a=int(input())
n=cse(a)
n.mech()

### OUTPUT
![image](https://github.com/user-attachments/assets/db51f155-e817-4d71-9507-2f104eec7e6c)

### RESULT
Thus, Python program to take the radius from the user and find the area of a circle using a class and a function was implemented and successfully executed.



