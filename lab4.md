# CSE15L
## Lab Report 4
### step 4

![screenshort1](login_ieng6.png)

Keypressed: 

            ssh<space><ctrl>+<v><enter>

Use ssh command then copy and paste cs15lfa23iv@ieng6.ucsd.edu and press enter to log into my ieng6 account without entering password.

### step 5 
![screenshort1](clone_sshURL.png)

Keypressed: 
            
            mkdir<space>cse15lLabReport4<enter>
            cd<space>cse15lLabReport4<enter>
            git<space>clone<ctrl>+<v><enter>
            ls<enter>

Make a new directory named LabReport4 to orgazies my files by using mkdir command. Then cd to the new dirctory then use git clone with copying and paste the ssh URL, since I previous generated SSH Keys for GitHub. Finally ls to check whether I succeed. 


### step 6
![screenshort1](run_test.png)

Keypressed: 

            cd<space>lab7<enter>
            ls<enter>
            bash<space>test.sh<enter>

Use cd command get into the new directory that I clone from my github. And then ls to check whether is correct and see if test.sh file is in there. And then run test with bash command. As expected, 1 test fails.

### step 7
![screenshort1](vim1.png)
![screenshort1](vim2.png)
![screenshort1](vim3.png)

Keypressed: 

            vim<space>L<tab>.java<enter>
            /index1<enter>nnnnnnnnn
            er2
            :wq<enter>
      
Time to run vim with ListExamples.java file to fix the bugs ~. L tap give only name for file so I have to type .java and then enter. I notice that cursor at the most top left corner. I don't like to use too many H J K L, extually there will be lots of J. Therefore, I use /index1 which will search the first occurence of the index1. Oh, what I didn't expect is after enter I need to press 9 times <n> to get the exact index1!!!  And then I press e, which will move my cursor to the end of the current word, then press "r2" to replace current charater where my cursor at without entering the insert mode. Then :wq save and exit the vim, which stands for write and run, no sorry write and quit!

Note: Ignore the bash test.sh line in the third code, it is for next step. This might seem obvious, but I mention it just to be clear! It shows I successfully exit from vim mode.

### step 8

![screenshort1](rerun_test.png)

Keypressed: 

            bash<space>t<tab><enter>

Finally, rerun the test, Yeah ~~~ 2 tests are OK! 

### step 9

![screenshort1](addCommitPush.png)

Keypressed: 

            git<space>add<space>L<tap><enter>
            git<space>commit<space>-m<space>"Update<space>ListExamples.java<space>line<space>44<space>index1<space>to<space>index2"<enter>
            git<space>status<enter>
            git<space>push<space>origin<space>main<enter>

Last step! 

I use "git add ListExamples.java" says to git, hey among all the files that I made changes I am gonna commit this file, get ready it for me. Which means  telling Git to stage the file ListExamples.java for the next commit. 

Then I use git commit with option -m and a commit message "..." tell git. Hey, you know that file I told you to get ready with git add? I've done with it and now I want to record this set of changes as an official 'commit'. Wrap up all those changes together, and put a label on them with this message 'Update ListExamples.java line 44 index1 to index2' so that I can understand what these changes are about when looking back

Next git status means, Hey git show me what's going on right now? I want to see which files have changes that I haven't staged yet (with git add), which changes are staged for the last commit (with git commit).

Finally, I use git push origin main, main is my branch name in my github repsoitory, tells make those change to my files in my github repository.



### Works Cited
Me

            after vim edit file , do I need to git add exmaple.txt.  Can I do git commit -m instead ?

ChatGPT

            Yes, after editing a file with Vim (or any other editor), you do need to stage your changes with git add before you can commit them. The git commit -m command requires that the changes be staged first. Here's why each step is important:
            
            Edit the File:
            
            When you edit example.txt in Vim and save your changes, these modifications are only made in your local working directory. Git is aware that changes have occurred, but it doesn't automatically track these changes.
            Stage the Changes with git add:
            
            By running git add example.txt, you are staging the changes you made. Staging is like preparing and packaging your changes for the next commit. It tells Git, "These are the changes I want to record."
            This step is crucial because it gives you control over which changes you want to commit. You might have made changes in multiple files but only want to commit some of them at a time.
            Commit the Changes with git commit -m:
            
            After staging your changes, you use git commit -m "Your commit message" to take a snapshot of those staged changes and add them to your repository's history.
            The -m flag allows you to add a commit message directly in the command line. This message should describe what changes the commit includes and why they were made.
            So, the process is: edit the file in Vim → save changes → stage changes with git add → commit staged changes with git commit -m.
            
            Skipping the git add step and directly using git commit -m won't work if the changes aren't staged. Git won't know what changes to include in the commit.
            
            Do you find this process of staging before committing helpful in organizing and tracking your changes?
            

















