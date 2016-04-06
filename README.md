# Cssi Prework Python Looping

## Objectives

1. Explain the purpose of using loops
2. Distinguish between the different loops available in Python
3. Use for and while loops to iterate through a list.

##Loops
Loops are a common tool is any programing language that lets us repeat a section of code over and over, even if we only type it out once. You have already seen loops once in JavaScript, and now that you understand Python's list syntax, it's important to be able to iterate over each item in a list, or (as you'll learn in the next lesson) over other datatypes.


###For Loops
The simplest looping situation is where you need to do something _for_ a certain number of times. In this case, the number of iterations is known. To do this, Python uses a for loop.

##### Example 1: Looping Through a List

This code will repeat for every element in the list.

```python
>>>for name in ["Lucy", "Ricky", "Ricky Jr."]:
>>>    print "Hi, my name is "+ name

Hi, my name is Lucy
Hi, my name is Ricky
Hi, my name is Ricky Jr.

```
Note that the variable `name` is what we are calling each element within the list. We could call that variable anything: `character`, `person`, `actor`. It doesn't matter, as long as we continue to use that variable later within the _for_ block.

Alternatively, we can declare a variable `names` which contains a list of all three members in the Ricardo family, and then use the same syntax.
```python
#same result, slightly different syntax
>>>names = ["Lucy", "Ricky", "Ricky Jr."]
>>>for person in names:
>>>    print "Hi, my name is "+ name

Hi, my name is Lucy
Hi, my name is Ricky
Hi, my name is Ricky Jr.

```
##### Example 2: Looping through Integers

The _for_ loop syntax is similar for integers. In the example below, string interpolation (a jargony word that means substitution) is used. The curly brackets act as a placeholder. The .format() method that is chained to the end of the string indicating which value should be substituted into the placeholder.

```python
>>>for i in range(1, 4):
>>>    print "I am looping and am currently on {}.".format(i)

I am looping and am currently on 1.
I am looping and am currently on 2.
I am looping and am currently on 3.

```
(Notice that the range function is not inclusive of the end number)

You can also declare your variable before the loop. And while `i` is the most common variable name for iteration, any variable name can be used.

```
>>>my_range = range(2,5)
>>>for num in my_range:
>>>    print "Did you know that {} times 2 is {}.".format(num, num*2)

Did you know that 2 times 2 is 4.
Did you know that 3 times 2 is 6.
Did you know that 4 times 2 is 8.
```

##### Example 2: Looping through a List

In the example below we'll loop through our to-do list:

```
>>>todoList = ["carve a pumpkin", "hide an egg", "cook a turkey", "light a tree"]

>>>for item in todoList:
>>>  print "Today I must {}".format(item)

Today I must carve a pumpkin
Today I must hide an egg
Today I must cook a turkey
Today I must light a tree

```
###While Loops
While loops continue to repeat _while_ - or as long as - a certain condition is met. While loops are used when we're not sure how many iterations (if any) might occur.

##### Example 1: A Simple While Loop
This code will repeat while the condition `n<5` is met. It will stop when n is equal to 5.

```python
n = 0
while n < 5:
  print n
  n = n + 1
```
##### Example 2: A While/Else Loop
While/Else is a loop type that does not exist in JavaScript. Once a condition is no longer true, the code block inside the else statement is executed.

In this case, once `n < 5` is not met, the instructions in the `else` block are executed. Then, the entire _while_ loop is exited, and the next instruction (to print `"You counted to 5"`) is executed.
```python
n = 0
while n < 5:
  print n, " is  less than 5"
  n = n + 1
else:
  print n, " is not less than 5"

print "You counted to 5"
```

#Conclusion
Creating, modifying and accessing lists are important for every programmer, as is being able to use _for_ loops and _while_ loops. Practicing these small examples are a great way to build your foundation as a strong developer and will prepare you for the next lab.
