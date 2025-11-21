# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise:")
matrix = [[int(input(f"Element [{i+1}][{j+1}]: ")) for j in range(cols)] for i in range(rows)]

print("\nOriginal Matrix:")
for row in matrix:
    print(row)

print("\nDiagonal Elements:")
for i in range(rows):
    for j in range(cols):
        if i == j:
            print(matrix[i][j], end=" ")
        else:
            print("  ", end=" ")
    print()

```

### Output:
![446540178-5089d356-0e16-4f1f-88fb-9f6f6659e161](https://github.com/user-attachments/assets/f61721a1-3aab-4308-9599-e20ffb5eb2c0)


## Result
Thus, the program is executed successfully
