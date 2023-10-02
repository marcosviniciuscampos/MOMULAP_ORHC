For each instance in its respective folder there are the following files:

FRONT_<INSTANCE NAME>.TXT => In each line of this file are the values ​​of the objective functions of the respective non-dominated solution. The first three values ​​refer to coverage, weighted distance and access equity. The next three bring the same information as the previous ones, but in a normalized way and treating all objectives as minimization. The solutions described in this file compose the set of non-dominated solutions for the refered instance resulting from all executions of the NSGA-II and SPEA2 algorithms.


The next five files follow the same pattern, differing from one another by the way the set of non-dominated solutions is generated.


FRONT_<INSTANCE_NAME>_EXISTING.CSV 			=> Set of non-dominated solutions considering existing mammography units
FRONT_<INSTANCE_NAME>_NSGAII.CSV  			=> Set of non-dominated solutions considering the 30 executions of the NSGA-II algorithm
FRONT_<INSTANCE_NAME>_SPEA2.CSV  			=> Set of non-dominated solutions considering the 30 executions of the SPEA2 algorithm
FRONT_<INSTANCE_NAME>_NSGAII_EXEC_<#EXEC>.CSV 	=> Set of non-dominated solutions for a executuion of the NSGA-II algorithm
FRONT_<INSTANCE_NAME>SPEA2_EXEC_<#EXEC>.CSV 		=> Set of non-dominated solutions for a executuion of the SPEA2 algorithm



The next two files present the results concern to the Hypervolume and Spacing indicators for each execution of each algorithm. In each line, the execution id, the Hypervolume value and the Spacing value are displayed

INDICATORS_<INSTANCE_NAME>_NSGAII.CSV 	=> Hypervolume and Spacing results using NSGA-II
INDICATORS_<INSTANCE_NAME>_SPEA2.CSV 		=> Hypervolume and Spacing results using SPEA2


The solution is described in the follow file:

S_<INSTANCE_NAME>_<ALGORITHM>_EXEC_<#EXEC>_<#SOLUTION>.TXT => That file describes a solution generated in one of the executions of an algorithm for a given instance. 

Its content consists of:

- Objective Functions Values
- Location, Allocations and Idle Service of each mammography unit
- List of cities covered by each mammography unit
- List of mammography units by city
- Coverage of Demand by city



