# Python QuickNotes
Python QuickNotes help you learn python.

Follow the quick notes to learn python programming.

## 1. Variable Assignment

<b>Note:</b>
* Variable names are case sensitive i.e both <b>var</b> and <b>VAR</b> are different variables.
* Variable names must <u>start with a letter or an underscore</u>. Eg: <b>_var</b> 
* Variable names can contain a number in between but not at the start. Eg: <b>var1</b>

### 1.1 Single Assignment

<b>Code:</b>

```
x = 10 # int
z = 5.5 # float
firstName = "Alexa" # str
is_female = True # bool

```

### 1.2 Multiple Assignment

<b>Code:</b> 

```name, age, weight, is_male = ("John", 22, 65.4, True)```

<b>Description:</b>

We can assign multiple variables at a single time. The above code is equivalent to -

```name = "John"```

```age = 22```

```weight = 65.4```

```is_male = True```

## 2. Basic Maths Operations

<b>Code:</b>

```
add = x + y # addition
sub = x - y # substraction
div = x / y # division

```

## 3. Type


## 4. Casting

<b>Code:</b>

```
x = str(x) # convert to string
y = int(y) # convert to integer
z = float(y) # convert to float

```

## 5. String
### 5.1 Concatenation

<b>Code:</b>

```
name = "Alexa"
age = 18

print("Hello, My name is " + name + " and I am " + str(age) + " years old.")

```

### 5.2 Argument by position

<b>Code:</b> 

```name, age = ("Alexa", 18)```

```print("My name is {name} and I am {age} years old.".format(name=name, age=age))```

<b>Description:</b>

We can position the arguments inside the ```{ }``` and then call the ```.format()``` method.

### 5.3 F-Strings

<b>Code:</b>

```print(f"My name is {name} and I am {age} years old.")```


### 5.4 String Methods
<b>Code:</b>

```s = "hello world"```

<b>Operations:</b> ```s.capitalize()``` ```s.upper()``` ```s.lower()``` ```s.swapcase()``` ```len(s)``` ```s.replace(old, new, count)``` ```s.count(substring)``` ```s.startswith(substring)``` ```s.endswith(string)``` ```s.split()``` ```s.find(substring)``` ```s.isalnum()``` ```s.isalpha()``` ```s.isnumeric()```


## 6. List

<b>Note:</b>
* List is a collection which is ordered and changeable.
* Allow duplicate members.

### 6.1 Create List

<b>Code:</b>

```fruits = ["Apples", "Oranges", "Mangos", "Pears"]```
or 
```fruits = list(("Apples", "Oranges", "Mangos", "Pears"))```

### 6.2 List Methods

<b>Operations:</b> ```fruits.append(element)``` ```fruits.remove(element)``` ```fruits.insert(position, element)``` ```fruits.pop(position)``` ```fruits.reverse()``` ```fruits.sort()``` ```fruits.sort(reverse=True)```


## 7. Tuple

<b>Note:</b>
* Tuple is a collection which is ordered and unchangeable. 
* Allow duplicate members.


<b>Code:</b>

```fruits = ("Apples",)```

<b>Description:</b> If you are assigning a single value inside the tuple please use ```,``` otherwise without ```,``` the ```type(fruits)``` return ```<class 'str'>``` instead of ```<class 'tuple'>```

## 8. Sets

<b>Note:</b>
* A set is a collection of unordered and unindexed. 
* No duplicate members.


<b>Code:</b>

```fruits = {"Apples", "Oranges", "Mangos"}```

<b>Operations:</b> ```fruits.add(element)``` ```fruits.remove(element)``` ```fruits.clear()``` ```fruits.update(element)``` ```fruits.pop()```


## 9. Dictionary

<b>Note:</b>
* A dictionary is a collection which is unordered, changeable and indexed.
* No duplicate members.

### 9.1 Create Dictionary

<b>Code:</b>

```
person = {
     'first_name': "John",
     'last_name': "Nash",
     'age' = 22
     }
```
     
### 9.2 Common Operations

<b>Operations:</b> ```person.get(key)``` ```person.items()``` ```person.keys()``` ```person.values()``` ```person.pop(key)``` ```person.clear()``` ```person.copy()``` ```len(person)```


### 9.3 Merge Dictionaries
<b>Code:</b>

```
x1 = {'first_name' : 'John', 'last_name' : 'Doe'}
y1 = {'age' : 31, 'gender' : 'male'}

merge_x1_y1_dict = {**x1, **y1}

```

<b>Description:</b> We can merge two or more dictionaries using ```**``` operator as shown in above code. In case if the key finds similar in two or more dictionaries, then the value of the key will be updated with the dictionay defined last.


## 10. Lambda Functions
<b>Code:</b> 

```
getSum = lambda num1, num2: num1 + num2
print(getSum(10, 3))
```

<b>Description:</b> A Lambda function ( ```lambda <arguments> : <expression>``` ) can take as many number of arguments, but can only have one expression.


## 11. Function Argument Unpacking
### 11.1 List/Tuple
<b>Code:</b>

```
def about(name, age, country):
    print(f"My name is {name} and I am {age} years old. I live in {country}.")
    
about_data = ["John Doe", 22, "USA"]

about(*about_data)

```

<b>Description:</b> In case your data is in a list or tuple then you can fetch it using ```*``` operator i.e. ```about(*about_data)``` instead of typing ```about(about_data[0], about_data[1], about_data[2])```  where ```about_data``` is the variable assigned to your list.

### 11.2. Dictionary
<b>Code:</b>

```
def about(name, age, country):
    print(f"My name is {name} and I am {age} years old. I live in {country}")
    
about_data = {'name': "John Doe", 'age': 22, 'country': "USA"}

about(**about_data)

```

<b>Description:</b> In case you have to parse your data (inside a dictionay) then you just have to use ```**``` operator in place of single ```*``` operator. <b>Note that in case of using dictionay the arguments must match exactly with the dictionay keys.</b>



### Stay Tuned for more learning...
