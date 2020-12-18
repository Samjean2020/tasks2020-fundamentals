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
                                                          Import relevant Python modules
#Import Numpy as np for numerical arrays and fitting lines.
#Import Matplotlib.pyplot as plt for plotting.
#Use the IPython magic command %matplotlib inline for displaying plots[1]
#Import seaborn as sns for data visualisation.
#Import pandas as pd for data analysis and manipulation.
#Use plt.style.use ("ggplot") to display nicer plot style.
#Use plt.rcParams["figure.figsize"] to get big size plots.rcParams defines the default values, which can be modified in the matplotlibrc file[4].

                                                         1st part of the code [2]

#Draw samples from a binomial distribution using Numpy random default random generator function by setting a variable first as rng = np.random.default_rng()[2].
#Set number of trials and probability of each trial as n, p = 100, .5[2].
#Set number of time to run the code using random number generator binomial function by setting a variable first as s = rng.binomial(n, p, 1000)[1].
#Check the result of flipping a coin 100 times, tested 1000 times as sum(rng.binomial(100, 0.1, 1000) == 0)/1000 [2].
#Simulation by calling s variable.

                                                         2nd part of the code [3]

#Set elements of normal distribution (mu and sigma)[3] as mu, sigma = 100, .5.
#Set a variable to generate random values as s = np.random.normal(mu, sigma, 1000)[3].
#Create the bins and histogram using matplotlib.pyplot histogram function as count, bins, ignored = plt.hist(s, 20, density=True)[3].
#Plot the distribution curve using matplotlib.pyplot function as plt.plot(bins, 1/(sigma * np.sqrt(2 * np.pi)) * np.exp( - (bins - mu)2 / (2 * sigma2) ), linewidth=3, color='b') [3].
#Display plot using matplotlib.pyplot function as plt.show().

References about the above task are included within the Jupyter Notebook.

                                                                  Task4.
4.	November 30th, 2020: Simpson’s paradox is a well-known statistical paradox where a trend evident in a number of groups reverses when the groups are combined into one big data set. Use numpy to create four data sets, each with an x array and a corresponding y array, to demonstrate Simpson’s paradox. You might create your x arrays using numpy.linspace and create the y array for each x using notation like y = a * x + b where you choose the a and b for each x , y pair to demonstrate the paradox. You might see the Wikipedia page for Simpson’s paradox for inspiration.
                                                            Code description

                                                  Import relevant Python modules
Import numpy as np for numerical arrays and fitting lines; matplotlib.pyplot as plt for plotting. Use the Ipython magic command %matplotlib inline for displaying plots[1]. Import seaborn as sns for data visualisation and pandas as pd for data analysis and  manipulation. Use plt.style.use ("ggplot") to display nicer plot style. Use plt.rcParams["figure.figsize"] to get big size plots.rcParams defines the default values, which can be modified in the matplotlibrc file[3]. 

                                                  Generate four datasets
Set variables a and b and generate datasets(x1,x2,x3,x4) with their corresponding y variables(y1,y2,y3,y4) using numpy linspace function for x variables as np.linspace() and numpy random normal function for y variables as a * x + b + np.random.normal(). Parameters within each argument, including noise must be adapted. np.linspace() returns evenly spaced numbers over a specified interval[4]. np.random.normal() draws random samples from a normal distribution[5]. Check the size of variables for the dataset 1 using the len function as len(). This verification of size can be done to other datasets variables. Request the coefficients of both variables (x and y) of each dataset using polyfit function as np.polyfit(x1, y1, 1). A coefficient is a number multiplied by a variable [2] as a * x + b.

                                                  Generate trend lines
Generate trend lines using seaborn regression plot x and y variables of each dataset as sns.regplot(x = x1, y = y1) for the first dataset. sns.regplot plots data and a linear regression model fit[6], [7].

                                                  Demonstrate the Simpson's paradox
Demonstrate the Simpson's paradox by combining parameters of different groups using seaborn sns.regplot () function Combining Group 1 with group 2 as sns.regplot(x = x1, y = x2) and combining Group 3 with group 4 as sns.regplot(x = x3, y = x4).

                                                  Synchronise all four plots in one plot
Synchronise all four plots in one plot using sns.regplot() function as sns.regplot (x1, y1, '.', label="Data set 1") for the dataset 1.

                                                  Fitting with polyfit

                                                  About coefficients
Retrieve coefficients of all four datasets variables using Numpy np.polyfit() function as np.polyfit(x1, y1, 1) for the dataset 1.

                                                  Fit each using polyfit
Fit each dataset variables using Numpy polyfit()function as coeffs1 = np.polyfit(x1, y1, 1) for dataset 1 and call coeffs1.

                                          Demonstrate Simpson's paradox (plt.plot ())
Demonstrate Simpson's paradox using coefficients of all four datasets using Matplotlib.pyplot() function as plt.plot () for dataset1 as below:
plt.plot(x1, y1, '.', label="Data set 1") plt.plot(x1, coeffs1 [0] * x1 + coeffs1 [1], '-', label='Best fit line 1')


References about the above task are included within the Jupyter Notebook.

