**1.	Practical :  Write a program to create variables of different types and perform basic arithmetic operations**
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
            print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)

**2.	Practical : Write a program to find the factorial of a number.**
n = int(input("Enter a number: "))
fact = 1
for i in range(1, n + 1):
fact = fact * i
print("Factorial is:", fact)

**3.	Practical : Write a program to check whether a number is even or odd.**
n = int(input("Enter a number: "))
if n % 2 == 0:
print("Even number")
else:
 print("Odd number")

**4.	Practical : Write a program to perform addition of two matrices.**
A = [[1, 2], [3, 4]]
B = [[5, 6], [7, 8]]
C = [[0, 0], [0, 0]]
for i in range(2):
 for j in range(2):
 C[i][j] = A[i][j] + B[i][j]
print("Matrix Addition:", C)

**5.	Practical : Write a program to perform multiplication of two matrices.**
 A = [[1, 2], [3, 4]]
B = [[5, 6], [7, 8]]
C = [[0, 0], [0, 0]]
for i in range(2):
for j in range(2):
for k in range(2):
            C[i][j] += A[i][k] * B[k][j]
             print("Matrix Multiplication:", C)


**6.	Practical: Write a program to check whether a given number is positive, negative, or zero using if–elif–else.**
n = int(input("Enter a number: "))
if n > 0:
print("Positive")
elif n < 0:
print("Negative")
else:
print("Zero")

**7.	Practical : Write a program to find the largest of three numbers.**
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
print("Largest number is:", max(a, b, c))

**8.	Practical: Write a program to print all even numbers from 1 to 50 using a for loop.**
for i in range(1, 51):
if i % 2 == 0:
print(i)

**9.	Practical: Write a program to check palindrome and anagram strings.**
s1 = input("Enter first string: ")
s2 = input("Enter second string: ")
# Palindrome
if s1 == s1[::-1]:
 print("Palindrome")
else:
 print("Not Palindrome")
# Anagram
if sorted(s1) == sorted(s2):
print("Anagram")
else:
            print("Not Anagram")

**10.	Practical: Write a program to calculate factorial of a number using recursion.**
def fact(n):
if n == 1:
return 1
else:
return n * fact(n - 1)
n = int(input("Enter number: "))
print("Factorial:", fact(n))

**11.	Practical: Write a program to find the square of a number using a lambda function.**
square = lambda x: x * x
n = int(input("Enter number: "))
print("Square:", square(n))

**12.	Practical: Write a program to find Spy Number, Harshad Number, and Duck Number**
n = input("Enter number: ")
num = int(n)
# Spy Number
sum_d = 0
prod = 1
for i in n:
sum_d += int(i)
prod *= int(i)
print("Spy Number:", sum_d == prod)
# Harshad Number
print("Harshad Number:", num % sum_d == 0)
# Duck Number
print("Duck Number:", '0' in n)

**13.	Practical: Write a program to create a list of 10 numbers and perform indexing, slicing, and update operations.**
lst = [1,2,3,4,5,6,7,8,9,10]
print("Indexing:", lst[2])
print("Slicing:", lst[2:6])
lst[0] = 100
print("Updated list:", lst)

**14.	Practical : a) Write a program to create a tuple and demonstrate tuple functions.**
         t = (10, 20, 30, 20, 40)
        print("Tuple:", t)
        print("Length of tuple:", len(t))
        print("Count of 20:", t.count(20))
         print("Index of 30:", t.index(30))

**b)Write a program to find the maximum and minimum elements in a tuple.**
t = (10, 20, 20, 30)
print("Max:", max(t))
print("Min:", min(t))
print("Count of 20:", t.count(20))
print("Length:", len(t))
**c)	Write a program to convert a list of tuples into a dictionary.**
           lst = [(1, 'Apple'), (2, 'Banana'), (3, 'Mango')] 
           d = dict(lst) 
            print("Dictionary:", d)

   **d)Write a program to count repeated elements in a tuple.**
       t = (1, 2, 3, 2, 4, 1, 2)
      print("Repeated elements count:")
      for i in set(t):
     print(i, ":", t.count(i))

