# Lecture 02 | Core Elements of a Program #

## IDLE ##
IDLE is the **IDE (Integrated Development Environment)** built for Python. So what does make a IDE:-
* Specialized Text Editor
* Provides Highlighting
* Auto Completion
* Smart Indent
* It also includes a **Shell** which is the environment that actually interprets the python code.
* Integrated Debugger, print statements are our friend.

## Object ##
Everything in python in `Object`, in fact Python code itself is an object. Each Object have a `type` which tells us
* Kind of object it is
* What can be done with the `object`
### Type of Object ###
There is a built in function called `type`, to find the "typeof" an object. There are two fundamental type of Object:- 
* **Scalar**:  These are indivisible, i.e. basic type which cannot be created from any other type.
* **Non Scalar**
### Scalar Type ###

The following are the **scalar type**.
* int
* float

#### Integers####
Integers in Python are represented as `int`,  for every type we write, we call the value assigned to it as **literal**. 
ex:-   
````
3
````
So when we check the `type` of `3` as shown below.  
````
type(3)
````
it will give the output as  
````
<type 'int'>
````
So the type of literal `3` is `int`

#### Float ####
Float's correspond to what we call **real numbers**.   
ex:- 
````
3.2
````
check the `type` of `3.2` as shown  
````
type(3.2)
````
it will give the output as   
````
<type 'float'>
````

So in python `3` is an `int` but `3.0` is a `float`.

**NOTE:- ** 
* Do not `float` same as real number, they are similar but not the same.

#### Boolean ####
Boolean have only two values.
* `True`, so `type(True)` gives `<type 'bool'>`
* `False`

#### None ####
There is also a value called `None`, whose `type` is `<type 'NoneType'>`. It is used when we want to fill the value of something temporarily.

### Non-Scalar Type ###
Python does not have a fundamental type for characters called `char`, as available in other programming languages, In its place we have `str`.
ex:-
````
'a'
````
when we check the `type` of `'a'` we get  
````
<type 'str'>
````

Literal of type `str` can be written with either `' '` or `""`.

## Operator ##

* **Expression:-** Sequence of operator and operands objects. 

ex:- 
````
3 + 2
````
gives an output as `5`, Now consider these two example.  

````
3/2
````
`/` is the **divide operator**, gives the output as `1` but consider this example.

````
3.0/2.0
````
gives the output as `1.5`.

**NOTE:-**
* Divide operator `/` on integer returns a literal with passing it by a  **floor** operator, which is not allowed in Python version 3.0
* User floating point number to get result as same as real number division.

## Overloading ##
Now consider this example, 
````
'a' + 'b'
````
returns `"ab"`

By this we can deduce that the operator `+` is **overloaded**.  **Overloaded Operators** have a meaning that depends on the type of the operands.

## Commands ##

**Program or Scripts**: These are sequence of commands, each commands telling the interpreter to do something.  
ex:- 
````
print type(5.6)
````
## Variables & Assignment ##
Consider this example, 

````
x = 3
````
The above expression is an **assignment** expression, and `x` is a **variable**. In Python, a variable is just a name for an object.

An **assignment** expression, binds a variable with a value/object.

## Input ##

To receive input from a keyboard we use `raw_input`
There are two type of input statement in Python2, 

* `raw_input`, only one present in Python 3,  it outputs all the input as strings. 
* `input`

**NOTE:-** Be careful python shell does print the quotes around the strings in shell.

## Straight Line and Branching Program ##

All the program seen till now are **Straight Line Program**, which is executing a sequence of commands one after another without making any deviations.

### Conditional Statement ###
Conditional statements are used to make decision about the flow of a programs. using this words.  
* `if`
* `else`
* `elif` : else if


ex:-

````
if x%2 == 0:
    print "Even"
else:
    print "Odd"    
````
The operator `==` is used to do a comparison.
We can also nest one condition inside another condition as shown below...:- 

````
if x%2 == 0:
    print "Even"
else:
    if x % 3 != 0
        print "Hello"
    print "Odd"    
````
Here is what an `if` constructs does:-
* Checks the condition, if it is true executes the `if ` block,
* Else block is executed
* It will either execute the `if` block or the `else` block but never both.
* The indentation is very important in python.  Because of this the visual structure is following the semantic structure. 

## Looping Construct ##
When we add loops to a programming language, these programing language belongs to a class of programming language called **Turing Complete**. The concept of Loops are called **iteration**.  
With loops, we can execute a same instructions multiple times.

Here is a simple loops.

````
while ans*ans*ans < abs(x):
    ans = ans + 1
``











