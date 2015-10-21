# GitHub Tutorial

_by Jennifer Mizhquiri_

---
## Git vs. GitHub
Git is a free software developed to help with version control that runs in the command line   
and It helps you keep control of changes by creating a "snapshot" of the code.  
Git can be compared to taking a picture of your present at the time code and you can add  
a message to show what you have added,modified or delelted.Git also requires no internet  
and works on your local machine.  
  
  You need to have a git in order to have a GitHub account.Github severs as a place in the cloud  
  to save your code. Unlike git it does not track the changes in code but the visual changes made to  
  the files.Github is also open source which means that anyone can send in code suggestions to change git.  
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



---
## Workflow & Commands-+