**e)Write a program to find the length of each element in a tuple of strings.**
         t = ("Python", "Java", "C", "Programming")
        for i in t:
        print(i, "length is", len(i)) 
      f)Write a program to merge two tuples without duplicates.
t1 = (1, 2, 3, 4)
t2 = (3, 4, 5, 6) 
                  merged = tuple(set(t1 + t2))
print("Merged tuple without duplicates:", merged)

**15.	Practical : Write a program to create a dictionary, add key–value pairs, and access values.**
d = {}
d['name'] = input("Enter name: ")
d['age'] = int(input("Enter age: "))

print(d)
print("Name:", d['name'])

**Practical : 16. (A)Write a program to demonstrate dictionary methods: keys(), values(), items(), update(), pop().**
# dictionary
student = {
 "roll_no": 46,
 "name": "Vishal",
 "course": "MCA",
 "age": 20
}
print("Keys:", student.keys())
print("Values:", student.values())
print("Items:", student.items())
student.update({"age": 21, "city": "Pune"})
print("After update:", student)
student.pop("course")
print("After pop:", student)
**#(a) Program to count word frequency in a given sentence**
sentence = "python is easy and python is powerful"
words = sentence.split()
freq = {}
for word in words:
freq[word] = freq.get(word, 0) + 1
print("Word Frequency:")
print(freq)
**#(b) Program to convert a dictionary into a list of tuples**
student = {
"roll_no": 101,
"name": "Rahul",
 "course": "BCA",
 "age": 20
}
tuple_list = list(student.items())
print("List of Tuples:")
print(tuple_list)

**Practical 17:  (a) Program to create a set and perform union, intersection, and difference**
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7}
print("Set A:", A)
print("Set B:", B)
print("Union:", A | B)
print("Intersection:", A & B)
print("Difference (A - B):", A - B)
**#17 (b) Program to find missing elements in a given range using sets**
numbers = {1, 2, 4, 6, 7}
full_range = set(range(1, 8))
missing = full_range - numbers
print("Missing elements:", missing)
**#17 (c) Program to find common elements in three sets**
A = {1, 2, 3, 4}
B = {2, 3, 5}
C = {2, 3, 6}
common = A & B & C
print("Common elements:", common)
**#17 (d) Program to convert a set into a sorted list**
s = {8, 3, 1, 5, 2}
sorted_list = sorted(s)
print("Sorted List:", sorted_list)

**Practical 18:  .Program to generate squares of numbers from 1 to N using list comprehension**
N = 10   
squares = [i * i for i in range(1, N + 1)]
print("Squares from 1 to", N)
print(squares)

**Practical : #19.Write a program to count vowels, consonants, digits, and spaces in a string.**
s = "Python 3 Programming"
vowels = consonants = digits = spaces = 0
for ch in s:
if ch.lower() in "aeiou":
vowels += 1
elif ch.isalpha():
consonants += 1
elif ch.isdigit():
digits += 1
elif ch == " ":
spaces += 1
print("Vowels:", vowels)
print("Consonants:", consonants)
print("Digits:", digits)
print("Spaces:", spaces)
# Write a program to find the longest word in a string.
s = "Python is very easy language"
words = s.split()
longest = max(words, key=len)
print("Longest word:", longest)
# Write a program to reverse words in a given sentence.
s = "Python is easy"
words = s.split()
reversed_sentence = " ".join(words[::-1])
print("Reversed sentence:", reversed_sentence)
# Write a program to replace all spaces with hyphens.
s = "Python is easy to learn"
result = s.replace(" ", "-")
print("After replacing spaces:", result)
# Write a program to count uppercase and lowercase letters.
s = "Python Programming"
upper = lower = 0
for ch in s:
if ch.isupper():
upper += 1
elif ch.islower():
lower += 1
print("Uppercase letters:", upper)
print("Lowercase letters:", lower)
# Write a program to check whether two strings are anagrams.
s1 = "listen"
s2 = "silent"
if sorted(s1) == sorted(s2):
print("Strings are Anagrams")
else:
print("Strings are Not Anagrams")

