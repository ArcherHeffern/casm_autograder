# Description
Autograder for COSI 131 CASM Problem sets, designed to be used with CASM-Darwin for TA's

# Student Submission Protocol: 
```verbatim
| -- student{n}.zip/
|   	| -- p1.casm
|		  | -- p2.casm
|	  	| -- ps.pdf
```

If doesn't match naming convention, points off and TA will have to manually fix
If doesn't compile -> 0 (You have an interpreter now...)

# File Format
```verbatim
.darwinC/
|	| -- student{n}/
|	|   	| -- p1.casm
|	|		  | -- p2.casm
|	|
|	| -- ...
|
| -- tests/
|	  | -- t1.test
|	  | -- t2.test
|	  | -- ... 
|
| -- results/
```

# COMMANDS
project-init SUBMISSION_ZIPFILE TESTFILES... : Initializes .darwinC
run_tests : Runs all tests on all students. Since running tests is fast, there is no need to more granularity. Outputs results to .darwinC/results.txt
dump_tests : Writes test results to a CSV
view-submissions: Hosts server to view student submissions and shows any error messages if we ran tests. 
