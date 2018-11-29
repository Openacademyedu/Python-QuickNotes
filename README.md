# Python QuickNotes
Python QuickNotes help you learn python.

Follow the quick notes to learn python programming.

## 1. Multiple Assignment

<b>Code:</b> 

```name, age, weight, is_male = ("John", 22, 65.4, True)```

<b>Description:</b>

We can assign multiple variables at a single time. The above code is equivalent to -

```name = "John"```

```age = 22```

```weight = 65.4```

```is_male = True```


## 2. String Formating
### 2.1. Argument by position

<b>Code:</b> 

```name, age = ("Alexa", 18)```

```print("My name is {name} and I am {age} years old.".format(name=name, age=age))```

<b>Description:</b>

We can position the arguments inside the ```{ }``` and then call the ```.format()``` method.

### 2.2. F-Strings

<b>Code:</b>

```print(f"My name is {name} and I am {age} years old.")```


## 3. String Methods
<b>Code:</b>

```s = "hello world"```

<b>Operations:</b> ```s.capitalize()``` ```s.upper()``` ```s.lower()``` ```s.swapcase()``` ```len(s)``` ```s.replace(old, new, count)``` ```s.count(substring)``` ```s.startswith(substring)``` ```s.endswith(string)``` ```s.split()``` ```s.find(substring)``` ```s.isalnum()``` ```s.isalpha()``` ```s.isnumeric()```
