**EXTEND THE SIMPLE SHELL IMPLEMENTED IN HOMEWORK 1 **

**PROJECT OBJECTIVES:** 

Add the following additional functionality to the simple shell program from Homework1:

1. If a command ends with the ampersand (&) symbol the shell must execute the program in
background and return the command prompt immediately after launching the command.

2. You should be able to list all the programs executing in the background using an internal
command jobs. Implement the internal command jobs that will list all programs currently
executing in the background. This should list all processes currently executing in the
background and include the process ID and name of these processes.

3. Provide support to implement the pipe operation in the simple shell. For example:
ps -elf | grep ssh
where ps and grep are two commands and the output from the command ps is provided as
the input to the command grep.

4. You should be able to support more than one pipe operation. For example:
ps -elf | grep ssh | wc -l

5. Note that the pipe operation should also work with I/O redirection. For example:
ps -elf | grep ssh > output.log


**AUTHOR:** Pratyusha Thundena 

**ACKNOWLEGMENT:** https://www.geeksforgeeks.org/implementing-lswc-command/; 
https://www.tldp.org/LDP/lpg/node11.html; http://man7.org/tlpi/code/online/dist/pipes/pipe_ls_wc.c.html

**PREREQUISITES:**

FileZilla 2 (transfer files to ssh client); Doc3.tar;  Linux Terminal (UAB)

**INSTRUCTIONS:**

To compile : gcc -o blazersh blazersh.c

**RUNNING THE TESTS:**

To print output:./blazersh 

**SCREENSHOTS/TEST CASES:**

The first screenshot demonstrated the following command ls: 

<img width="598" alt="Screen Shot 2019-03-31 at 1 02 17 PM" src="https://user-images.githubusercontent.com/46456051/55291494-66c6c780-53b5-11e9-8b5d-1e096e5e8893.png">

The second screenshot demonstrated the following command ls with the ampersand symbol: 

<img width="548" alt="Screen Shot 2019-03-31 at 1 36 27 PM" src="https://user-images.githubusercontent.com/46456051/55291852-16059d80-53ba-11e9-99f0-bc6f5406fb5c.png">

The third screenshot demonstrated implementing internal commands: 

<img width="603" alt="Screen Shot 2019-03-31 at 2 09 25 PM" src="https://user-images.githubusercontent.com/46456051/55292259-cd041800-53be-11e9-9d67-23672b66b78d.png">


The fourth screenshot demonstrated the following commands: ls | sort; ls | sort | wc; ls | sort | wc -l;
ps -elf | grep ssh; ps -elf | grep ssh | wc: 

<img width="761" alt="testcases1" src="https://user-images.githubusercontent.com/46456051/55292072-a3e28800-53bc-11e9-9e32-528ff40c3886.png">

The fifth screenshot demonstrated pipe operation with I/O redirection:

<img width="517" alt="testcases2" src="https://user-images.githubusercontent.com/46456051/55292120-2b2ffb80-53bd-11e9-8947-8c6d5445e37e.png">


**CONTACT ME:**

thundena@uab.edu


