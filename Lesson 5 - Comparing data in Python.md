## Lesson 5 - Comparing data in Python
```bash
from helper_functions import print_llm_response, get_llm_response
```
Take a closer look at the True/False variable you saw at the end of the last lesson.
```bash
food_preferences_tommy = {
    #"dietary_restrictions": "vegetarian",
    "favorite_ingredients": ["mushrooms", "olives"],
    "experience_level": "intermediate",
    "maximum_spice_level": 6
}
```
You added the element "is vegetarian" with a value equal to True
```bash
food_preferences_tommy["is_vegetarian"] = True
```
This type of data is known as booleans. It can take only two values: True or False.
```bash
print(food_preferences_tommy)
```
### True and False
True and False may look like strings without quotation marks. They are the two values that booleans can take.
```bash
print(True)
print(False)
```
Below, you can check the type for each of these values.
```bash
type(True)
type(False)
```
If you're curious, ask chatbot why it's called Boolean
```bash
🤖 Use the Chatbot: Why is the True or False data type called a Boolean?
```

As with any other data type, you can assign booleans to variables:
```bash
is_tommy_my_friend = True
is_isabel_older_than_me = False
print(is_tommy_my_friend)
print(is_isabel_older_than_me)
type(is_isabel_older_than_me)
```
### Comparison Operators
Booleans are what you get back when you compare variables in python. For example, here are the ages for Isabel, Daniel and Tommy:
```bash
isabel_age = 28
daniel_age = 30
tommy_age = 30
```
In Python you can compare values using the same operator you probably encounter in math classes. Let's start determining if Isabel is older than Daniel using >.
```bash
print(isabel_age > daniel_age)
```  
Now, let's determine if she is younger using <:
```bash
print(isabel_age < daniel_age) 
is_isabel_older_than_daniel = isabel_age > daniel_age
print(is_isabel_older_than_daniel)
```
You can also use <= and >= to check if one number is greater than or equal to the other, or if it is lower than or equal to the other.
```bash
print(isabel_age <= daniel_age)
```
Since Daniel and Tommy are the same age, when you use <= and >= you will get True for both cases:
```bash
print(tommy_age < daniel_age)
print(tommy_age <= daniel_age)
```
### Equality Operator

So, what if you want to check if to things are equal? You would neeed to use ==.

=is an assignment operator, it assigns values to variables
== is a comparison operator, it checks if two things are holding the same value, or if two pieces of data are equal
So, going back to comparing Daniel's and Tommy's age:

print(tommy_age == daniel_age)
And Isabel's and Daniel's:
```bash
print(isabel_age == daniel_age)
```
This operator works for strings too. Here you have definitive proof that a vegetarian is not the same as a vegan.
```bash
#strings
print("vegetarian" == "vegan")
```
### Logical Operators
Operations with booleans involve logical operators like and and or. Let's define a couple of boolean variables:
```bash
is_tommy_my_friend = True
is_isabel_my_friend = True
```
If you want to check whether both Tommy and Isabel are your friends, you can use the and operator:
```bash
print(is_tommy_my_friend and is_isabel_my_friend)
```
If you want to check whether at least one of them is your friend, you can use the or operator:
```bash
print(is_tommy_my_friend or is_isabel_my_friend)
```
Let's say that Isabel, Tommy and Daniel are playing a game involving their ages:
```bash
isabel_age = 28
daniel_age = 30
otto_age = 29
```
The game involves checking whether Isabel is younger than both Tommy and Daniel:
```bash
is_isabel_younger_than_tommy = isabel_age < tommy_age
is_isabel_younger_than_daniel = isabel_age < daniel_age
print(is_isabel_younger_than_tommy and is_isabel_younger_than_daniel)
```
In the next video, you will use booleans to write programs that execute different lines of code depending on the boolean value.

### Extra practice
Please go through the exercises in the cells below if you want some extra practice for the topics you covered in this lesson.
```bash
# Check whether Isabel is older
# than at least one of my friends (Tommy and Daniel)
​
### EDIT THE FOLLOWING CODE ###
# Hint: Replace the "?" with the correct comparison operator
is_isabel_older_than_tommy = isabel_age ? tommy_age
is_isabel_older_than_daniel = isabel_age ? daniel_age
### --------------- ###
​
### EDIT THE FOLLOWING CODE ###
#Hint: Recall the logical operators "and" and "or" 
print("Check if Isabel is older than at least one of my friends")
### --------------- ###
```
