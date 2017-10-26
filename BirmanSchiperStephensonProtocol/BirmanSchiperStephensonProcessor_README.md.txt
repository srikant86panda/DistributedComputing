Name: Srikant Panda
ID: 2016HT12588

--------------
File Contents:
--------------
1. birmanSchiperStephensonProcessor.c: Source file
2. birmanSchiperStephensonProcessor.exe: Executable
3. birmanSchiperStephensonProcessor_README.txt: Read me
4. birmanSchiperStephensonProcessor_SNAPSHOT.jpg

---------------
DETAILED STEPS:
---------------
Assuming 3 processor in the system
1. Open 3 instance of birmanSchiperStephensonProcessor.exe.
	2. On terminal 1 enter 3 in  (Enter Total Number Of Processes (max 99):)
	3. Enter 0 in (Enter Process Id of Current Process (should be 0 to 2))
	4. Enter port of process 0 (ex. 4000) in (Enter (Procees-0) Port To Recevice Brodacast Message)
	5. Enter port of process 1 (ex. 4001) in (Enter (Procees-1) Port To Recevice Brodacast Message)
	6. Enter port of process 2 (ex. 4002) in (Enter (Procees-2) Port To Recevice Brodacast Message)
7. Repeat steps 2 to 6 on remaining two terminals (except change the value of process id in step 3,  terminal-2 : 1, terminal-3: 2)
8. Enter something on any one of the terminals to initate the brodacaste message

Each process having some delay to send message to other processes, this will be shown in the output window  'Channel Delays to Process 0 to 2 ----> 0,4,7
ie. p1-p1 = 0 delay
	p1-p2= 4 seconds
	p1-p3 = 7 seconds

when p1 sends message to p2 and p3, p2 gets the message first and p3 second. Once p2 gets message and itself sends message to p3,p1 then p3 first gets the message from p2 and p1 gets. If p3 gets message from p2 before its receive message from p1 then p3 puts the p2 message in buffer, after that whenever p3 receives message from p1 then it delivers both buffered and received message to process

-----------
TO COMPILE:
-----------
* To compile the program open CYGWIN:
	gcc birmanSchiperStephensonProcessor.c -o birmanSchiperStephensonProcessor

-------
TO RUN:
-------
* To run the program, type 

	Double click on birmanSchiperStephensonProcessor.exe