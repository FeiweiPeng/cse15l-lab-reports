# Lab Report 3
## Researching Commands
** I chose the find command, and the four options I chose are -name, -atime, -o, and -type.** <br />
** -name ** <br />
1. First Example<br />
The command and output are as follows: <br />
```
$ find ./technical/911report/  -name "chapter-1*.txt"
./technical/911report//chapter-13.4.txt
./technical/911report//chapter-13.5.txt
./technical/911report//chapter-13.1.txt
./technical/911report//chapter-13.2.txt
./technical/911report//chapter-13.3.txt
./technical/911report//chapter-1.txt
./technical/911report//chapter-12.txt
./technical/911report//chapter-10.txt
./technical/911report//chapter-11.txt
```
This command finds all the txt files started with "chapter-1..." in the ./technical/911report/ directory. It is useful because it can sort the files in a folder that match the name we want. <br /> Source: https://www.computerhope.com/unix/ufind.htm.
2. Second Example<br />
The command and output are as follows: <br />
``` 
$ find ./technical/government/Gen_Account_Office/ -name "ai*.txt"
./technical/government/Gen_Account_Office//ai00134.txt
./technical/government/Gen_Account_Office//ai9868.txt
./technical/government/Gen_Account_Office//ai2132.txt
``` 
This command finds all the txt files started with "ai..." in the ./technical/government/Gen_Account_Office/ directory. It is useful because it can sort the files in a folder with the specified name. <br /> Source: https://www.computerhope.com/unix/ufind.htm.
** -atime ** <br />
1. First Example <br />
The command and output are as follows: <br />
```
$ find . -atime -1
.
./gov.txt
./time.txt
./911.txt
```
This command prints out the files in or below the current directory that is accessed less than 1 day ago



