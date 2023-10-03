# Python Cheatsheet for JS Developers

i will add to this as i go....
contributions are welcomed 🌻

## Table of Contents

* [virtualenv](#virtualenv-(highly-recommended))
* [General](#General)
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
