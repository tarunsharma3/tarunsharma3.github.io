# Phases of Problem Solving

Below is a preview of the kind of questions you may consider for each of the phases of problem solving.

## Problem Modelling
1. What are the most important questions that you should be asking for that particular problem?
2. Based on the answers to above mentioned list of questions, **identify the variables** involved in the problem and **quantify these variables** [Look at it at a coarser granularity]. This exercise should also help you in getting a good grasp of below mentioned points with respect to the problem at hand:
   - Amongst all these variables what are key *input variables* (raw material) and key *output variables* (processed outcomes).
   - How do these variables interplay with each other? What are the allowed operations that can be performed on these variables?
   - For e.g. *d = sqrt(x^2 + y^2)* , where *x* and *y* are the input variables representing the coordinates of the point of interest along x-axis and y-axis respectively. *d* is an output variable and represents the distance of this point of interest from origin. Subset of allowed operations on *x* and *y* that we are using in this example are *exponentiation* (*^*), *addition* (*+*), and *square-root* (*sqrt*).
 
## Survey of Candidate Solutions
1. Is the problem you are trying to solve has been solved by others for a similar kind of problem? Search, and read good books, research papers, etc. to become a knowledgable person in this regard.
2. If multiple candidate solutions are present then narrow down further by looking at "what the numbers look like for those workloads that mimic the kind of workload you would be handling for your particular problem?".
   - Consider, looking at the benchmarking results published for variety of workloads for each of the candidate solution, and/or,
   - Consider, generating synthetic datasets (that mimics the workload of your problem) and evaluate them across the candidate solutions, and/or,
   - Consider non-functional aspects like flexibility, maintainability, evolvability, and community support or vendor support for the candidate solution you have narrowed down.

## Solution Design and Implementation
The obtained candidate solutions may not be directly applicable to your problem. Following are some guiding points that might move you closer to the desired solutions:
1. *Representation Transformation:* The candidate solution identified above may not be directly applicable due to the way information or variables are represented in the given problem. Perform a transformation of the representation of the values you are being given. For instance, for the problem of finding aerial distance between two or more cities in a tour. You might have a black-box module which provided latitude, longitude of both the cities under consideration, returns with a aerial distance value in kilometres. Your task would essentially boil down to representing each city in the tour itenerary with it's latitude, longitude value and supplying to this black-box module to get results. Similar holds true for output variables too, in this case, kilometre to miles conversion. Other examples of transformation of representation may be from "Cartesian Co-ordinate system" to "Polar Coordinate System", "Relational Database Management System" to "Graph-Oriented Databases", etc.
2. *Breakdown into Sub-Tasks:* Divide the problem into simpler and smaller known sub-problems. Design a map of how these sub-solutions obtained from these sub-tasks would lead to eventual solution. Prove that the correctness of the design would lead to desired solution under given or identified constraints. For instance, to obtain distance between 2 coordinates you can treat this overall problem's solution to be composed of sub tasks to take *exponentiation*, *addition* and *square-root*, and combining them to report the result.
3. *Execution:* Take actions as per the design and get the desired outcomes.
