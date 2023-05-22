# Lab Report 4
## Editing From The Command Line
In this Lab Report, I'm going to edit the code from command line and record the keys I pressed in each step.<br />
**Step 4: Log into ieng6** <br />
Keys pressed: `Ctrl-R ssh<enter>`
 ![Image](step 4.jpg)
First, I pressed Ctrl-R to search the command history, and typed "ssh" so I can search the ssh commands with my username I used in the past. Then press enter to confirm the command, and I successfully logged into ieng6. <br />
**Step 5: Clone** <br />
Keys pressed: `git<space>clone<space>Ctrl-V<enter>`
![Image](step5.jpg)
I typed "git clone" and copied and pasted my SSH key(git@github.com:FeiweiPeng/lab7.git) of the lab7 repository from my github to the terminal. Then pressed enter to continue and this repository is cloned to ieng6. <br />
**Step 6: Run the tests**<br />
Keys pressed: `cd<space>lab7<enter>` `bash<space>test.sh<enter>`
![Image](step6.jpg)
First I typed "cd lab7" to move to lab7 directory, so I can run the tests. Then I typed "bash test.sh" to run the tests using the script that is already written with out typing the long commands. A failure occurred after running the test.<br />
**Step 7: Edit the code**<br />
Keys pressed: `vim<space>Shift-l ist<tab>.java<enter>` `/chan<enter>jllxi2<esc>:wq<enter>`
![Image](step7.jpg)
Type "vim" to edit the file in command line, then type "List" and tab to autofill the remaining characters, and type ".java" to finish the file name. In the vim, type "/" to enter the search mode, and search "chan" and enter to move cursor to word "change" in the comment line. Then type "jll" to move cursor to "1" after "index". Type "x" to delete the "1", type "i" to enter insert mode, then type "2" to correct the mistake. After that, use esc to back to normal mode, and type ":wq" to save and exit vim. Thus, the error in the code is fixed.<br />
**Step 8: Run the tests**<br />
Keys pressed: `bash<space>test.sh<enter>`


