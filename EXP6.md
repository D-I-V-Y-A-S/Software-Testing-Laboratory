# Ex.No: 6 To check whether the string is Palindrome and generate test cases.

### DATE:20-9-24                                                                         
### REGISTER NUMBER : 212221040043
### AIM: 
Write a Python program to check whether the string is Palindrome and generate test cases. 
### Algorithm:
1. Start
2. Get an input from the user by prompting 
3. Run a loop form 0 to len/2.
4. Check if the characters are the same both from the start and the end till len/2. 
5. If it is, return the result that it is a palindrome.
6. Else, return that it is not a palindrome. 
7. Stop the program.
### Program:
```
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (high + low) // 2

        # Check if x is present at mid
        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1
        else:
            return mid  # x found at index mid

    return -1  # x not found in the array

arr = [2, 3, 4, 10, 40]
x = input("Enter the element to be searched: ")

try:
    x = int(x)
    result = binary_search(arr, x)
    if result != -1:
        print("Element is present at index", str(result))
    else:
        print("Element is not present in array")
except ValueError:
    print("Enter a valid input!")
```
### Output:
![exp_6](https://github.com/user-attachments/assets/e9d14808-a309-4d8f-bea8-497df51c64d2)
### Result:
Thus, a program to check palindrome has been written and test cases have been written and verified successfully.
