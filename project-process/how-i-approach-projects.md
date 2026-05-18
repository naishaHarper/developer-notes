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
Now ask: 
Whos handles: 
- menus
- user input
- program flow?
That is NOT the job of:
- task
- task manager
so we create: Main class
Responsible for:
- starting the program
- showing menus
- taking user input
- calling TaskManager methods

note: We seperate responsibilities because it makes code cleaner, easier to understand, easier to debug and easier to improve. 


STEP 7 (Design the structure) 
Now we know the system needs: 
Task 
Task Manager 
Main 

so the structure becomes: 
task-manager/
├── src/
│   ├── Task.java
│   ├── TaskManager.java
│   └── Main.java
└── README.md

STEP 8 (Build in small steps) 

1. Create Task class
2. Create TaskManager class
3. Create Main class
4. Add menu
5. Add add-task feature
6. Add view-tasks feature
7. Add complete-task feature
8. Add delete-task feature
9. Test and improve

STEP 9 (Test constantly) 
Does this work?
What happens if input is wrong?
Does the output make sense?

STEP 10 (Refractior and improve) 

Once something works we ask: 

Can this be cleaner?
Can naming improve?
Can structure improve?

MOST IMPORTANTLY

thainking like a developer means thinking: 
                                  
What is the problem?
What data exists?
What responsibilities exist?
How should the system be organised?




  
  















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
  
  

  
  

  
