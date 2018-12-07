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


## 4. List Methods
<b>Code:</b>

```fruits = ["Apples", "Oranges", "Mangos", "Pears"]```
or 
```fruits = list(("Apples", "Oranges", "Mangos", "Pears"))```

<b>Operations:</b> ```fruits.append(element)``` ```fruits.remove(element)``` ```fruits.insert(position, element)``` ```fruits.pop(position)``` ```fruits.reverse()``` ```fruits.sort()``` ```fruits.sort(reverse=True)```


## 5. Tuple
<b>Code:</b>

```fruits = ("Apples",)```

<b>Description:</b> If you are assigning a single value inside the tuple please use ```,``` otherwise without ```,``` the ```type(fruits)``` return ```<class 'str'>``` instead of ```<class 'tuple'>```

## 6. Sets
<b>Code:</b>

```fruits = {"Apples", "Oranges", "Mangos"}```

<b>Operations:</b> ```fruits.add(element)``` ```fruits.remove(element)``` ```fruits.clear()``` ```fruits.update(element)``` ```fruits.pop()```

<b>Description:</b> A set is a collection of elements which are unordered and unindexed. And no duplicate members in a set be created.


## 7. Dictionary
<b>Code:</b>

```
person = {
     'first_name' = "John",
     'last_name' = "Nash",
     'age' = 22
     }
```
     
<b>Operations:</b> ```person.get(key)``` ```person.items()``` ```person.keys()``` ```person.values()``` ```person.pop(key)``` ```person.clear()``` ```len(person)```


## 8. Merge Dictionaries
<b>Code:</b>

```
x1 = {'first_name' : 'John', 'last_name' : 'Doe'}
y1 = {'age' : 31, 'gender' : 'male'}

merge_x1_y1_dict = {**x1, **y1}

```

<b>Description:</b> We can merge two or more dictionaries using ```**``` operator as shown in above code. In case if the key finds similar in two or more dictionaries, then the value of the key will be updated with the dictionay defined last.

## 9. Lambda Functions
<b>Code:</b> 

```
getSum = lambda num1, num2: num1 + num2
print(getSum(10, 3))
```

<b>Description:</b> A Lambda function ( ```lambda <arguments> : <expression>``` ) can take as many number of arguments, but can only have one expression.


### Stay Tuned for more learning...
