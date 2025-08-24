# module-4
# Exp. No: 4a  
## Dictionary – Sorting the Keys and Values in alphabetical using Dictionary  value
###  Aim
To write a Python program to sort the keys and values of a dictionary in alphabetical order based on the values.

---

###  Algorithm

Start

Input the number of key-value pairs in the dictionary.

Create an empty dictionary.

Using a loop, take key-value pairs from the user and store them in the dictionary.

Use the sorted() function with the key parameter to sort the dictionary items by values.

Store the sorted result in a new dictionary using dictionary comprehension.

Display the original dictionary and the sorted dictionary.

Stop

---

### 🧾 Program

```
my_dict ={
    1:2,
    2:56,
    3:323,
    4:24,
    5:12,
    6:18
}
sorted_items = sorted(my_dict.items(), key=lambda item: item[1])
print("Keys and Values sorted in alphabetical order by the value")
print(sorted_items)

```
### OUTPUT

<img width="1127" height="186" alt="image" src="https://github.com/user-attachments/assets/128064a4-d910-4adf-85dd-67c28477f7e7" />

### RESULT

Thus, the Python program to sort a dictionary by its values alphabetically was successfully executed and verified.









# Exp. No: 4b  
## Exception  – write a python program for the solution of value error in exception handling and check whether the number is even or odd.

###  Aim
To write a Python program that handles ValueError using exception handling and checks whether the entered number is even or odd.
---

###  Algorithm

To write a Python program that handles ValueError using exception handling and checks whether the entered number is even or odd.

---

### 🧾 Program

```
try:
    x=input()
    b=int(x)
    if b%2==0:
        print("You entered even number")
    else:
        print("An odd number")
except ValueError:
    print("Enter only number")
```

### OUTPUT
<img width="699" height="229" alt="image" src="https://github.com/user-attachments/assets/1985ad0d-3925-4ed7-9e33-4e446c191e5d" />

### RESULT

Thus, the Python program to handle ValueError using exception handling and check whether the number is even or odd was successfully executed and verified.







# Exp. No: 4c 
## Files Modules – Write a Python program to read a file and count the frequency of each character in it
###  Aim
To write a Python program that reads a file and counts the frequency of each character present in the file.
---

###  Algorithm

Start

Open the file in read mode using the open() function.

Read the entire content of the file using read().

Create an empty dictionary to store character frequencies.

Traverse each character in the file content:

If the character is already in the dictionary → increment its count.

Otherwise → initialize its count as 1.

Close the file after reading.

Display the frequency of each character.

Stop

---

### 🧾 Program

```
from collections import defaultdict
def create_file(file_path,content):
    with open(file_path, 'w') as file:
        file.write(content)
def char_frequency(file_path):
    freq_dict=defaultdict(int)
    with open(file_path,'r') as file:
        content=file.read()
        for char in content:
            freq_dict[char]+=1
    return freq_dict
```


### OUTPUT

<img width="1126" height="332" alt="image" src="https://github.com/user-attachments/assets/b08498f8-d3f2-48fb-98a0-f0f5f5752d17" />


### RESULT

Thus, the Python program to read a file and count the frequency of each character was successfully executed and verified.






# Exp. No: 4d  
## Classes & Objects – Write Python Program to take the radius from the user and find the area of the circle using class name 'pen' and function name 'stationary'

###  Aim
To write a Python program to calculate the area of a circle by taking the radius from the user using a class (pen) and a method (stationary).
---

###  Algorithm

Start

Define a class named pen.

Inside the class, define a method called stationary which:

Accepts the radius as input from the user.

Calculates the area of the circle using the formula:

Area=π×r^2

(Use 3.1416 or math.pi for π).

Displays the calculated area.

Create an object of the pen class.

Call the stationary() method using the object.

Stop

### 🧾 Program
```
import math

class cse:
    def mech(self, radius):
        area = math.pi * radius * radius
        print(f"Area of circle: {area:.2f}")

# Take input from user
r = float(input())

# Create object and call method
obj = cse()
obj.mech(r)

```

### OUTPUT

<img width="638" height="204" alt="image" src="https://github.com/user-attachments/assets/4950b914-7322-4dbe-b7df-3470c53b311b" />

### RESULT
Thus, the Python program to find the area of a circle using a class named pen and a function named stationary was successfully executed and verified







# Exp. No: 4e 
## SEB – Place result="You can't divide with 0" to the right place so that program avoids ZeroDivisionError.

###  Aim
To write a Python program to handle ZeroDivisionError using exception handling and display an appropriate message when the user tries to divide by zero.

---

###  Algorithm

Start

Take two numbers as input from the user.

Use a try-except block to handle division:

Inside the try block:

Divide the numerator by the denominator.

Store the result in the variable result.

Inside the except block:

If the denominator is 0, assign
result = "You can't divide with 0".

Print the result.

Stop

### 🧾 Program

```
a=int(input())
b=int(input())
try:
    result=a/b
    print(result)
except ZeroDivisionError:
    print("You can't divide with 0")
     

```

### OUTPUT

<img width="622" height="268" alt="image" src="https://github.com/user-attachments/assets/6c495cbb-f41f-4de2-b84e-28347d0af38d" />


### RESULT
Thus, the Python program to handle ZeroDivisionError by placing
result = "You can't divide with 0" at the right place was successfully executed and verified.
```

```
