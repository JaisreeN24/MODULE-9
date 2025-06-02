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

      class Numbers:
          def __init__(self,N=0):
              self.N=int(input())
          def create_list(self):
              self.L=[]
              for i in range(self.N):
                  x=int(input())
                  self.L.append(x)
          def sorting(self):
              for ind in range(self.N):
                  min_index=ind
                  for j in range(ind+1,self.N):
                      if self.L[j]<self.L[min_index]:
                          min_index=j
                  (self.L[ind],self.L[min_index])=(self.L[min_index],self.L[ind])
          def print_list(self):
              for i in range(self.N):
                  print(self.L[i])
      L1=Numbers()
      L1.create_list()
      print('Before Sorting')
      L1.print_list()
      L1.sorting()
      print("After Sorting")
      L1.print_list()

## OUTPUT:
![image](https://github.com/user-attachments/assets/41512c24-de50-422e-b99b-13bc6d39f725)

## RESULT:
Thus, the program with functions to Create a list of integers, Sort it using the **Insertion Sort** algorithm, Display the sorted list is executed and verified successfully.
