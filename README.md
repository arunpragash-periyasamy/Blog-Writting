# Git-tutorial
#Tutorial about the Git with commands

![1](https://github.com/arunpragash-periyasamy/Git-tutorial/blob/main/Screenshot%20from%202022-12-16%2014-40-41.png)
Git Tutorial in Linux Terminal
Hello, everyone! In this article, we’ll look at how to download or install git in Linux, as well as the basic commands for working with git. Okay, without wasting time, let’s just start learning git.

What is Git![Uploading Screenshot from 2022-12-16 14-42-14.png…]()

Git is a distributed version control system that is used to enable software project development by having multiple independent local copies of the project code. These copies, or branches, are created to maintain a copy of the source code of each version of the project to track our code if any mistake is made in the last update.

How to Install Git in Linux
Open the terminal using taskbar icon of the terminal in Ubuntu.

open terminal in linux using taskbar icon
Open terminal using terminal icon in Taskbar
Or else you can use the keyboard shortcut Ctrl + Alt + T to open a terminal.

opening a terminal in linux
Terminal in linux
To install git, just type the command sudo apt install git and press Enter.

Installing git in linux using terminal command
Installing git in linux using terminal command
Then it will ask you for your password in order to obtain and install git.


enter password to proceed
Just type your password, which is your lock screen password, and press ENTER.


Sometimes it will ask you Y/N with the message just press Y and press Enter. Sometimes it will ask you for that thing.

You can use the command git to check whether or not git is installed after it has been installed.It will display the git command for use, as shown in the image below.


Okay, now that git is installed successfully, Let’s get into the git and work with a file. So that we can work with git using that file, we need to create a file.

Creating a file to work with file in Git
Mostly everyone who likes to work with git is using it to manage their project source code in various file types or various technologies, so I can’t explain all the file types or various project types. But I can try to explain how to work with project source to manage versions of the files and changes to files using the text file type. It is a similar method for working with other file types. Right Just get started with git by creating a file.

Before creating a file, I like to get into the project folder. So I can create a new folder named “Git_Sample.” Use mkdir foldername to create a folder or directory.

Creating a folder in linux
Creating a folder using terminal in linux
To see if your folder has been created, type ls in the command line, which will show the list of folders.


So get into the folder, then type the command “cd foldername”. Here, CD is mentioning the “current directory,” and the folder name is telling the terminal to get into the specific folder.


Before creating the file, we just need to initialise the git in the folder, so we can use the command git init to initialise the git.

Git initialization in the folder
This will initialize the git to that folder
In Linux, use the terminal to create a file by typing touch filename.txt. Here touch is the predefined command to create a file, and filename is the name of the file you provided. Following the filename .txt is the file type, which is a text file, but you can use anything else, such as .java for a java file, .html for an html document, .php for php, and so on.


Creating a new file
We can use the git status command to see what changes have been made to our folder, whether they have been updated or not, what updates have been done previously, and so on.

git status of the folder
git status
In the above snapshot, it shows that we just created a file, but no commit has yet occurred. A commit indicates whether or not we have saved the project to git. And here, the sample.txt file is not tracked by the git.

So we need to make a git commit to track our project or the change made in the project folder. To update our changes in git, it is very simple to use the git add filename command to save the changes in a single file to git. Otherwise, if you want to update all of the files in the folder or project, use “git add .”, which will update all of the files in the folder or project.

Update the changes in git
Update the changes to git
You can also add some notes or comments about the project saved by using git commit -m “write your message here” ,which means that we are adding a message for the recent commit, where -m denotes that message.

git commit message
Commit message
To edit the sample.txt file, I just used the vi editor to show you how git works. You can use any editor, like VS Code, DreamViewer, Eclipse, NetBeans, or any other editor you like, to update your changes in the project using the git commands.

To edit the file using the vi editor, just type vi filename in the terminal, and then the file will open in the vi editor.

Open the vi editor
Open vi editor and change something in the file
I just opened the editor and made some changes to the file to view the status of the changes made in the folder.


File edited in the vi editor
To exit from the vi editor, you can use the ESC key and :x to save the file and exit from the editor.

If you’d like to see what is inside the file, you can print the content of the file using “cat filename.txt”.


Print the content inside the file
Let’s check the git repository status to see if the changes have been detected.

File modified detected in git
File modified detected in git
It shows the message that the file is modified; now you can save the changes to the save point by using “git add” or “git commit -a”.

If you are using “git commit -a” then it will open a commit message box , you can add a commit message and save by CTRL + X


It will notify you of what happened after you commit changes in the terminal.


Here, the commit has the message “This is the message of the commit,” and 1 file has changed, along with 1 insertion in the file.

If you want to see the project’s history, use the “git log” command to see the changes that have been made so far.

I just changed the content inside the file to restore the previous version of the file and let us see the changed content in the file.


The change content will be displayed below, and we will update the “git commit -a” later and restore the previous content in the file. Okay, now just commit the file; later, we will see about restoring.


We just changed the content in the file, but sometimes in the project, we have to commit it with some changes, but it contains bugs or the previous version is sufficient. In this situation, you can restore the previous version using “git restore — staged sample.txt”.


To view the history, just use the command “git log,” and to delete some of the changes to the file. Let me demonstrate how to delete it using id.



Here the ID mentions mixed characters followed by “commit.” I just highlighted. If you’d like to delete the last commit, then you need to select the previous ID for the last commit.

I would like to delete the last commit, so I just copied the previous id for the last commit.

Use the command “git reset id” to delete the commit.


If you do not get it, just see the ID I just copied and used in the command.

I think I just covered the basics of working with git. I used more snapshots for you to understand git. I hope that you can get some idea of how the git command is working and for what purpose.
