# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
student_marks = {
    "Alice": [85, 90, 78, 92, 88],
    "Bob": [80, 70, 75, 85, 90],
    "Charlie": [95, 88, 92, 91, 89],
    "David": [70, 65, 80, 75, 60]
}

total_marks = {}

for student, marks in student_marks.items():
    total = sum(marks)
    total_marks[student] = total

topper = max(total_marks, key=total_marks.get)

print("Total Marks of Students:", total_marks)
print("Topper:", topper, "with", total_marks[topper], "marks")
```


## OUTPUT:
![446537679-e10234cd-f3bd-4ad5-81ba-fb0d5c3aca6e](https://github.com/user-attachments/assets/011841fe-58a5-421c-8730-beaec95d76d5)

## RESULT:
Thus, the program is executed successfully
# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
student_marks = {
    "Alice": [85, 90, 78, 92, 88],
    "Bob": [80, 70, 75, 85, 90],
    "Charlie": [95, 88, 92, 91, 89],
    "David": [70, 65, 80, 75, 60]
}

total_marks = {}

for student, marks in student_marks.items():
    total = sum(marks)
    total_marks[student] = total

topper = max(total_marks, key=total_marks.get)

print("Total Marks of Students:", total_marks)
print("Topper:", topper, "with", total_marks[topper], "marks")
```


## OUTPUT:
![446537679-e10234cd-f3bd-4ad5-81ba-fb0d5c3aca6e](https://github.com/user-attachments/assets/011841fe-58a5-421c-8730-beaec95d76d5)

## RESULT:
Thus, the program is executed successfully
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
# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
def create_matrix(r, c):
    print(f"Enter elements for a {r}x{c} matrix:")
    return [[int(input(f"Element [{i+1}][{j+1}]: ")) for j in range(c)] for i in range(r)]

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

print("\nMatrix A:")
A = create_matrix(r, c)

print("\nMatrix B:")
B = create_matrix(r, c)

C = [[A[i][j] - B[i][j] for j in range(c)] for i in range(r)]

print("\nResultant Matrix (A - B):")
for row in C:
    print(row)
```

## OUTPUT:

![446541783-4d1f77c6-9a40-4cc1-8918-88d9d3566b71](https://github.com/user-attachments/assets/297d9941-352e-48d0-a4d8-7d67c5b930ee)

## RESULT:

Thus, the program is executed successfully
# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:
```
class InsertionSorter:
    def __init__(self):
        self.nums = []

    def create_list(self):
        n = int(input("Enter number of elements: "))
        self.nums = [int(input(f"Enter element {i+1}: ")) for i in range(n)]

    def insertion_sort(self):
        for i in range(1, len(self.nums)):
            key = self.nums[i]
            j = i - 1
            while j >= 0 and self.nums[j] > key:
                self.nums[j + 1] = self.nums[j]
                j -= 1
            self.nums[j + 1] = key

    def print_list(self):
        print("Sorted List:", self.nums)

sorter = InsertionSorter()
sorter.create_list()
sorter.insertion_sort()
sorter.print_list()

```
## OUTPUT:
![446542342-9cfaba91-dd80-432c-b5ab-4c61ee0a1458](https://github.com/user-attachments/assets/ca702729-c394-402c-bff1-8e62c4392ef2)


## RESULT:
Thus, the program is executed successfully
