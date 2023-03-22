# This is the first Repository on my GitHub
  I am learnig to deal with git and github to be more effecient and more relevvent to work with teams 
  and cooperate with others, and I will let my notes while learning here.

## Important commands to deal with Git:
- git init                                   --> to create a local repository
- git status                                 --> to chech the status of the filea you work with
- git add file                               --> to add a file you have from working directory to ataging area
- git commit -m "put your massage here"      --> to push the file to local reopsitory
- git reset head file                        --> to remove file from the staging area
- git branch                                 --> to show the branches that exist in your repository
- git remote -v                              --> to show the remoteName of your repository
- git push remoteName branchName             --> to push your files to the remote repository
- git pull remoteRepo                        --> to have the copy of the branch with the last edits, and merge 
                                                 the new copy with the copy exists in your local repository
- git config                                 --> to show the configurations of the git & you can edit it as you want

------------------------------------------------------------------------------
## To generate a public key:
1- use the command "$ ssh-keygen -t rsa -b 4096"
2- enter the file you want to save the key in
3- you can enter a password for your key file or you can simply press enter for skiping that
4- after that you open the content of the public key file, you will find it as a file.pub and to open it in the 
   terminal use the command "$ cat file.pub"
5- copy the content of the file and go to GitHub to create a new SSH key by typing the nake of the key and paste 
   the ssh key you copied previously, then click enter to save the kay on your account.

### To make sure that your key is working  
- There are some steps to do that.
   - at first make sure that ssh agent is working by this command "$ eval "$(ssh-agent -s)" "
   - then check if the ssh key is working by this command "$ ssh -T git@github.com"
