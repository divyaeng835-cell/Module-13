# Exp.No:34  
## PREFIX EVALUATION


### AIM  
To write a Python program to evaluate a user-given Prefix expression using a stack. The expression must contain operators such as Multiplication, Addition, and Subtraction.

-
### ALGORITHM

1. **Start the program.**
2. Define a set of valid operators: `*, -, +, %, /, **`.
3. Initialize an empty stack.
4. Traverse the prefix expression from **right to left**:
   - If the character is a **digit**, convert it to an integer and push it onto the stack.
   - If the character is an **operator**, pop two elements from the stack.
     - Apply the operator on the two popped operands.
     - Push the result back onto the stack.
   - If an invalid character is encountered, raise an error.
5. After traversal, the stack should contain only **one element**.
6. Return the **single element** as the evaluation result.
7. **End the program.**


### PROGRAM

```
OPERATORS=set(['*','-','+','/'])
def str_list(str):
    l=[]
    for char in str:
        l.append(char)
    l=l[::-1]
    return l;
    
def prefix_Eval(expression):
    stack=[]
    for char in expression:
        if char not in OPERATORS:
            stack.append(char)
        else:
            smallexp=""
            a=stack.pop()
            b=stack.pop()
            smallexp+=a+char+b
            stack.append(str(eval(smallexp)))
    return stack[0]

expression = input()
print(f"Prefix Expression : {expression}")
print("Evaluation result :",prefix_Eval(str_list(expression)))

```


### OUTPUT
![Screenshot 2025-05-17 112526](https://github.com/user-attachments/assets/67be0e2e-2bb8-4c90-b64b-c4e31b2ba391)

### RESULT
Thus the python program to evaluate a user-given Prefix expression using a stack has been implemented successfully
