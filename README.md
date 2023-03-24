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
- use the command "$ ssh-keygen -t rsa -b 4096"
- enter the file you want to save the key in
- you can enter a password for your key file or you can simply press enter for skiping that
- after that you open the content of the public key file, you will find it as a file.pub and to open it in the 
   terminal use the command "$ cat file.pub"
- copy the content of the file and go to GitHub to create a new SSH key by typing the nake of the key and paste 
   the ssh key you copied previously, then click enter to save the kay on your account.

### To make sure that your key is working  
- There are some steps to do that.
   - at first make sure that ssh agent is working by this command "$ eval "$(ssh-agent -s)" "
   - then check if the ssh key is working by this command "$ ssh -T git@github.com"
------------------------------------------------------------------------------
## To make a repository for an existing project you have
- At first, you need to go to the folder you have project files in
- Then, initialize a repository in this folder by using command "$ git init", and you will have the filder .git 
  which contain the configuration file forn the repository
- After that, add and commit the files of the project to the local repository by the usual command we said previosly
  "$ git add file", and "$ git commit -m "put your massage here" "

Congratulations, you have added your project files to local git reository, and now you want to push it to a remote repository, and to do that you need to do some more steps.

- At first, make a new repository on GitHub for example or any website that does the same work
- Then, you need to add a remote repository to the local repository exists and name the branch you work on, and 
  finally push the local repository to the remote.
    - "$ git remote add origin SSH_link_of_your_repository" to add the remote repository to the local one
    - "$ git branch -M master" to name the brach to master
    - "$ git push -u origin master" to push the local repository to the remote
------------------------------------------------------------------------------
To collaborate with others on a repository, You need to know more about pull request
  You need pull request to modify and merge your work with the repository files you work on, and you can collaborate with the team you work on your own project or witl a remote team that open the access to modify their repository.
  And for that you fork the repository you want to modify and work on and add it to your repositpries list, modify the files and solve the issues that you want, and to tell the owner of the repository about your edits and merge it to the original one, you need to pull requeast to tell him about that, and if he approve these edits, it will be merged to the original repository.
  Also, you can push these edits or modifications into the master branch in your account or making another branch to work on something, then push it from the branch you made to the master one.