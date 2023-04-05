# Python Cheatsheet for JS Developers
i will add to this as i go....
contributions are welcomed 🌻

---

`JS` --> ```Python```

---

# General

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
