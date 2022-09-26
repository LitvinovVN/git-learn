# Remote Repository: GitHub

## What is remote repository?

Local repositories reside on the computers of team members. In contrast, remote repositories are hosted on a server that is accessible for all team members - most likely on the internet or on a local network.

## GitHub

GitHub is one of the most popular Internet hosting services for software development and version control using Git.

Here is a short manual.

1. Creating an SSH key

* Open Git Bash Here
* Print command **ssh-keygen -t ed25519 -b 4096**
* Input file name
* Input password (you won't see any symbols while inputting)
* Input password again (you won't see any symbols while inputting)

**The result: two files were created. Put them into .ssh folder in C:\Users\Username\ (if there's no such folder then create one).**

Later everytime you work with a new device you should put the "closed" file (the one without an extension) into .ssh folder.

2. Telling GitHub about the SSH key

* Open the ssh file with .pub extension using a notepad and copy all the insides
* Go to GitHub -> Account -> Settings -> SSH & GPG keys -> SSH keys and press NEW
* Input the title and paste the copied ssh.pub insides into Key field
* Press Add

3. Connecting git and GitHub

* Open VScode, bash terminal
* Print command **eval "$(ssh-agent -s)"**
* Print command **ssh-add ~/.ssh/SSH file name**
* Input the password

**Now git is ready for work!**

4. Working with GitHub

* Print command git clone + SSH link to the exact remote repository at GitHub
* Create a new branch
* Do all the things you need to do
* Add and Commit the changes
* Print command **git push --set-upstream origin Name
* Go to GitHub and make a pull request