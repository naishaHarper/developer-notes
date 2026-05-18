## How i Approach Projects 

notes about how i approach projects...

STEP 1 (Problem Analysis) 

What am I actually building?
What should the system do?
Who is using it?
What problem does it solve?

e.g. 

what is Task manager? 
A system that helps users keep track of tasks 

what should the user be able to do? 
V1:
- add tasks
- veiw tasks
- mark tasks as complete
- delete tasks

note: version 1 should always be SMALL but SOLID. Good developers reduce complexity.


 STEP 2 (Data)

What information does the system need to store?

e.g.
What is a task?
title + completed status

what type of data are these?
string + boolean

STEP 3 (Think about what the thing should be able to do)

What actions should a task be able to preform? 
- mark itself complete
- display its infomation

note: Objects usually have data + behaviour.
  ex.
Task

stores:
- title
- completed status
  
 and can:
- mark complete
- display itself
Thats why task becomes a class

STEP 6 (Think about responsibilities) 

What responsibilities exist in this system? 

R1 - One Task 
A task is responsible for: 
- storing task information
- updating its own status
- displaying itself
This becomes: Task class 

R2 - Managing multiple tasks
Who should manage all the tasks? 
A single task should NOT: 
- manage every task
- delete other tasks
- contol the whole system
This becomes: TaskManager class
Responsible for:
- storing all tasks
- adding tasks
- removing tasks
- showing tasks

R3 - Running the program





  
  















  STEP 3 (Define responsibilities)
  
  What should this part of the system be reponsible for?
  note: this prevents messy code

  e.g.
  
  A task should: 
  - store its own data
  - mark itself complete
  - display its information
 
  TaskManager shoud:
  - store all tasks
  - add tasks
  - remove tasks
  - show tasks
  - manage tasks

  Main should:
  
  

  
  

  
