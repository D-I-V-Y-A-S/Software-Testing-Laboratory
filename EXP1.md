# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE: 16-8-24                                                                         
### REGISTER NUMBER : 212221040043

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program. 
### Program:
i.)do…while: 
```
def display(): 
start=input("Enter a positive value for START: ") 
end=input("Enter a positive value for END: ") 
if start.isnumeric() and end.isnumeric(): 
while True: 
start=int(start) 
end=int(end) 
print(start,end=‘ ‘) 
if start<end: 
start+=1 
else: 
break 
else: 
print("Enter a valid positive number.") display()
```
## Output:
![exp-1-1](https://github.com/user-attachments/assets/f1212b6e-d89f-4911-81a6-923cc2dd3be2)

ii.) while…do 
```
start=input("Enter a positive value for START: ") end=input("Enter 
a positive value for END: ") 
if 
start.isnumeric() 
start=int(start) 
end=int(end) 
while start<end: 
print(start) 
start+=1 
else: 
and end.isnumeric(): 
print("Enter a valid positive number.")
```
## Output:
![exp-1-2](https://github.com/user-attachments/assets/d90072d4-a17a-4c56-87ee-684aecedc1fc)

iii.) switch 
```
def switch(): 
switcher={ 
0:"even", 
1:"odd" 
} 
n=input('Enter a value for N: ') try: 
n=int(n) 
print(switcher[n%2]) 
except ValueError: 
print("Enter a valid number.") 
switch()
```
## Output:
![exp1-3](https://github.com/user-attachments/assets/db56deb2-e070-4ad7-ba85-3fd500ff32a0)

iv.) if else 
```
def compare(): 
a=input("Enter a value for A: ") 
b=input("Enter a value for B: ") 
try: 
a=int(a) 
b=int(b) 
if a>b: 
print("A is greater than") 
elif a<b: 
print("B is greater than") 
else: 
print("A is equal to B") 
except ValueError: 
print(“Enter a valid number.”)
```
## Output:
![exp1-4](https://github.com/user-attachments/assets/60900869-df19-4e72-aec7-7869658e9d6a)

v.) for 
```
def iterate(): 
string=input("Enter a string: ") for 
i in string: 
print(ord(i),end=" ") 
iterate()
```
## Output:
![exp1-5](https://github.com/user-attachments/assets/188d7f3c-bf19-4dfc-b8b1-08aafb79b0f1)

### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


