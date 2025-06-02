# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
    def create_matrix(rows, cols):
        return [[int(input(f"Enter element [{i}][{j}]: ")) for j in range(cols)] for i in range(rows)]
    
    def transpose_matrix(matrix):
        return [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
    
    r = int(input())
    c = int(input())
    
    matrix = create_matrix(r, c)
    
    transposed = transpose_matrix(matrix)
    
    
    print("\nMatrix:")
    for row in matrix:
        print(row)
    
    print("\nMatrix:")
    for row in transposed:
        print(row)
## OUTPUT:
![image](https://github.com/user-attachments/assets/2c7859a5-e56d-450e-9c79-5fe2ba6b85c4)

## RESULT:
Thus, the program to compute the **transpose** of a matrix using **list comprehension** is executed and verified successfully.