**Practical : #20.Write a program to demonstrate list methods: append(), insert(), remove(), pop(), reverse(), sort().**
lst = [10, 30, 20, 40]
print("Original List:", lst)
lst.append(50)
print("After append:", lst)
lst.insert(1, 15)
print("After insert:", lst)
lst.remove(30)
print("After remove:", lst)
lst.pop()
print("After pop:", lst)
lst.reverse()
print("After reverse:", lst)
lst.sort()
print("After sort:", lst)
# W rite a program to find the frequency of each element in a list.
lst = [1, 2, 2, 3, 1, 4, 2]
print("Element Frequency:")
for i in set(lst):
print(i, ":", lst.count(i))
**#Write a program to merge two lists and sort the result.**
list1 = [5, 1, 3]
list2 = [4, 2, 6]
merged = list1 + list2
merged.sort()
print("Merged and Sorted List:", merged)
**#Write a program to split a list into even and odd lists.**
lst = [1, 2, 3, 4, 5, 6, 7, 8]
even = []
odd = []
for i in lst:
if i % 2 == 0:
even.append(i)
else:
odd.append(i)
print("Even List:", even)
print("Odd List:", odd)
**#Write a program to find common elements between two lists.**
list1 = [1, 2, 3, 4, 5]
list2 = [4, 5, 6, 7]
common = list(set(list1) & set(list2))
print("Common Elements:", common)
**
**Practical : #21. Write a program to create a text file, write data into it, and read data line by line.****
# Writing to file
with open("s.txt", "w") as file:
file.write("Line 1: Python\n")
file.write("Line 2: File handling\n")
file.write("Line 3: Jupyter Notebook\n")
# Reading from file
with open("s.txt", "r") as file:
print("File content:")
for line in file:
print(line.strip())

**Practical : #22.Write a program to append new data to an existing file.**
# Append data safely using with
with open("s.txt", "a") as file:
 file.write("Another appended line\n")
# Read file
with open("s.txt", "r") as file:
for line in file:
print(line.strip())

**Practical: #23.Write a program to read and write CSV files using the csv module.**
import csv
# write to csv
with open("employees.csv", "w", newline="") as file:
 fieldnames = ["ID", "Name", "Salary"]
 writer = csv.DictWriter(file, fieldnames=fieldnames)
 # Write header
 writer.writeheader()
 # User input
 n = int(input("Enter number of employees: "))
 for i in range(n):
 print(f"\nEnter details of employee {i+1}")
 emp_id = input("Enter ID: ")
 name = input("Enter Name: ")
  salary = input("Enter Salary: ")
  writer.writerow({
   "ID": emp_id,
   "Name": name,
    "Salary": salary
     })print("\nData written to CSV successfully")
# read from csv
with open("employees.csv", "r") as file:
 reader = csv.DictReader(file)
 print("\nEmployee Details from CSV File:")
  for row in reader:
print(row)

**Practical: #24.Write a program to read and write JSON files using the json module.**
import json
# write to json
data = {
    "employees": [
        {"ID": 1, "Name": "Anita", "Salary": 50000},
        {"ID": 2, "Name": "Rohit", "Salary": 60000}
    ]
}
with open("employees.json", "w") as file:
    json.dump(data, file, indent=4)
print("Data written to JSON file successfully")

# read from json
with open("employees.json", "r") as file:
    json_data = json.load(file)
print("\nReading data from JSON file:")
for emp in json_data["employees"]:
    print(emp)
