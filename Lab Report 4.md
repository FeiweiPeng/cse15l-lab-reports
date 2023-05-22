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
![Image](step8.jpg)
Back to the command line, type "bash test.sh" again to run the tests. There shouldn't be any failures as we just fixed the mistake.<br />
**Step 9: Commit and push**<br />
Keys pressed: `git<space>add<space>Shift-l ist<tab>.java<enter>` `git<space>commit<space>-m<space>Shift-" edited Shift-"<enter>` `git<space>push<enter>`
![Image](step9.jpg)
Type "git add" plus the name of the file we just edited, and type "git commit" with option "-m" to add the message "edited", then type "git push" to push the change to my repository. <br />
**Summary**<br />
1. Ctrl-R: search the history of commands used before.
2. git clone: clone the repository.
3. Ctrl-V: paste the text just copied.
4. cd: change the current directory to the directory entered after this command.
5. bash: run the shell scripts.
6. vim: open vim.
7. tab: autofill the rest of the line until there are multiple possibilities.
8. /: enter search mode in vim.
9. j: move cursor one line down.
10. l: move cursor one character to the right.
11. x: delete the character pointed by the cursor.
12. i: enter insert mode in vim.
13. escape: back to normal mode in vim.
14. :w : save the changes in vim.
15. :q : exit vim.
16. git add: add changes or new files to the staging area.
17. git commit -m: commit the changes and add a message.
18. git push: push the changes to repository

