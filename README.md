# py.10.12.20
Assignment on List, Tuples. Dictionary

1) Create a list of strings. Write a Python program which creates another list from the first taking the first character from each word.
list=["Rohit","Sarkar","Python"]
n=len(list)
l=[]
for i in range(n):
	s=list[i]
	l.append(s[0])
print(l)
   
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

4) Write a program in Python to do slicing in all possible ways with all possible parameters, providing positive and negative values for step. Also, perform slicing from start and end both.


t=list(input("Enter List Elements separated by comma: ").split(','))
print("Specifying start and end index: ",t[2:6])
print("Without defining start index: ",t[:6])
print("Without defining end index: ",t[8:])
print("Neither is defined: ",t[:])
print("Index with negative value: ",t[-9:-6])
print("Specifying an increment: ",t[3:8:2])
print("Specifying increment only: ",t[::4])
print("Step is negative: ",t[::-3])

2) Write a Python program that prompts the user to enter an alphabet. Print all the words in the list that starts with that alphabet.
list=["Roshan","Rohit","Sarkar","singh","rahul"]
print(list)
n=len(list)
l=input("Enter the alphabet\n")
for i in range(n):
	s=list[i]
	if(l==s[0]):
		print(s)

8) Write a program that has a dictionary of your friends’ name (as keys) and their birthdays. Print the items in the dictionary in a sorted order. Prompt the user to enter a name and check if it is present in the dictionary. If the name does not exist, then ask the user to enter DOB. Add the details in the dictionary.


import operator
d={}
n=int(input("Enter No. of Friends: "))
for i in range(0,n):
  key=input("Enter Name: ")
  dob=input("YYYY-MM-DD: ")
  d[key]=dob
sorted_d = sorted(d.items(), key=operator.itemgetter(1))
print('Dictionary in ascending order by value : ',sorted_d)
name=input("Enter Name: ")
if name in d:
  print("Date of Birth: ",d[name])
else:
  print("Name not present!")
  p=input("Enter DOB as YYYY-MM-DD: ")
  d[name]=p
  print("Information Updated!")
