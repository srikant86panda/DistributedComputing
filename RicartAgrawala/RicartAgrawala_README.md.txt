SRIKANT PANDA
ID: 2016HT12588

---------------
FILES INCLUDED:
---------------
ricartAgrawala.c
ricartAgrawala.exe
ricartAgrawala_config.txt
ricartAgrawala_README.txt
ricartAgrawala_snapshot_1.JPG
ricartAgrawala_snapshot_2.JPG

---------------
DETAILED STEPS:
---------------
Sample log (a folder containing 4 log files, out1,out2,out3 and out4)

* Sending and Recieving of messages are done in the same program. So we have to run 
  the same program on as many sites as needed.

* To run say 4 sites, there should be 4 consoles open on 4 different machines. 

* The processes will not start execution until all processes are started. So please 
  make sure that all processes are strated correctly.

* ricartAgrawala.exe is the executable.

* RICART AGRAWALA MUTAUL EXCLUSION - IMPLEMENTATION has the documentation and a brief explanation of the design and 
  implementation of the project. 

* ricartAgrawala_config.txt is the configuration file. Please make sure that the ricartAgrawala_config.txt file 
  is in the same directory as that of ricartAgrawala.c

-----------
TO COMPILE:
-----------
* To compile the program open CYGWIN:
	gcc ricartAgrawala.c -o ricartAgrawala

----------
EXECUTION:
----------
Please make sure that the port number and the machine name given in config.txt matches with
what is given during run time. 

-------
TO RUN:
-------
* To run the program, type 

	ricartAgrawala ID MACHINENAME PORTNUMBER

For eg., ricartAgrawala 1 localhost 4001

Terminal 1
$ ./ricartAgrawala 1 localhost 4001
Terminal 2
$ ./ricartAgrawala 1 localhost 4002
Terminal 3
$ ./ricartAgrawala 1 localhost 4003
Terminal 4
$ ./ricartAgrawala 1 localhost 4004

----------
LOG FILES:
----------
* There are no seperate log files maintained. The output is shown on the cosole.
  At the runtime, the output can also be redirected to another output file or log file,
  one for each process.

FOr eg., ricartAgrawala 1 localhost 4001 > ricartAgrawala_1.log