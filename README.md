Download Link: https://assignmentchef.com/product/solved-cmpt141-assignment2-functions
<br>
<strong>Question 1 </strong>

<strong>Purpose: </strong>To distinguish between the different parts of functions and function calls.

<h1>Degree of Difficulty: Easy</h1>

<table width="652">

 <tbody>

  <tr>

   <td width="652">def calculate_coffee( num_coffee, price_coffee, discount):“””Computes the total amount due for the purchase of num_coffeenum_coffee: An Integer for the number of coffees purchased price_coffee: A Float for the price per coffee discount: A Float for a discount off the purchase price returns: the total amount due from the customer“”” total_before_tax = num_coffee * price_coffee total_after_tax = add_tax(total_before_tax) total_after_discount = total_after_tax – discount return total_after_discountdef add_tax(cost):“””Adds 7% tax to the costreturns total the amount including tax“””total = cost * 1.07 return total# compute the total for 1 coffee at $2.00 per coffee, no discount customer1 = calculate_coffee(1, 2.00, 0)# compute the total for 3 coffees at $3.25 per coffee, $2.00 discount customer2 = calculate_coffee(3, 3.25, 2.00)# compute the total for 7 coffees at $2.75 per coffee, $5.00 discount customer3 = calculate_coffee(7, 2.75, 5.00)</td>

  </tr>

 </tbody>

</table>

Below is a program that uses functions to compute the total cost of purchasing coffees. It includes the ability to calulate tax and subtract a discount from the purchase.

1

2

3 4 5 6

7 8

9

10

11 12

13 14

15 16

17 18

19 20

21

22

23 24

25 26

27 28

29

30

31

Answer the following questions. Refer to line numbers if you find it helpful in your answers.

<ul>

 <li>List all of the <em>function parameters </em>in this program.</li>

 <li>List all of the <em>function arguments </em>in this program.</li>

 <li>List all of the variables that are not <em>arguments </em>or <em>parameters</em>.</li>

 <li>What is the <em>scope </em>of the folowing variables:

  <ol>

   <li>total_after_tax</li>

   <li>cost</li>

  </ol></li>

</ul>

<ul>

 <li>customer2</li>

</ul>

<ul>

 <li>How many <em>function definitions </em>are in this program?</li>

 <li>How many <em>function calls </em>are in this program?</li>

 <li>What is the value of customer1 when the program ends?</li>

</ul>

<strong>Question 2:</strong>

<strong>Purpose: </strong>To write a function that performs a subtask and returns an answer.

<h2>Degree of Difficulty: Easy</h2>

A travel agent would like to compute the total cost of a trip that includes a flight, plus a number of nights at a hotel for a group of people. The agent is assuming double occupany, which means two will share each hotel room, unless there is an odd number of people. Thus to determine the <strong>number of rooms </strong>required each night you could use the formula

number_of_rooms = number_of_people // 2 + number_of_people % 2

Write a Python function trip_cost that takes four parameters as input and returns the <strong>total cost of the trip</strong>. The four parameters should be the <strong>airfare </strong>in dollars, the <strong>room cost </strong>per night in dollars, the <strong>number of people</strong>, and the <strong>number of nights</strong>.

Ask the user to input values for each of the function arguments from the console. You may assume that the user supplies valid input. Call the trip_cost function with the arguments you read from the console and output the its return value to the console.

Your function trip_cost should do no console input and no console output. It must receive its input through its parameters and send its output using a return value.

<strong>NOTE: </strong>The cost of flight is <strong>per person </strong>and not for the whole group.

<h1>Sample Run</h1>

Here is an example of how your program’s console output might look. Green text was entered by the user;

<table width="652">

 <tbody>

  <tr>

   <td width="652">Calculate Trip CostEnter cost of flight ($): 1000Enter cost of a double room per night:100.00Enter the number of people: 11 Enter the number of nights:7The total cost of the trip for the group is $15200.0</td>

  </tr>

 </tbody>

</table>

blue text came from data returned by the function.




