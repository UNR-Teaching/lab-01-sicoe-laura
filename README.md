# CS 202 Lab 1 - Linux and Git
This lab walks you through the process of setting up your computer for development, and using Git to manage your program source.


### Learning Targets
* (CORE) I can use Git to manage source code
* I can perform basic operations in the Linux operating system


## Activities for this Lab

1. Choose your dev environment (see below) and work through the install. 
2. Install Git on your machine if it does not already exist
3. Create a GitHub account (if you do not already have one)
4. Accept the assignment in Github Classroom
5. Clone the project to your machine
6. Complete the tasks and associated questions at the end of this document

 **Reference Documents** 
You will find a number of PDFs 
[here](https://webcampus.unr.edu/courses/84308/pages/resources) that cover development environment installation steps and getting started with Github. There is resource page as well on Notion: [CS 202 Resources](https://cosmic-boot-d3d.notion.site/CS-202-Resources-09d01bbb0e8740f5ac8460a0d02a3adb)
> If the link does not work for some reason, look under Pages/Resources on WebCampus

## Setting up Your Dev Environment

**IMPORTANT**: The instructions for installing an evironment are *only* for installing on your personal computer. Do not follow these instructions on a lab computer! If you do not have a laptop with you, reboot the lab computer and choose the Linux option when it reboots. You can then follow the instructions beginning with Github Registation below.

* **If you have the Virtual Box setup you used for CS 135 available, you are ready to go.**

* If not, you have options based on your operating system
   * If you run Linux on your computer natively, you are good to go. Any distro should work for this class.
   * If you own a Mac, you do not need to run Virtual Box, since MacOs is a UNIX based system. You may need to install some additional software such as Git if it is not already on your machine. You could install VirtualBox on the Mac, but it is not necessary.
   * If you are on Windows, you have choices
     * Install VirtualBox and Ubuntu (or other distro), or
     * Use WSL 2, the Windows subsystem for Linux
* Use a docker container running Ubuntu

#### Some Considerations in Choosing a Development Environment
* The TAs can provide you with support for the VirtualBox option on Windows or Mac, or the native Linux option. For other options, you are on your own (although there is not really anything difficult about them)
* The vast majority of the code we write for this class will work on any of the options mentioned
   * There are certain file functions that are very low level that might not work on the Windows WSL or native Mac OS. There are workarounds in most of these cases.

### Setting up Linux VirtualBox

The files you will need to follow to set up Virtual Box are found at
[Files on Webcampus](https://webcampus.unr.edu/courses/84308/pages/resources).
_If the link does not work for some reason, look under Pages/Resources on WebCampus_

## GitHub Registration
You will need a Github account to access assignments, and to upload your solutions. If you do not already have an account, follow these steps:

1. Go to https://github.com/ and click "Sign up for GitHub". 
2. When you are asked for your preferred username, use your last name and first name separated by an underscore (for example, "davis-sara").
3. Complete any required confirmation (emails,etc.)

> Github now requires that you generate a personal access token to access repositories. Instructions can be found here: [Creating a token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token)

## Accepting GitHub Classroom Assignments
You will need to use basic Linux commands for the remainder of this assignment. You can find a Linux cheat sheet on Webcampus [here](https://webcampus.unr.edu/courses/84308/pages/resources).

1. Click [here](https://classroom.github.com/a/5jHH0u65) to accept the assignment in GitHub Classroom. This will create a project in your personal workspace on GitHub. We will be using this approach for all the programming assignments this semester.
2. Clone the project to your computer. You do this by clicking the "Code" dropdown in GitHub as shown in the diagram. ![Cloning](cloning.png). <span id="clone"></span>
1. Open a terminal and create a directory called _cs202_ in a convenient directory like home or Desktop.
2. Change directory (cd) into that directory. Type `ls` to list the directory contents just to ensure that you are in an empty directory. Since you going to have many assignments and labs, create a directory called _labs_ and then `cd` into the labs directory.
3. Type `git clone`, one space, and then paste in the clone URL that you copied from Github and then hit return. If you did not create an access token previously, you will need to do so now. [Creating a token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token)

4. Type return and you should see messages saying that code is being downloaded to your machine. You can now `cd` into the lab directory that was just created.

### Complete the following tasks and answer the questions

1. In a terminal, change directories in the `labs` directory and then into the lab 1 directory that was created when you cloned the project
2. Open a file named `answers.txt` in an editor. You will answer the questions in this section in that file.
3. Type `ls` to view the contents of your lab directory. Now type the command `ls > newfile.txt`. Use the `ls` command again to view the contents of the directory. What has changed? What do you think the `>` in the previous statement did when combined with the `ls` command?
4. Add `newfile.txt` to the git repository using the command `git add newfile.txt`
5. Run the command `git status`. What does it say about `newfile.txt`?
6. Open the file `newfile.txt` in a editor. Add the line "This is my file listing" to the top of the file and save it. Now run the command `git diff`. What does this command tell you about your files and their contents? You will need to type 'q' to exit the diff viewer.
7. Check your answers file to ensure that you have answered all the questions, and then save and close it.
8. Run the git command `git add .`.
9. Run the git command `git commit -m "my first commit"
10. You may encounter what looks like an error message that looks something like this

```
Please tell me who you are. 

Run 
	git config --global user.email "you@exanple.com 
	git config --global user.name "Your Name"

```
Follow the directions by typing in the lines, of course using your own email and name, and then run the git commit command again. 

11. Push your code to Github using the command `git push`

## What to Turn In
In the text entry for this assignment, put your Github username. Go to your Github repository for this lab and copy the clone url as you did in step 2 [here](#clone). Paste the clone URL into the text field on the next line after your github name.

Submit your assignment.









