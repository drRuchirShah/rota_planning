# rota_planning

## Aim
Junior doctors are often expected to rotate departments and hospitals several times a year. Rota and life planning is often beyond their control. They are often arbitrarily assigned to a random rota line that may or may not suit their leave preferences. On top of that they may have mandatory exams and courses they are expected to take that only run on certain dates so need to plan for these. 

This tool aims to assign doctors to a rota line that minimises oncall clashes with leave preferences. This will therefore minimise the number of swaps and adjustments required. 


## Assumptions
This tool makes the following assumptions:
1.	A rota can be simplified into shifts/days where a doctors can not take off, and shifts/days where a doctor can take off or are not working
2.	Doctors input their preference into days they do and don’t want to work- coded as 0 (unavailable) and 1 (available). Their leave preferences do no specify whether it a scheduled non-working day or whether it is a normal shift on which leave can be taken


## Pitfalls
This does not offer the best solution but merely an optimum solution.
There may be other constraints not accounted for- for example minimum staffing levels. 

## Conclusion
This proposes to offer a better solution than current practice which may just be arbitrarily assigning doctors to a rota line with no consideration of their leave requests. 

# How to work this

There are 3 R scripts. Run in this order:
1. create_csv_to_fill
2. import_values
3. hungerian

It relies on a solution called the Hungarian solution. I am no mathematician so please google if you are curious to understand more. 
Create_csv_to_fill creates a csv table which is easy to understand and fill out. A “rota manager” should take charge of completing this however they like with the team. 

For work schedule, 0 = normal shift/or day off, 1 = oncall
Normal shift is any shift where leave can be taken. 1 is any shift where leave can not be taken. This is for the purpose of this algorithm. 

For Doctor preferences, 0 = unavailable, 1 = available to work 

After this run import_values and hungerian (spelling to be corrected)


# Contact
Please give in touch if you have any feedback or would like to help support. The aim is to create a tool that is free to all junior doctors within the NHS. 
This is still work in progress
