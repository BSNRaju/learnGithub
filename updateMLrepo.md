# Updating files in forked introml repo and creating pull request to original repo

I provide step-by-step explaination for making changes and updating the forked repo and then contributing back to Prof. Rangan's repo by creating a pull request. 

Note: Students can also provide the [feedback using these instructions](https://github.com/ishjain/introml#feedback) without forking the original repository.

## 1. Updating files in forked introml repo

Prereq1: Access to Git Bash

Prereq2: You forked the introml repository and cloned it on your local machine (e.g. `git clone https://github.com/`**`ishjain`**`/introml.git` ) Note that I used my GitHub username **ishjain**, which you must replace with your own username (not sdrangan, nor yaowangatpoly).

Prereq3: Basic configuration of name and email address is done using Git Bash command line. E.g. 
```
git config --global user.name "Ish Kumar Jain"
git config --global user.email "ish***@gmail.com"
```

Check the configuration using command `git config --list`


**Note:** A good introductory [tutorial video](https://www.youtube.com/watch?v=uR6G2v_WsRA) (30 min) by David Mahler.
It explains basics of GitHub like creating/cloning a repository, basic commands (git add and git commit), 
and checking status and commit history (git status and git log). I recommend this video to anyone new to the GitHub environment.

Now, suppose you made some changes in the files or created new files. Follow these steps to update the online repository.

### Move to the introml directory
```
cd introml
```
Note that you may need to provide a full path to the introml if introml folder is not in the same directory. check the current working directory using `pwd` and use command like `cd \path_to_intoml\introml`, with `path_to_introml` replaced by the path to the introml folder cloned using your own forked repository.
### Check the status
```bash
git status
```
![alt text](https://drive.google.com/uc?id=1g76LSEzOu7t_PMj1A3-GTK0VGYvic_5_ "Title") 

It says there is one untracked file and suggests using `git add` command.

**Note:** You can also see the difference/changes inside all the files using `git diff` command.
### Adding the file to staging area
```
git add .
```
Note the dot at the end (It is part of the code). This command will add all the new files to the staging area. To add any specific file use `git add filename.pptx`. 
Now check the status using `git status`.

![alt text](https://drive.google.com/uc?id=1k5nmQNfe7o3tSCsX8olInJigZb6tQWnm "Title")

It says the changes need to be commited.

### Commiting changes
```
git commit -m "Modified Lecture-1 slides"
```
You can give any reasonable message for making the commit.

![alt text](https://drive.google.com/uc?id=15FGokqHfTQHhpsLnAHxibC_WG1h7BRgH "Title")

Check the status again: `git status`

![alt text](https://drive.google.com/uc?id=1EAOe49C7XljKPJaVpHe46osISD-roG-r "Title1")

#### Optional: Checking the commit history
```
git log
```
![alt text](https://drive.google.com/uc?id=17qmKda0v9WI0wcXSmqQe66u7cCB_tTy7 "Title")

In order to exit use `Shift + Q` key.

### Push the changes to the online repository
```
git push -u origin master
```
![alt text](https://drive.google.com/uc?id=11jka7HcULUMlAekJqhnXValoZBN4YO1L)

It may ask you to login to your github account for the first time. After this, you can see the changes in the online github repository.


## 2. Creating Pull Request to Prof. Rangan introml repo

Go to your GitHub page. E.g. https://github.com/ishjain/introml and click on Pull Request

![alt text](https://drive.google.com/uc?id=1K9Rjqkmk9oCp6ba1rRbp46IHCV6-gnkv)

See the changes and confirm the Pull Request. Prof. Rangan can then be able to merge this pull request to his original repository.

![alt text](https://drive.google.com/uc?id=1A7zChKRTin8Sq0KVQRJrbY7TyFmKpQJv)

## 3. Syncing your forked repository
In case Prof. Rangan makes any changes in his original GitHub repo, you can apply those changes to your forked repo 
using [this tutorial](https://help.github.com/articles/syncing-a-fork/) on syncing a fork. 
It basically downloads all the new commits made in the original repo (by Prof. Rangan) 
to a new branch called 'upstream/master' in your repo and merges this branch to your master branch.

Again [this Part-2 tutorial video](https://www.youtube.com/watch?v=FyAAIHHClqI) (30 min) by David Mahler on 
creating and merging branches is very useful.



