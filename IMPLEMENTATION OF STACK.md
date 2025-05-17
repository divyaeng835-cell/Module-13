# Exp.No:31  
## IMPLEMENTATION OF STACK


### AIM 
To write a Python program to implement a stack using a list and its built-in methods (`append()`, `pop()`).
Get five items from the user and save them in stack, then pop two items from stack and display the stack before and after popped. 

### ALGORITHM

1. **Start the program.**
2. **Define a class `st`** with the following methods:
   - `push(self, num)`: Adds the number `num` to the stack.
   - `pop(self)`: Removes and returns the top element from the stack.
3. **Create a stack object `s`** using the class `st`.
4. **Input the stack size**: Take an integer input `size` to define the size of the stack.
5. **Loop through numbers from 1 to size**: Add only the odd numbers to the stack using the `push()` method.
6. **Display the elements** in the stack after the loop completes.
7. **Call `pop()`** to remove the top element from the stack and display the popped element.
8. **Display the stack again** to show the remaining elements.
9. **End the program.**

### PROGRAM

```
stack = []
for i in range(5):
    stack.append(input())
print("Stack before elements are popped")
print(stack)
print()
stack.pop()
stack.pop()
print("Stack after elements are popped:")
print(stack)

```
### OUTPUT
![Screenshot 2025-05-17 110933](https://github.com/user-attachments/assets/0f7b7bd9-d881-42b0-a358-55b9dabc6e76)

### RESULT
Thus the python program to implement a stack using a list and its built-in methods (`append()`, `pop()`) has been implemented and executed successfully.
