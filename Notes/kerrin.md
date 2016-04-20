# Feb 2nd

the technical term for overwriting someone's important changes is...clobber

distributed version control - when you get together and verbally figure out what to do and who should work on what

git allows anyone to checkout a file - work on the same file at the same time

Mac OS and Windows are graphical shells - it abstracts away the complexity of the program underneath

## key commands for git

    pwd - tells you where you are
    ls - list directory (what's there in the current directory) 
    cd - change directory
    clear - clears screen and puts you back at top
    man - manual + command gives you
    cd .. - go up a directory
    cd ../.. - go up 2 directories 
    mkdir - makes a directory 
    rmdir - removes a directory if it's empty 
    mv - (current name) (new name) - renames 

    
there is actually a hidden folder in the folder where you create a repo 
a lot of the commands we run are repository specific
a repository is a project 
all commits are additive - you're adding to the repository's history 

git add - add files to the "staging area"
git rm - removes file from directory and git
github  is just a place where remotes can be - git and github are actually totally separate thing. github : big, valuable company, git is an open source system. github is hosting for your project repos 

markdown - plain text that allows you to add formatting 


# February 16th

adding a repo to another repo - a sub module, but it's really problematic 

subtrees 


to make changes on repos you find...
clone the repo, push to github, issue pull request

## git fork vs clone

head: reference to the last committ in the current working branch 

untracked files

or fork instead of clone

# Git for Humans Chapters 1-3

Grace Hopper is credited for the term "bugs" related to software after discovering that moth nests were interfereing with the processing of the Harvard Mark II

Checking out a file - just like a library book, no one else can edit that file until you're done with it

cloning will create a new working directory, init a new repo and adds a remote called origin

adding vs committing - adding adds to git's database so that the file may be tracked

branch - a virtual copy of a project within the project where changes can be made freely without affecting the original branch

topic branches - branches with a particular topic or goal separate from master, ie "new homepage"

# Git for Humans Chapters 4-5

remote - copy of a git project that lives somewhere else, another computer, or a service like github

the hub model - each team mate has a shared copy of the project on a server and then clone their own versions which they made changes to and then push to the hub 

git pull - brings down changes from one branch

git fetch - brings down all changes from an entire repo

# Week 4 Reading Notes

Git Workflows

treat the master branch as anything ready to be deployed 

to work on sometihng new, make a new branch for that specific feature, and committ often

open a pull request when ready for a merge

someone else reviews code

push to master

the Gitflow work flow

this is my branch. there are many others like it but this one is mine.
