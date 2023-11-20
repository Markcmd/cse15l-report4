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
            bash t<tap>

Time to run vim with ListExamples.java file to fix the bugs ~. L tap give only name for file so I have to type .java and then enter. I notice that cursor at the most top left corner. I don't like to use too many H J K L, extually there will be lots of J. Therefore, I use /index1 which will search the first occurence of the index1. Oh, what I didn't expect is after enter I need to press 9 times <n> to get the exact index1!!!  And then I press e, which will move my cursor to the end of the current word, then "r2" this replace current charater where my cursor at without entering the insert mode. Then :wq save and exit the vim, which stands for write and run, no sorry write and quit! Finally, rerun the test, Yeah ~~~ te

### step 8

![screenshort1](rerun_test.png)

Keypressed: bash<space>t<tab><enter>

### step 9

![screenshort1](addCommitPush.png)

Keypressed: git<space>add<space>L<tap><enter>
            git<space>commit<space>-m<space>"Update<space>ListExamples.java<space>line<space>44<space>index1<space>to<space>index2"<enter>
            git<space>status<enter>
            git<space>push<space>origin<space>main<enter>


            

















