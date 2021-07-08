# git-tutorial-asr2021

## What is git?

Git is a distributed version control system. It facilates merging of different source codes from different developers. And codes are distributed among developers. Make a copy of the repository in your local machine and work offline, and then push your changes to the server. 

- Distributed version control system
- Trunk based development
  - Working in different versions simultaneously


Install Git in your PC
- Linux
```shell
sudo apt-get update
sudo apt-get install git
git --version (for checking Git version)
```
- Windows
  - Download Git installer from following link and install
  - https://gitforwindows.org/

Set-up Git in your PC
```shell
git config --global user.name "username" 
git config --global user.email "youremail@domain.com" 
git config --list
	user.name=username
	user.email=youremail@domain.com
```
You can see all the configuration done for your git account from the .gitconfig from you Home directory
```shell
gedit .gitconfig
```
Other commands 
```shell
- git clone (url)
- git branch (check the branch)
- git add (file names) 
- git status
- git commit -m "(committed message) 
- git push -u origin master 
- git remote add origin master (url) 
```

For creating a new branch
```shell
git checkout -b testbranch
git add .
git commit -m "test"
git push origin testbranch
```
For merging with main/master branch
```shell
git checkout main
git merge testbranch
git push
```