**Pratical: #25.Write a program to demonstrate try, except, else, and finally blocks.**
try:
    a = int(input("Enter number1: "))
    b = int(input("Enter number2: "))
    result = a / b
except ZeroDivisionError:
    print("Cannot divide by zero")
except ValueError:
    print("Invalid input")
else:
    print("Result:", result)
finally:
    print("Execution completed")

**Practical: #26.	Write a program to create a simple Python class demonstrating OOP concepts.**
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)
s1 = Student("Vishal", 21)
s1.display()

**Practical: #27.Write a program to demonstrate inheritance and polymorphism using Python classes.**
class Animal:
    def sound(self):
        print("Animal makes sound")
class Dog(Animal):
    def sound(self):
        print("Dog barks")
class Cat(Animal):
    def sound(self):
        print("Cat meows")
animals = [Dog(), Cat()]
for a in animals:
    a.sound()

**Practical: #28.Write a program to create NumPy arrays and perform basic operations (addition, multiplication, mean, sum).**
import numpy as np
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6]
print("Addition:", arr1 + arr2)
print("Multiplication:", arr1 * arr2)
print("Mean:", np.mean(arr1))
print("Sum:", np.sum(arr1))

**Practical: #29.Write a program to create a Pandas DataFrame, read a CSV file, perform data cleaning, and basic operations (head, tail, describe).**
import pandas as pd
# Create DataFrame
data = {"Name": ["Rahul", "Amit", None], "Age": [21, 22, None]}
df = pd.DataFrame(data)
# Save CSV
df.to_csv("data.csv", index=False)
# Read CSV
df = pd.read_csv("data.csv")
# Data Cleaning
df = df.dropna()
print(df.head())
print(df.tail())
print(df.describe())

**Pratical: #30.Write a program to create different plots using Matplotlib: line chart, bar chart, scatter plot, and pie chart**
import matplotlib.pyplot as plt
x = [1, 2, 3]
y = [4, 5, 6]
# Line chart
plt.plot(x, y)
plt.title("Line Chart")
plt.show()
# Bar chart
plt.bar(x, y)
plt.title("Bar Chart")
plt.show()
# Scatter plot
plt.scatter(x, y)
plt.title("Scatter Plot")
plt.show()
# Pie chart
plt.pie(y, labels=x, autopct='%1.1f%%')
plt.title("Pie Chart")
plt.show()

**Practical: #31.Write a program to connect to a SQLite/MySQL database and perform CRUD operations on student records.**
import sqlite3
# Use completely new name
conn = sqlite3.connect("fresh_student_123.db")
cursor = conn.cursor()
# Create table
cursor.execute("""
CREATE TABLE students (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT
)
""")
# Insert data
cursor.execute("INSERT INTO students (name) VALUES (?)", ("Rahul",))
cursor.execute("INSERT INTO students (name) VALUES (?)", ("vishal",))
# Fetch data
cursor.execute("SELECT * FROM students")
print(cursor.fetchall())
conn.commit()
conn.close()

**Practical: #32.Write a program to design an employee payroll management system using Python and a database to calculate salary and generate salary slips.**
import sqlite3
conn = sqlite3.connect("payroll.db")
cursor = conn.cursor()
cursor.execute("""
CREATE TABLE IF NOT EXISTS employee(
id INTEGER, name TEXT, salary REAL
)
""")
# Insert
cursor.execute("INSERT INTO employee VALUES (1, 'Rahul', 50000)")
cursor.execute("INSERT INTO employee VALUES (2, 'vishal', 510000)")
cursor.execute("INSERT INTO employee VALUES (3, 'dev', 50000)")
# Fetch and generate slip
cursor.execute("SELECT * FROM employee")
for emp in cursor.fetchall():
    print("----- Salary Slip -----")
    print("ID:", emp[0])
    print("Name:", emp[1])                                             
    print("Salary:", emp[2])
conn.commit()
conn.close()

                               




