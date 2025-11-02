# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
```
import math
class area:
    def slot(self,r):
        a=math.pi*r*r
        print(f"Area of circle: {a:.2f}")
r=int(input())
s=area()
s.slot(r)
```

## Output
<img width="943" height="243" alt="image" src="https://github.com/user-attachments/assets/07f9dbf5-bef7-4a7a-a6c9-b6605165606d" />


## Result
Thus the program has been successfully executed

## To find sum of all items in a Dictionary 

## 🎯 Aim
To write a Python program to find the sum of all items (values) in a dictionary.

## 🧠 Algorithm
1.Start

2.Create a dictionary with key–value pairs.
Example: d = {'a':100, 'b':200, 'c':300}

3.Extract all the values from the dictionary using d.values().

4.Find the sum of all the values using the sum() function.
Example: result = sum(d.values())

5.Display the result using the print() statement.

6.Stop
## 🧾 Program
```
d={'a':100,'b':200,'c':300}
result=sum(d.values())
print("Sum :",result)
```

## Output
<img width="751" height="162" alt="image" src="https://github.com/user-attachments/assets/1e2fd08d-b205-40af-a05c-377f19a7e290" />


## Result
The program successfully computes the sum of all dictionary values.

# 🔤 To display the keys alphabetically using dictionary



## 🎯 Aim

To write a Python program to display all the keys of a dictionary in sorted order.

## 🧠 Algorithm

1.Start

2.Create a dictionary with key–value pairs.

Example: d = {1:'a', 2:'b', 3:'c', 4:'d', 5:'e', 6:'f'}

3.Use the sorted() function to get all keys in ascending order.

4.Use a for loop to iterate through the sorted keys.

5.Print each key using the print() statement.

6.Stop

## 🧪Program
```
d={1:'a',2:'b',3:'c',4:'d',5:'e',6:'f'}
print("Keys are")
for key in sorted(d):
    print(key,end=" ")
```

## Sample Output
<img width="472" height="197" alt="image" src="https://github.com/user-attachments/assets/1e4da0b4-eef2-4c1b-9756-8707f690b2e6" />

## Result
The program successfully displays all the keys of the dictionary in sorted order.


# Exception Handling in Python: Raise an exception

## 🎯 Aim
To write a Python program that takes the user's age as input and calculates the year of birth, handling invalid input using exception handling.

## 🧠 Algorithm
1.Start the program.

2.Read the user's age using input() and convert it to an integer.

3.Print the entered age.

4.Use a try block to handle errors:

5.If the age is less than 0, display a message "Input Correct age."

6.Otherwise, calculate the year of birth using year = 2022 - age.

7.Print the calculated year of birth.

8.Use the except block to catch and print any errors.

9.Stop the program.

## 🧾 Program
```
age=int(input())
print("Age is:")
print(age)
try:
    if(age<0):
        print("Input Correct age.")
    else:
        year=2022-age
        print("Year of Birth is:")
        print(year)
except:
    print(e)
```

## Output
<img width="870" height="355" alt="image" src="https://github.com/user-attachments/assets/c1e40985-6862-4c26-a08c-73b70d72db10" />

## Result
The program successfully displays the user's age and calculates their year of birth if the input is valid.
If the input age is negative, it prompts the user to enter the correct age.

# File Handling in Python: To find longest word in the file

## 🎯 Aim
To write a Python program to create a text file and find the longest word present in that file.

## 🧠 Algorithm
1.Start the program.

2.Define a function create_file(file_path, content) that:

3.Opens a file in write mode.

4.Writes the given content to the file.

5.Closes the file automatically using the with statement.

6.Define another function find_longest_word(file_path) that:

* Opens the file in read mode.

* Initializes an empty string long to store the longest word.

* Reads the file line by line.

* Splits each line into words using split().

* Compares the length of each word with the current longest word.

* Updates long if a longer word is found.

* Returns the longest word.

7.Call both functions — first to create the file, then to find the longest word.

8.Stop the program.

## 🧾 Program
```
def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

# Function to find the longest word in a file
def find_longest_word(file_path):
    with open(file_path,'r')as file:
        long=""
        for line in file:
            for words in line.split():
                if len(words)>len(long):
                    long=words
    return long

```

## Output
<img width="1054" height="332" alt="image" src="https://github.com/user-attachments/assets/78a240bd-7d35-4c2f-b87e-2d14a571152b" />


## Result
The program successfully creates a text file with user-provided content and displays the longest word in that file.
