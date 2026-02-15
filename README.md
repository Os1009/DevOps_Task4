## 1- Launch this command, then Record its Job ID 
  cat /dev/zero > /dev/null &\
  Answer : cat /dev/zero > /dev/null & (7815)
## 2- Use a single command to display detailed information about this process
  Answer : ps -f -p 7815
## 3- Save the full output of this command to a file named process_info.txt 
  Answer : ps -f -p 7815 > process_info.txt
## 4- Change the priority of this cat process between 10 and 15
  Answer : renice 10 -p 7815
## 5- Verify the change by displaying the process's new niceness value. Append 
this verification output to process_info.txt 
  Answer : ps -o pid,ni,cmd -p 5421 >> process_info.txt 
  cat process_info.txt
## 6- Terminate the original cat /dev/zero > /dev/null process using its PID.
  Answer : kill 7815   
## 7- Verify the process is no longer running. 
  Answer :to Verify It's terminated : ps -p 5421


