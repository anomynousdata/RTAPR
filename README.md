## Replication Package

This repository contains the replication data and relevant descriptions. 

    .
	|-- AllData 
		|--  APR_source_code
		|-- Subject_name.json.tar.gz 
			|-- each tool 
			    |-- i_CLASS
			    |-- i_METHOD
			    |-- i_STATE
			    |-- i_NORTS

 *AllData* is the root directory, and it contains the results of all 12 studied APR tools as shown in the following table.

| Category      | Tools |
| ----------- | ----------- |
| Heuristic | Arja, GenProg-A, Kali-A, RSRepair-A, SimFix |
| Template   | AVATAR, FixMiner, kPar, PraPR, TBar|
| Constraint   | ACS, Dynamoth |

For the subjects, we include the results of six Subjects (e.g., Lang, Math, Mockito, Time, Chart, and Closure). 

For each subject, e.g., *Lang*, it contains 4 items for each buggy version i, i.e., i_CLASS, i_Method, i_STATE, and i_NORTS. They represent the patch execution information with different RTS strategies (i.e., Class-level, Method-level, Statement-level RTS, and without RTS). 


For each item, it has 8 columns of data items, which are seperated by commas:
* 1st column means the unique identifier for each patch: patchid + "-" + package name + ":" + class name + ":" + line number
* 2nd column means the patch categoery: including Stop_P, Stop_F, Plausible
* 3rd column means the number of executed failed tests in partial matrix 
* 4th column means the number of executed passed tests in partial matrix 
* 5th column means the number of executed tests in partial matrix 
* 6th column means the number of executed failed tests in full matrix 
* 7th column means the number of executed passed tests in full matrix 
* 8th column means the number of executed tests in full matrix 
