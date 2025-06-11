# OPTIMIZATION-MODEL
COMPANY : CODTECH IT SOLUTIONS
NAME : MANDRAJULA ARUN PRABHU TEJA
INTERN ID : CT06DF375
DOMAIN : DATA SCIENCE
DURATION : 6 WEEKS
MENTOR : NEELA SANTHOSH KUMAR

📊 Problem Statement :

Title: Optimizing Workforce Scheduling Using Linear Programming

Introduction :

Workforce scheduling is a critical operational challenge faced by many service-based industries such as customer support centers, healthcare facilities, retail chains, and logistics companies. The objective is to ensure that there are enough workers available on each day of the week to meet customer demand, while simultaneously minimizing labor costs and avoiding overstaffing. Achieving this balance is complex due to constraints such as employee shift lengths, rest days, and varying daily demand levels.

This project aims to solve a real-world business problem by developing an optimization-based workforce scheduling system. The solution is built using Linear Programming (LP) with the PuLP library in Python. The core idea is to determine the optimal number of employees that should start their 5-day shifts on each day of the week to satisfy daily staffing requirements with the fewest number of workers possible.

Problem Definition :

The business scenario assumes a 7-day workweek, where each worker is scheduled to work 5 consecutive days. For instance, an agent starting work on Monday will work from Monday through Friday, while someone starting on Saturday will work through Wednesday.

Each day of the week has a predefined minimum required number of agents to ensure smooth operations:

Day	Minimum Agents Needed
Monday	17
Tuesday	13
Wednesday	15
Thursday	19
Friday	14
Saturday	16
Sunday	11

The goal is to determine the minimum number of employees and their corresponding start days such that these daily requirements are met.

Objectives :

Define a mathematical model using linear programming.

Minimize the total number of agents required.

Ensure that on each day, the number of available agents (working that day) is at least the minimum required.

Visualize the distribution of agent start days using bar and line plots.

Methodology
Decision Variables:
Let 
𝑥
𝑖
x 
i
​
  represent the number of agents who start their 5-day shift on day 
𝑖
i (where 
𝑖
∈
{
Mon
,
Tue
,
…
,
Sun
}
i∈{Mon,Tue,…,Sun}).

Objective Function:
Minimize the total number of agents:

Minimize
∑
𝑖
𝑥
𝑖
Minimize 
i
∑
​
 x 
i
​
 
Constraints:
For each day, ensure the sum of agents working that day (based on their shift start day) meets or exceeds the required demand.

Solver:
Use PuLP’s built-in solver to compute the optimal solution.

Visualization:
Display the result using bar and line charts to make the insights actionable and easy to communicate.

Tools and Libraries Used :

PuLP – Formulation and solving of linear programming problems

Matplotlib – Visualization of scheduling output

Python – General-purpose programming and data handling

Business Impact :

Cost Optimization: Reduces total workforce size without sacrificing service levels.

Operational Efficiency: Guarantees sufficient coverage every day of the week.

Scalability: Easily extendable to more complex scheduling scenarios (e.g., part-time workers, different shift lengths, multi-location operations).
