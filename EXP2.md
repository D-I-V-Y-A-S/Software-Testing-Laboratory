# Ex.No: 2   Matrix Multiplication 

### DATE: 23-8-24                                                                          
### REGISTER NUMBER : 212221040043

### AIM: 
Write a python program for matrix multiplication and inspect for failures.
 
### Algorithm:
Algorithm:
1. Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program.
### Program:
```
r1, c1 = input("Enter row and column count in matrix 1: ").split()
r2, c2 = input("Enter row and column count in matrix 2: ").split()

if r1.isnumeric() and c1.isnumeric() and r2.isnumeric() and c2.isnumeric():
    r1 = int(r1)
    c1 = int(c1)
    r2 = int(r2)
    c2 = int(c2)
    
    if c1 != r2:
        print("Matrix multiplication not possible")
    elif max(r1, c1, r2, c2) > 20 or min(r1, c1, r2, c2) == 0:
        print("Matrix multiplication not possible")
    else:
        # Input for matrix 1
        matrix1 = []
        print("Enter elements for matrix 1:")
        for i in range(r1):
            row = [int(input(f"Matrix1[{i}][{j}]: ")) for j in range(c1)]
            matrix1.append(row)

        # Input for matrix 2
        matrix2 = []
        print("Enter elements for matrix 2:")
        for i in range(r2):
            row = [int(input(f"Matrix2[{i}][{j}]: ")) for j in range(c2)]
            matrix2.append(row)

        # Initializing the result matrix with zeros
        result = [[0 for _ in range(c2)] for _ in range(r1)]

        # Matrix multiplication logic
        for i in range(r1):
            for j in range(c2):
                for k in range(c1):  # or `range(r2)` as c1 == r2
                    result[i][j] += matrix1[i][k] * matrix2[k][j]

        # Display the result
        print("Resultant matrix:")
        for i in range(r1):
            for j in range(c2):
                print(result[i][j], end=" ")
            print()

else:
    print("Enter valid numeric values")
```
### Output:
![exp-2](https://github.com/user-attachments/assets/b1d5e1cf-bece-4d1c-84a4-72efeee81d04)

### Result:
Thus, the python program for matrix multiplication is implemented and the causes for its failure is introspected successfully.

