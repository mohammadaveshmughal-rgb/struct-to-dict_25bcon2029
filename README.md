STRUCT TO DICTIONARY IN PYTHON

1. Aim:
   To write a Python program to convert a data object into a dictionary.

2. Description:
   Python's dataclasses module provides a convenient way to store structured data. The asdict() function converts a dataclass object into a dictionary.

3. Requirements:

* Python 3.7 or later
* dataclasses module

4. Program:
   from dataclasses import dataclass, asdict

@dataclass
class Student:
name: str
age: int
course: str

s1 = Student("Avesh", 20, "B.Tech")

student_dict = asdict(s1)

print(student_dict)

5. Sample Output:
   {'name': 'Avesh', 'age': 20, 'course': 'B.Tech'}

6. Conclusion:
   The program successfully converts a dataclass object into a dictionary.
