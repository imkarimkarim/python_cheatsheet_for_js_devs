# Python Cheatsheet for JS Developers

i will add to this as i go....
contributions are welcomed 🌻

## Table of Contents

* [virtualenv](#virtualenv-(highly-recommended))
* [General](#General)
* [Data Types](#Data-Types)
* [Loops](#Loops)
  * [forEach](#forEach)
* [Null Checking](#Null-Checking)
* [OOP](#OOP)
* [User Input](#User-Input)
* [Try Catch](#Try-Catch)
* [Django](#Django)

## virtualenv (highly recommended)

python -m venv env_name  
source env_name/bin/activate

---

`JS` --> ```Python```

---

## General

`console.log("")` --> ```print("")```

`x.toString() / String(x)` --> ```str(x)```

`if(true){}` --> ```if True:```

`null` --> ```None```

`true` --> ```True```

`false` --> ```False```

`x.length` --> ```len(x)```

```py
# python dictionary(js object)
student = {
    'name': 'John Doe',
    'age': 20,
    'major': 'Computer Science',
    'gpa': 3.8,
}
name = student["name"]

# python ternary:
def even_or_odd(number):
    return "Even" if number % 2 == 0 else "Odd"
```
find a character index in string / find a value in array
```python
index = string.find(char)
```

## Data Types

```python
Python provides several built-in data types that allow you to store and manipulate data. Here are some of the most commonly used data types with examples:

1. Integer (int): An integer is a whole number, both positive and negative, without a decimal point.
   Example:
   ```python
   x = 10
   y = -5
   print(type(x))  # Output: <class 'int'>
   print(type(y))  # Output: <class 'int'>
   ```

2. Float: A float is a floating-point number, which is a number with a decimal point.
   Example:
   ```python
   x = 3.14
   y = -2.5
   print(type(x))  # Output: <class 'float'>
   print(type(y))  # Output: <class 'float'>
   ```

3. String (str): A string is a sequence of characters enclosed in single or double quotes.
   Example:
   ```python
   name = "John"
   age = '30'
   print(type(name))  # Output: <class 'str'>
   print(type(age))  # Output: <class 'str'>
   ```

4. Boolean (bool): A boolean represents one of two values: True or False.
   Example:
   ```python
   x = True
   y = False
   print(type(x))  # Output: <class 'bool'>
   print(type(y))  # Output: <class 'bool'>
   ```

5. List: A list is an ordered collection of items enclosed in square brackets.
   Example:
   ```python
   fruits = ['apple', 'banana', 'orange']
   numbers = [1, 2, 3, 4, 5]
   print(type(fruits))  # Output: <class 'list'>
   print(type(numbers))  # Output: <class 'list'>
   ```

6. Tuple: A tuple is an ordered, immutable collection of items enclosed in parentheses.
   Example:
   ```python
   coordinates = (1, 2, 3)
   colors = ('red', 'green', 'blue')
   print(type(coordinates))  # Output: <class 'tuple'>
   print(type(colors))  # Output: <class 'tuple'>
   ```

7. Set: A set is an unordered collection of unique items enclosed in curly braces.
   Example:
   ```python
   unique_fruits = {'apple', 'banana', 'orange'}
   prime_numbers = {2, 3, 5, 7}
   print(type(unique_fruits))  # Output: <class 'set'>
   print(type(prime_numbers))  # Output: <class 'set'>
   ```

8. Dictionary (dict): A dictionary is an unordered collection of key-value pairs enclosed in curly braces.
   Example:
   ```python
   person = {'name': 'John', 'age': 30, 'city': 'New York'}
   countries = {'USA': 'Washington DC', 'Canada': 'Ottawa', 'Mexico': 'Mexico City'}
   print(type(person))  # Output: <class 'dict'>
   print(type(countries))  # Output: <class 'dict'>
   ```

These are the basic data types in Python. You can perform various operations on these data types, such as concatenation, indexing, slicing, and more.
```


## Loops

### forEach

JS:

```js
items.forEach(item => {
    console.log(item)
})
```

Py:

```python
for item in items:
 print(item)
```

## Null Checking

`variable === null` --> ```if variable is None```

`variable !== null` --> ```if variable is not None```

## OOP

JS:

```js
class ClassMates{
 constructor(name,age){
     this.name=name;
       this.age=age;
    }
   displayInfo(){
     return this.name + "is " + this.age + " years old!";
    }
}

let classmate = new ClassMates("Mike Will",15);
classmate.displayInfo();  // result: Mike Will is 15 years old!
```

Py:

```python
class Dog:
    # constructor
    def __init__(self, name):
        self.name = name

    def get_name(self):
        return self.name


# checks if a Python script is being run as the main program or if it's being imported as a module into another script.
if __name__ == "__main__":
    d = Dog(str(input("name your dog: ")))
    print((d.get_name()))

```

## User Input

```python
age = input('how old are you bitch?!: ')
```

## Try Catch

```python
try:
    # code...
except Exception:
    # handle error...
```

## Django

creating a [venv](#virtualenv-(highly-recommended)) at first is recommended...

```bash
# setup
pip install django
django-admin startproject project_name
cd project_name
python manage.py migrate
python manage.py runserver

# create a user to access admin panel
python manage.py createsuperuser

# add a new app(feature) to the project
python manage.py startapp hello

```

### good links

* [Django not in 100 Seconds | Django for Beginners](https://youtu.be/0gT0xJ5M6Fs)

* [Python Django Explained In 8 Minutes](https://youtu.be/0sMtoedWaf0)

* <https://www.django-rest-framework.org/tutorial/quickstart/>
