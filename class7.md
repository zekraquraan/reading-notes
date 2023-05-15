## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

# Variable Scope in Python:
# Variable scope refers to the portion of a program where a variable is accessible and can be referenced. In Python, there are two main types of variable scope: local scope and global scope.

# Local Scope: Variables defined within a function have local scope, meaning they are only accessible within that specific function. Local variables are created when the function is called and are destroyed when the function execution completes.
# Global Scope: Variables defined outside of any function or in the global scope are considered global variables. Global variables are accessible from anywhere within the program, including inside functions.
# x = 10  # global variable

# def my_function():
   # global x
   # x = 20  # modifying the global variable
   # print(x)

# my_function()  # Output: 20
# print(x)  # Output: 20
## How do the global and nonlocal keywords work in Python, and in what situations might you use them?
# Nonlocal Keyword: The nonlocal keyword is used to indicate that a variable is defined in the nearest enclosing scope that is not global. It is used when you want to access or modify a variable from an outer (enclosing) scope in a nested function.

    
    
## In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.
# Big O notation is a way to analyze and describe the efficiency or complexity of an algorithm. It provides a mathematical representation of how the runtime or space requirements of an algorithm grow as the input size increases
## Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.
# To simulate a dice roll using Python, you can use the random module, which provides functions for generating random numbers. Here's an example of how you can simulate a dice roll:

# python



# import random

# def roll_dice():
   # return random.randint(1, 6)  # Generate a random number between 1 and 6

# Simulating a dice roll
# result = roll_dice()
# print(f"The dice rolled: {result}")
# In the above code, the roll_dice() function uses random.randint() to generate a random integer between 1 and 6, simulating a dice roll.

# To calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials, you can simulate multiple dice rolls and count the occurrences of the desired outcome. Here's an example:


# import random

# def roll_dice():
  #  # return random.randint(1, 6)

# def calculate_probability(target_number, num_trials):
 #   occurrences = 0

 #   for _ in range(num_trials):
 #       result = roll_dice()
  #      if result == target_number:
   #         occurrences += 1

   # probability = occurrences / num_trials
   # return probability

# target_number = 6
# num_trials = 1000000

# probability = calculate_probability(target_number, num_trials)
# print(f"The probability of rolling a {target_number} is approximately: {probability}")
# In the above code, the calculate_probability() function takes the target number (in this case, 6) and the number of trials as arguments. It simulates the dice rolls for the specified number of trials and counts the occurrences of the target number. Finally, it calculates the probability by dividing the number of occurrences by the total number of trials.

# By increasing the num_trials parameter, you can get a more accurate estimation of the probability.


## Things I want to know more about
# How do the global and nonlocal keywords work in Python, and in what situations might you use them?