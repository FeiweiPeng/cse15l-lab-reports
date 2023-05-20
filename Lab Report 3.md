# Lab Report 3
## Researching Commands
**I chose the find command, and the four options I chose are -name, -atime, -o, and -type.** <br />
**-name** <br />
1.First Example<br />
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
This command finds all the txt files started with "chapter-1..." in the ./technical/911report/ directory. It is useful because it can sort the files in a folder that match the name we want. <br /> [Source](https://www.computerhope.com/unix/ufind.htm).<br />
2.Second Example<br />
The command and output are as follows: <br />
``` 
$ find ./technical/government/Gen_Account_Office/ -name "ai*.txt"
./technical/government/Gen_Account_Office//ai00134.txt
./technical/government/Gen_Account_Office//ai9868.txt
./technical/government/Gen_Account_Office//ai2132.txt
``` 
This command finds all the txt files started with "ai..." in the ./technical/government/Gen_Account_Office/ directory. It is useful because it can sort the files in a folder with the specified name. <br /> [Source](https://www.computerhope.com/unix/ufind.htm).<br />
**-atime** <br />
1.First Example <br />
The command and output are as follows: <br />
```
$ find . -atime -1
.
./gov.txt
./time.txt
./911.txt
```
This command prints out the files in or below the current directory that were accessed less than 1 day ago. It can be used to find the files recently opened, so we can continue working on it. <br /> [Source](https://www.computerhope.com/unix/ufind.htm).<br />
2.Second Example <br />
The command and output are as follows: <br />
```
$ find . -atime -1h30m
.
./gov.txt
./min.txt
./time.txt
./911.txt
```
By typing "h", "m", and other time units, we can find files that were opened at the specific time slot. This command is finding the files in or below the current directory that were accessed less than one hour and thirty minutes ago. <br /> [Source](https://www.computerhope.com/unix/ufind.htm).<br />
**-o** <br />
1.First Example <br />
The command and output are as follows: <br />
```
$ find ./technical/biomed/ -name "1468*.txt" -o -name "rr1*.txt"
./technical/biomed//1468-6708-3-10.txt
./technical/biomed//rr171.txt
./technical/biomed//rr167.txt
./technical/biomed//rr166.txt
./technical/biomed//rr172.txt
./technical/biomed//1468-6708-3-4.txt
./technical/biomed//1468-6708-3-7.txt
./technical/biomed//rr196.txt
./technical/biomed//1468-6708-3-3.txt
./technical/biomed//rr191.txt
./technical/biomed//1468-6708-3-1.txt
```
Sometimes we may want to find files with several names. This option can find files that satisfy any of the multiple requirements. For this one, we are finding the txt files that start with "1468..." or "rr1..." under ./technical/biomed/ directory. <br /> [Source](https://www.computerhope.com/unix/ufind.htm). <br />
2.Second Example <br />
The command and output are as follows: <br />
```
$ find ./technical/911report/  -name "chapter-1*.txt" > 911.txt
$ find . -name "911.txt" -o -name "Session*.txt"
./technical/government/Alcohol_Problems/Session2-PDF.txt
./technical/government/Alcohol_Problems/Session3-PDF.txt
./technical/government/Alcohol_Problems/Session4-PDF.txt
./911.txt
```
First, we created a txt file called "911.txt". Then, we want to find the "911.txt" file and all the files start with "Session..." under current directory. This command can match files with several names at the same time. <br /> [Source](https://www.computerhope.com/unix/ufind.htm). <br />
**-type** <br />
1.First Example <br />
The command and output are as follows: <br />
``` 
$ find ./technical/government/ -type d
./technical/government/
./technical/government//About_LSC
./technical/government//Env_Prot_Agen
./technical/government//Alcohol_Problems
./technical/government//Gen_Account_Office
./technical/government//Post_Rate_Comm
./technical/government//Media
```
This command prints out all the directories in or under ./technical/government/ directory. It is useful when we want to know what directories are under a specified directory. <br /> [Source](https://www.computerhope.com/unix/ufind.htm). <br />
2.Second Example <br />
The command and output are as follows: <br />
```
$ find ./technical/government/Gen_Account_Office/ -name "ai*.txt" -type f
./technical/government/Gen_Account_Office//ai00134.txt
./technical/government/Gen_Account_Office//ai9868.txt
./technical/government/Gen_Account_Office//ai2132.txt
```
This command prints out all the files in or under the ./technical/government/Gen_Account_Office/ directory and with names start with "ai...", without showing non-regular file types. This can be used when we only want regular files under specified directory. <br /> [Source](https://www.computerhope.com/unix/ufind.htm). <br />





