# Python Cheatsheet for JS Developers
i will add to this as i go....
contributions are welcomed 🌻

---

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

## user input

```python
age = input('how old are you bitch?!: ')
```

## try catch

```python
try:
    # code...
except Exception:
    # handle error...
```