<strong>Question 3 :</strong>

<strong>Purpose: </strong>To write a function that performs a subtask and returns an answer.

<h2>Degree of Difficulty: Easy</h2>

In Physics the speed of a moving object can be calculated by dividing the distance traveled by the time taken:

<em>speed </em>= <em>distance </em>÷ <em>time</em>

Write a Python function named calculate_speed which has two parameters (distance and time) and returns the value of speed.

Also write a main program that reads the two necessary values from the user, passes the entered values to the calculate_speed function to perform the computation, obtains the function’s return value, then prints a message to the console that reports the value of speed.

Your function calculate_speed should do no console input and no console output. It must receive its input through its parameters and send its output using a return value.

<h1>Sample Run</h1>

Here is an example of how your program’s console output might look. Green text was entered by the user;

<table width="652">

 <tbody>

  <tr>

   <td width="652">Calculate SpeedEnter desired distance (km): 510 Enter desired time (hours): 5In order to travel 510 km in 5 hours you must travel at 102 km/h.</td>

  </tr>

 </tbody>

</table>

blue text came from data returned by the calculate_speed function.

The above shows the result of traveling 510 km over 5 hours.

<strong>Question 4 :</strong>

<strong>Purpose: </strong>Solve a problem by writing multiple functions that perform different subtasks, and combining their use to solve a larger problem. Also to practice documenting functions.

<h2>Degree of Difficulty: Moderate</h2>

Siblings John and Jane opened up a lemonade stand for a day to raise funds for buying their first dog. The lemonade was a hit! What they weren’t sure about was how much money they earned at the end of the day.

Your task is to write a Python program that calculates and displays the amount of funds raised by the youth after taking their expenses into consideration, that is, their profit. To accomplish this, you will need to write three Python functions: cost, revenue, and profit.

The cost function should take parameters n_lemons (the number of lemons bought and used to make lemonades), cost_per_lemon (price per lemon), and return the total cost of running the lemonade service. The total cost is:

<em>total</em>_<em>cost </em>= <em>number of lemons </em>× <em>cost per lemon.</em>

The revenue function should take parameters donations (the amount of money donated towards their cause), n_lemonades (the number of lemonades sold), price_per_lemonade (the selling price for one lemonade) and return the total amount of money earned. The total money earned is:

<em>total</em>_<em>revenue </em>= <em>donations </em>+ <em>money earned from lemonades sold</em>

The profit function determines the net profit (net money earned) by the youth. It should:

<ul>

 <li>call cost and revenue and use their return values to compute the net profit earned by the siblings;</li>

 <li>return the computed profit.</li>

</ul>

The parameters of the profit function should be chosen so that they provide the necessary information required to call the cost and revenue functions. The profit is:

<em>profit </em>= <em>total</em>_<em>revenue </em>− <em>total</em>_<em>cost</em>

You must now test your program by preparing three examples (of number of lemons used, buying price per lemon, number of lemonades sold, selling price per lemonade, and donations) in advance so that you can judge whether your program is correct. Write code to ask the user for all five of these inputs, then display the cost, revenue, and profit of each prepared example to the console. Copy the console output from each of your three testing example into a text file and hand that text file in (see “What to Hand In”, below).

You may assume that the user supplies valid input from the console, that is, a positive number for the number of lemons, the buying price per lemon, the number of lemonades sold, the selling price per lemonade, and for monetary amount of donations received. See the sample run on the next page.

<h1>Sample Run</h1>

Here is an example of how your program’s console output might look. Green text was entered by the user;

blue text came from data returned by the function.

How many lemons were used?: 5

What was the cost per lemon (in dollars)?: 1.15

How many lemonades were sold?: 25

What was the selling price of one lemonade (in dollars)?: 0.50

How much money did you receive in donations (in dollars)?: 10.00 Revenue: $22.5

Costs: $5.75

<table>

 <tbody>

  <tr>

   <td> </td>

  </tr>

 </tbody>

</table>

Profit: $16.75


