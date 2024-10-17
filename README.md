Project Readme Template
Version 1 9/11/24
A single copy of this template should be filled out and submitted with each project submission, regardless of the number of students on the team. It should have the name readme_”teamname”
Also change the title of this template to “Project x Readme Team xxx”
1
Team Name: cdevine5
2
Team members names and netids: Charlie Devine, netID: cdevine5
3
Overall project attempted, with sub-projects: Rewrite DumbSAT to use an incremental search through possible solutions.
4
Overall success of the project: Pretty successful, was able to successfully implement the incrementing function to improve the dumbSAT using various test cases. Obtained reasonable results with varied inputs and the expected curve of the exponential graph. 
5
Approximately total time (in hours) to complete: 8
6
Link to github repository: 
7
List of included files (if you have many files of a certain type, such as test files of different sizes, list just the folder): (Add more rows as necessary). Add more rows as necessary.

File/folder Name
File Contents and Use
Code Files
incrementaldumbSAT_cdevine5.py
Script that implements incrementing into dumbSAT
Test Files
data_test_cases_cdevine5.txt
Test cases varying from 4 to 22 variables, 9 to 32 clauses, 2 or 3 literals per clause, and 10 trials for each.
Output Files
output_resultsfile_cdevine5 
output_tracefile_cdevine5 
output_cnffile_cdevine5
The results file lists the output that the code generates, including problem number, number of variables, number of clauses, literals per clause,  trial number, total literals, satisfiability, time, and assignment. The trace file has similar output, also including the number of unsatisfied and satisfied, the max sat and unsat time, and average sat and unsat time. The cnf file contains data about each cnf with the clauses, variables, and satisfiability for each problem. 
Plots (as needed)
plot_cdevine5.png
This plot displays the number of variables vs execution time for the incremental dumSAT implementation, showing green for satisfied problems and red for unsatisfied. It makes an exponential curve that follows the unsatisfiable points. 



8
Programming languages used, and associated libraries: python, with imported time, random, numpy, and matplotlib libraries. 
9
Key data structures (for each sub-project): This used lists and strings.
10
General operation of code (for each subproject): 

The code starts by parsing a file containing test case parameters (number of variables, clauses, literals per clause, and trial numbers) into a list. It generates random wffs based on these parameters and checks their satisfiability using an assignment incrementing function. The check function evaluates whether any variable assignment satisfies the wff by iterating through clauses and literals. For each test case, the code measures execution time and records the satisfiability results. Finally, it writes these results to output files and plots the data on a scatter plot, showing the difference between satisfiable and unsatisfiable cases, and producing a line of best fit through the unsatisfiable cases.
11
What test cases you used/added, why you used them, what did they tell you about the correctness of your code.

I used a series of test cases to evaluate the correctness and performance of the satisfiability checking code. Initial cases assessed basic functionality with small numbers of variables and clauses, confirming the algorithm's ability to determine satisfiability. As complexity increased, I evaluated performance with larger inputs, seeing if the algorithm could handle more significant problems effectively. Additional cases examined the handling of clauses with different numbers of literals and variables. Overall, these test cases confirmed the code's robustness in accurately identifying both satisfiable and unsatisfiable formulas.
12
How you managed the code development

I managed code development within Google CoLabs. I was able to successfully and efficiently manage all of my development within one notebook and stored all of my input and output files within the same folder in CoLabs.
13
Detailed discussion of results:

The results from the satisfiability checking algorithm demonstrated its effectiveness in determining the satisfiability of the problems across various test cases. The algorithm successfully identified both satisfiable and unsatisfiable wffs, maintaining accurate results even as the complexity increased with more variables and clauses. While execution times rose with larger inputs, especially for unsatisfiable cases, this behavior aligns with the expected complexity of satisfiability problems. The diverse test cases, including different combinations of positive and negated literals, showcased the algorithm's flexibility in handling various inputs. Overall, the consistent performance and correctness across these scenarios indicate the codes’ success, being able to implement incrementing into dumbSAT.
14
How team was organized 

I worked by myself for this project.
15
What you might do differently if you did the project again

If I were to do this project again, I would take more diverse test cases to see how that would impact the performance of the algorithm I developed. Working in a team may have helped streamline the process more efficiently, using a different set of eyes and minds to look over the code and see if any improvements could be made. 
16
Any additional material:


