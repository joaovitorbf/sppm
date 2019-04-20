# sppm: Simple Python Process Manager
A small script to manage your Python processes.  
It creates a permanent list of Python scripts for easy access and management.

It currently lacks features such as stdout/stderr monitoring and the code is pretty ugly, but it works for simple usage!

## Requirements
```
prettytable==0.7.2
psutil==5.4.8
tinydb==3.11.1
```

## Usage
```
Simple Python Process Manager

sppm.py <command>

Available commands:
help - show this help message
start <file/taskid/all> [args] - start the process with optional arguments
stop <taskid/all> - stop the process
restart <taskid/all> [args] - restart the process with optional arguments
remove <taskid> - remove the process from the list
list - list all processes
```

## Example list output
```
+----+----------------+------+---------+-------+--------------------------------------------------+
| ID |      Name      | Args | Running |  PID  |                       Path                       |
+----+----------------+------+---------+-------+--------------------------------------------------+
| 1  |   runtest.py   |      |   Yes   | 13060 |   C:\Users\JoaoVitorBF\Desktop\sppm\runtest.py   |
+----+----------------+------+---------+-------+--------------------------------------------------+
| 3  | runtest_two.py |  2   |    No   |  2744 | C:\Users\JoaoVitorBF\Desktop\sppm\runtest_two.py |
+----+----------------+------+---------+-------+--------------------------------------------------+
| 4  | runtest_two.py |      |   Yes   |  8684 | C:\Users\JoaoVitorBF\Desktop\sppm\runtest_two.py |
+----+----------------+------+---------+-------+--------------------------------------------------+

```
