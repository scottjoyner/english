# Freshman CSC NCSU Github Guide
This guide will go over the basic functionality of github starting with logging onto your new account through NC State. This github account is where the majority of your projects will be done in your programing classes. Understanding how this tool works is fundemental to your success in this major. You are probably a CSC 116 or 216 student right now and github is the platform in which all of your projects progress can be stored, tracked, and saved. By the time you are done with this you should have a git repository added to your existing ncsu github account. First make sure that you have downloaded the correct software to get a bash terminal open. 

# User guide on Git and Github at NCSU
This guide will walk you through the steps to installing git on your local machine, logging onto and getting comfortable using basic git functionality including how to store projects, mananage versions, and push new changes to your code. 
Introduction paragraph after the title that describes: (a) the activity that will be completed, (b) why the activity is important, and (c) what prior knowledge may be needed in order to complete the activity. This should be concise and straight-to-the-point.
Description or List of Equipment and/or List of Materials
## Tools
- Git
- Text Editor
- Console (CLI)

## INSTALL NOTES
#### Mac Users
If you haven't installed brew install it now.
Navigate to Spotlight at the top right and type in terminal.
Once you are in the shell you are going to have to type some commands. You may copy and paste, but make sure you understand what you are installing onto your device.
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install git
git --version
```
Expected
```
git version 2.xx.x (Apple Git-113)
```
#### Windows 10 Users
Recomended Downloads
- [Git for Windows](https://git-scm.com/ "Local Git management tool")
- [PUTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html "Latest Release Download link") SSH client to connect to host: remote.eos.ncsu.edu username 
#### Linux Users
- Depending on your distribution the commands will be different refer to [this website](http://linuxbsdos.com/2017/01/23/how-to-install-and-configure-git-on-your-favorite-linux-distribution/ "Git install Guide") for distro dependant configs.


If your task is strictly computer-based, you would have a list of equipment, including such items as any necessary software (including version) and the type of computer required (Mac, PC, Linux, etc.).
    The actual step-by-step directions, separated into tasks.
    Every step should:
### Task List
- [ ] 1. Navigate to [github.ncsu.edu]
![alt text][logo]
[Screenshot_2019-10-07 Build software better, together.png]
- [ ] 2. Login using your ncsu email and password
- [ ] 3. Navigate to your homepage and see what repositories you have. Most likeley there arent any.
- [ ] 4. Create a new repository from the command line and add a file to the repo called README.md

Introduction to the git command
```
$git --help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
```
First we want to create a folder to hold our git repositories
```
cd ~/
mkdir git
cd git
```
Now we are inside of our new directory called git
lets create a new folder called helloworld and move into the directory
```
mkdir helloworld
cd helloworld
```
Now we are finally ready to initialize our git repository.
```
git init
```
This should tell you that you have initialized an empty git repository. 
If you want to see what files were created you can input this command to see the .git directory that was initialized.
```
ls -hf
```
Lets add a new file to this repository to tell people what it is for.
In your terminal you will need to create a new file using a command.
```
// Initializes  the file
touch README.md
// Edit the file using a text editor 
nano README.md
```
Lets add a few lines to the README.md file
```
# Hello World
## <unityid>
Write about your class here.
```
Now save this change and exit your text editor. Next lets add our file to the repository
```
git add README.md
```
Lets write a commit message to tell people what we did
```
git commit -am "Added new README file to repository"
```
Now that we have added our commit message we are ready to push the new git repository to a github account. Entering the git push command will bring up a prompt for a username and password. This is the same as the login you used to access your account online. Git will ask if you would like to store your password, this option is up to you; however, it is less secure.
```
git push
unityid
password
```
Now navigate back to your browser, refresh the page listing your repositories, did you see the new respository helloworld added to your account? Great! you are on the way to learning mroe about git commands.


### Troubleshooting Common Issues
Q: What is my Unity ID? How do I find my password? How to reset password? 
A: Navigate [here](https://oit.ncsu.edu/my-it/unity-credentials/ "Unity Credentials") to find information about your unity id, password and more. 
