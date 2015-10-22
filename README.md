# GitHub Tutorial

_by Jennifer Mizhquiri_

---
## Git vs. GitHub
Git is a free software developed to help with version control that runs in the command line   
and It helps you keep control of changes by creating a "snapshot" of the code like a photographer.  
Git can be compared to taking a picture of your present at the time code and you can add  
a message to show what you have added,modified or delelted.Git also requires no internet  
and works on your local machine.  
  
  You need to have a git in order to have a GitHub account.Github severs as a place in the cloud  
  to save your code, like an album where your snaps are put together. Unlike git it does not track the changes in code but the visual changes made to  
  the files.Github is also open source which means that anyone can send in code suggestions to change it.  
  Github also is useful for people when they want to work together on the same project because it merges  
  the new parts together to create one project with both changes.Github can run on the command line as   
  well but it also has its own website-->  [Github Website](http://github.com)  
  that people log into to work with repositories and the commits they have made which show
  different visual   
  changes.  
    
  Both offer a basic workflow, but Github allows you to work with another person's repository by using forking,  
  cloning, push and pull which will be expalined later on in the tutorial.
  
  
 


---
## Initial Setup
*  Open up IDE
*  Go to settings
*  Look for SSH Key option, click it  
  * Copy SSH code, should start with  
  `ssh-rsa`  
An SSH Key is a long encryption that serves as a way of identification and doesn't require a  
password, which makes it safer because it isn't open for people to try to guess your password and   
mess with your files.
* Go to [Github](Github.com) Website  
* Click button that says "Sign up" for Github  
  * Insert information (e-mail,username,password etc.)  
  * Confirm account by checking e-mail 
* Look at the top right of the screen on Github.
* Click on your account picture 
  * Click settings
    * on left their is a drop down menu, click on SSH Keys
    * add SSH key give the key a title
* Return to your IDE add the lines of code github gives you, SEPERATLY!!
* Insert `ssh -T git@github.com` to that you connected your IDE with your Github
  * You should see `Hi <username>! You've successfully authenticated, but GitHub does not provide shell access. ` 
* After this you should do `git config --global user.name "First Last" ` which will prompt you to do  
`git config --global user.email email@whatever.org`  
-Doing this allows the changes being added to be put under your name to give you credit for your work



---
## Repository Setup
Once you get through the initial setup, to start git you have to `cd <directory>`  
This chooses what files are being monitered and included in the snapshot.   
You use `git init` to initialize git. Once Git is initialized the directory becomes a   
Repository. To have the repo on Github you have to create a Repo with the same name.  
It has to be IDENTICAL or it will not `push` from your local machine to your remote.  
A remote is helpful to have because you can access your code from any computer and `pull`  
it down to continue working on it, and then `push` it back up, saving the changes.  
Once you have work in your repo you have to do `git add <file name>` which brings   
your work to the stage. The stage is like the prepping place, it sets up your files for  
the 'picture'. Once that's done you can go ahead and do `git commit -m "msg of what you did present tense"`  
and after this you type `git push` if you set a `orgin master` if you haven't then, typing 
```
git remote add origin git@github.com
git push -u origin master
```  
##### What this does is sets up the main repository where all your pushes will go to.
---
## Workflow & Commands 
`git add` is constantly used after changes are made to files and files have to be sent again to the stage
where `git commit` takes another picture that shows the changes.
`git status` helps you monitor what files have been renamed,deleted or modified.
A sample would be 
```
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
```
Once you `comit` changes you can 
`git push` and you can do `git status` inbetween to see the changes. It's an ongoing that doesnt   
have a real order but the options are , add/modify/delete, `git add`, `git status`, `git commit`, `git push` and in some   
cases when collaborating `git pull. 


