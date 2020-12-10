# py.10.12.20
Assignment on List, Tuples. Dictionary

1) Create a list of strings. Write a Python program which creates another list from the first taking the first character from each word.
l1=['rohit','sarkar','python','virat']
l2=[]
for char in l1:
    l2=char[0]
    print(list(l2))
   
3) Write a Python program to implement user-defines stack
my_first_stack = []
my_first_stack.append('Rohit')
my_first_stack.append('sarkar')
my_first_stack.append('Python')
print(my_first_stack.pop())
print(my_first_stack)
print(my_first_stack.pop())
print(my_first_stack)
print(my_first_stack.pop())
print(my_first_stack)


5) Write a Python program to count the elements in a list until an element is a tuple.

num = [10,20,30,(10,20),40]
ctr = 0
for n in num:
    if isinstance(n, tuple):
        break
    ctr += 1
print(ctr)

6) Write a Python program that displays information about an employee. Use nested dictionary to do this task.
d1={'Name':'abc',
    'DOB':'10.12.1983',
    'add':'xxx',
    'post':{'developer':{1:'python',2:'c++',3:'java'}}}

print(d1)

7) Create a dictionary of products purchased and their MRPs. Calculate the bill and display to the customer.

d1={'rice':50,'potato':80,'drinks':100,'chips':20}
sum=0
for value in d1:
    sum=sum+d1[value]
print(d1)
print("bill to be paid",sum)
