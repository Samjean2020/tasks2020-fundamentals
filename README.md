# tasks2020-fundamentals
README
                                                               
                                                               Introduction
                                                                  
Tasks2020 Assignment contains four different tasks, including Python function called counts for transforming inputs list outputs to a dictionary, Python function called dicerolls that simulates rolling dice, Python code that simulates flipping a coin 100 times, and  Simpson’s paradox demonstration using Numpy.

                                                                Running of codes

                                                                Prerequisites
These are:
Numpy for mathematics or numerical operations;
Matplotlib.pyplot for plotting;
Pandas for data manipulation and analysis; 
Seaborn for data visualisation;
Jupyter Notebook for text, code, and visualisations; and
Python programming language for the execution of all instructions.

                                                                 Description of Algorithms

                                                                 Task1
                                                                    
1. October 5th, 2020: Write a Python function called counts that takes a list as input and returns a dictionary of unique items in the list as keys and the number of times each item appears as values. So, the input ['A', 'A', 'B', 'C', 'A'] should have output {'A': 3, 'B': 1, 'C': 1}. 
Your code should not depend on any module from the standard library or otherwise. You should research the task first and include a description with references of your algorithm in the notebook.

                                                                  Code description
                                                                
•	Define Python function called counts as per problem statement.
•	Create a variable and allocate an empty dictionary where output from list will be stored. 
•	Set up a for loop to loop over the bloc to generate keys and values by connecting the variable count with get () function and return count.
•	dict.get () function method—is an approach that enables the program to work more efficiently with minimal algorithm [1, 2.].
•	get () function default will return None if the key is not present [1, 2].
•	count () a Python built-in function will return the frequency of a specified item in list [3].
•	Set a driver function to enable the Python Interpreter to read the source code[4, 5]
•	And finally, call the function print () to execute the program.

References about the above task are included within the Jupyter Notebook


                                                                   Task2
                                                                
2. November 2nd, 2020: Write a Python function called dicerolls that simulates rolling dice. Your function should take two parameters: the number of dice k and the number of times to roll the dice n. The function should simulate randomly rolling k dice n times, keeping track of each total face value. It should then return a dictionary with the number of times each possible total face value occurred. So, calling the function as dicerolls(k=2, n=1000) should return a dictionary like: {2:19,3:50,4:82,5:112,6:135,7:174,8:133,9:114,10:75,11:70,12:36} You can use any module from the Python standard library you wish and you should include a description with references of your algorithm in the notebook. 1By the standard library, we mean the modules and packages that come as standard with Python. Anything built-in that can be used without an import statement can be used.

                                                                   Code description

•	Import defaultdict () function from collections in Python to perform operations within the script.
•	Import randit () function to randomly generate integers.
•	Create a variable called rolls to allocate the default dictionary function.
•	Set a Python function to group instructions within the bloc:            define dicerolls () function, its argument must encapsulate two       parameters as per problem statement.
•	Set up a for loop, to loop over the bloc until the settled conditions are met: for in range () to perform the rolling of dice action 1000 times.
•	Randomly generate integers for the dice 2, from 2 to 12 and increase the corresponding output plus 1.
•	Call the defined function direrolls () 
•	And finally, call the function print () to output rolls variable content.

References about the above task are included within the Jupyter Notebook.

                                                                    Task3

November 16th, 2020: The numpy.random.binomial function can be used to simulate flipping a coin with a 50/50 chance of heads or tails. Interestingly, if a coin is flipped many times then the number of heads is well approximated by a bell-shaped curve. For instance, if we flip a coin 100 times in a row the chance of getting 50 heads is relatively high, the chances of getting 0 or 100 heads is relatively low, and the chances of getting any other number of heads decreases as you move away from 50 in either direction towards 0 or 100. Write some python code that simulates flipping a coin 100 times. Then run this code 1,000 times, keeping track of the number of heads in each of the 1,000 simulations. Select an appropriate plot to depict the resulting list of 1,000 numbers, showing that it roughly follows a bell-shaped curve. You should explain your work in a Markdown cell above the code.


We can solve this problem by using the numpy.random.binomial function. In numpy.random.Generator.binomial with a method as Generator.binomial(n, p, size=None) we can draw samples from a binomial distribution. Samples are drawn from a binomial distribution with specified parameters, n trials and p probability of success where n an integer >= 0 and p is in the interval [0,1]. (n may be input as a float, but it is truncated to an integer in use) [1]

                                                                    Code description

•	numpy.random.binomial function draw from distribution
•	Select an appropriate plot to depict the resulting list of 1,000 numbers, showing that it roughly follows a bell-shaped curve.
•	Create a variable named random number generator, rng in short to assign the function np.random.default_rng() function.
•	Have n as integer at 100 as number to simulate flipping a coin and p as interval at .5 as probability of each trial.
•	Create a variable named s to allocate the rng.binomial function containing 3 parameters in the argument n, p, and 1000 as number of times to run the script.
•	Test 1000 times, the result of flipping a coin 100 times 
•	Select an appropriate plot to depict the resulting list of 1,000 numbers, showing that it roughly follows a bell-shaped curve. 

References about the above task are included within the Jupyter Notebook.

