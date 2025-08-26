# Experiment-2
Write a program in Python language for Matrix multiplication fails. Introspect the causes for its failure and write down the possible reasons for its failure. 
## Aim
Write a python program for matrix multiplication and inspect for failures. 

## Algorithm
1.	Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program. 

## Program:
```python
r1=int(input("Enter number of rows in Matrix A:"))
c1=int(input("Enter number of colums in Matrix A:"))
r2=int(input("Enter number of rows in Matrix B:"))
c2=int(input("Enter number of colums in Matrix B:"))

if c1!=r2:
    print("Multiplication is not possible")
else:
    print("Enter elements of matrix A:")
    A=[[int(input(f"A[{i}][{j}]: ")) for j in range(c1)] for i in range(r1)]
    print("Enter elements of matrix B:")
    B=[[int(input(f"B[{i}][{j}]: ")) for j in range(c2)] for i in range(r2)]

    result=[[9 for _ in range(c2)] for _ in range(r1)]

    for i in range(r1):
        for j in range(c2):
            for k in range(c1):
                result[i][j]+=A[i][k]*B[k][j]

    print("\nResultant Matrix:")
    for row in result:
        print(row)
```

## Output:
<img width="1480" height="548" alt="image" src="https://github.com/user-attachments/assets/f8eeec84-70c2-40b9-9b45-6621d610c92c" />

<img width="1460" height="161" alt="image" src="https://github.com/user-attachments/assets/0fae2fde-3fab-4127-86dc-e41451b6b908" />


## Result:
Thus, the multiplication of matrices has been executed successfully.
