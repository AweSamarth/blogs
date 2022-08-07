## Git and GitHub for Beginners

# Introduction
As a developer, knowing a version control system is very helpful. Massive organizations use such systems and it becomes necessary for their employees to understand them. If you're trying to contribute to open source then you absolutely NEED to know it! I'm sure you've all heard of GitHub in some way or the other. You may have wondered how it is different from Git, what the prerequisites are, and what basic commands you need to know. In this blog, we'll go over these topics (and more!) in a very simple and easy-to-understand manner. Please feel free to use the Table of Contents to skip to a certain topic. So, without further ado, let's get started!

# What is Git?
![Git-Icon-1788C.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659773398030/iHFoREJAi.png align="left")
Git is a free and open source version control system born in 2005. It is relevant to this day and is definitely here to stay, at least for the coming few years. Using such a system allows us to "capture" the exact state of our files and come back to it any time if we feel like we made some mistakes while changing something there. It also allows us to collaborate with our teammates. We can also see the list of contributors and their contributions, accurate to the last line and to the last character.

### Branches
Branching is one of the most goated 🐐🐐 features of git and is the main reason why companies, organizations and teams use it in the first place. By default, the branch in which we make all our changes is called the 'main' branch. If we want to mess with our code in a separate environment without breaking our code in the main branch, we can create new branches and do what we want there. We can then merge our changes with the main branch as well if we want to. 

# What is GitHub And How Is It Different From Git?

![25231.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659810629218/0edO1dIt0.png align="left")


GitHub is an online platform which allows us to store our code and our git version history on the cloud. A wise man once proclaimed that the 2 are different in the same way as P\*\*n and P\*\*nHub are different. And right he was because that is exactly how it works 😆😆 . GitHub is just a git provider. So it is basically just a service that adds value on top of Git, as may be evident from the name as well. Other examples of Git providers are [BitBucket](https://bitbucket.org/product) and [GitLab](https://about.gitlab.com/)

# Installing Git
Download git for windows from the official site [here](https://gitforwindows.org/). Keep going through with the installation. 

I changed the default editor to VS code instead of Vim. You can use other editors if you feel like doing so. 
![Default editor 2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659776165368/7EYr7M9I-.png align="left")
** I highly recommend changing the default branch name to "main" **
![main branch.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659776027420/3uEjvCC0r.png align="left")

To check if you have correctly installed git, use this command in your terminal

```sh
git --version
```

You should be getting something like this

![cmd.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659776327076/Ctj7BNCxs.png align="left")



# Creating A GitHub Repository
A repository is like a folder in a version control system. If you want to upload your version history and code to GitHub, you need:
- Git on you machine
- A GitHub account
- An Internet Connection (duh)

Here are the steps for creating a new GitHub repository
1. Login to your GitHub account
2.  Click on "New" 
![New.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659791641899/b4boH5d8U.png align="left")
3. Decide a name 
4. Click on create repository

Simple as that!

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659793159932/9O7vHlIxj.png align="left")



# Basic Git Commands

### init
For initializing a git repository in the current directory (specified in your terminal).

```sh
git init
```

### config 
When you start using Git, you'll need to put in a username and an email id (given you didn't change the settings of the setup.
```sh
git config --global user.name "Your Username"
git config --global user.email youremail
```

### add 
After making some changes, we need to add them to git. Once we do this, our changes get recorded in the version history. This adds the changes to the "staging area".

```sh
git add filename
```

To add all the files to the history use "." like so:
```sh
git add .
```
*Notice the space after "add"*

###  restore
To "un-add" the changes that we've made. Here we need to use *--staged* for keeping the changes that we have made to our files.

```sh
git restore --staged filename
```


### commit
This command is put in for finalizing the changes that we have added. We need a message along with this command as well. We use **-m** for writing this message. Here's how we can commit our changes

```sh
git commit -m "write your commit message here, eg. made changes to the header"
```

*Note: -m is one of the many flags that are used in git. Flags are used for providing additional input to a command*

### log
This is used for showing the commit history of the repository. Git log displays:
- the commit's unique, 40 character long hash obtained using SHA (Secure Hash)
- author
- date
- commit message 

```sh
git log
```

###  remote
Now it is time to use the repository that we created on GitHub. 

#### remote add origin 
We need to connect our local repository to the one on GitHub. We can do so by using this command:
```sh
git remote add origin https://github.com/yourusername/nameoftherepo.git
```
#### remote -v
To check if you have indeed added the remote repo as the origin, run git remote with the -v flag
```sh
git remote -v
```
###  push
This is used to "push" our changes to a remote server. In this case we'll use the GitHub repository that we created. We can push our changes to the repo like so:
```sh
git push origin main
```
Here, origin is the remote repository on GitHub and main is the branch that we are working on locally and want to push the remote repo.

###  status
This command is used for viewing all the changes that we have done. It shows the state of the working directory (the current folder you're in and the ones inside it). It shows how many changes need to be committed and how many changes are waiting to be pushed.

```sh
git status
```



### clone
This is used for copying a GitHub repository to our local machine. The one on our machine will be connected to the one we cloned, which means the remote repo is the 'origin' of our local repo. 

```sh
git clone url_of_the_repository
```

### checkout

```sh
git checkout branchname
```
This command can be used to make a new branch and switch to it. If the branch already exists, git checkout just switches to it.



### fetch
It **just shows** the changes that are present in the remote repository but not in the local one. It does not apply the changes to the local repo.
```sh
git fetch
```

### pull
It *retrieves* the changes that are present in the remote repo but not in the local one. It applies the changes to the local repo.

```sh
git pull 
```

### revert
This command can be used for reverting the changes that we have committed. **We have to be very careful while reverting our changes** because if we're reckless about it, things can escalate real quickly as we may end up deleting our files! Always be 100% alert when trying to revert. A simple method of reverting to the state our repo was in before the latest commit is as shown:
```sh
git revert HEAD
 ```
The state of our repo gets restored to how it was before 1 commit but the fact that we had to revert gets recorded in the commit history, once we use git commit after reverting.


# Some Useful Terms And What They Mean
### Open Source
Any software whose code is published online and can be viewed, modified and redistributed by anyone is open-sourced software.


### Fork a Repository
Creating a copy of someone else's repository and storing it in your own account is called forking a repository. You can easily fork open-sourced software, make your own modifications to them and distribute them under a different name. Don't worry, it won't be called stealing because people will always know that it's a fork 😆😆

*For the sake of conserving the spirit of open-source please avoid trying to monetize and / or close-source your forks. Also if you ever think of doing such a thing, do it at your own risk lol. StreamlabsOBS &ast;cough cough&ast; Streamlabs sure paid the price. *

### Pull Request
If you've made some changes to someone's repo, either in a cloned repo (in a different branch) or a forked one, you can request the owners of the repository to merge your changes into their project by creating a pull request. In other words, you are asking them to "pull" changes from your repo and apply it to their branch, hence the name. Here's the process of creating a pull request:
1. Go the the other person's repo
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659806556436/mKIGYLh7v.png align="left")
2. Click on Pull Requests
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659806456401/rGny8MSeu.png align="left")
3. If you have made changes, you'll see GitHub asking you to "compare and pull request". Just click that button
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659806473792/dEn_AqiKA.png align="left")
4. Click on create pull request
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659806536454/BmWP2ESqA.png align="left")

### Contributors
Everyone who has committed changes to a repo is called a contributor to that repo. 

### Owners
The people who have access to the main branch of a repo are called its owners. If you are one of the owners, one thing to remember is that even though you can, you should **never push to the main branch directly** . ALWAYS work in a separate branch and then create a pull request to merge your changes into the main one.

# My (Only) Problem With GitHub
GitHub is an amazing platform, no doubt. The only problem I see with it, as a Web3 developer, is that it is centralized. Though GitHub has always proved to be resistant to censorship, there is not telling when that may change. There are people trying this to solve this problem and one such solution is the Radicle protocol. It also uses git for version control. To see how to use it, head over to @[Olubisi Idris Ayinde](@olanetsoft)'s blog on it [here](https://web3.hashnode.com/how-to-build-and-push-projects-to-a-web3-decentralized-git-hosting-protocol-radicle). Note that it is currently does not support Windows. As much as I want to shift to decentralized solutions like Radicle, there is no denying the fact that GitHub is going to be more useful and relevant for the time-being. It is your one stop solution for finding open source projects and contributing to them. So, make sure you learn it well and put it to good use!

# Additional Resources
@[Kunal Kushwaha](@kunalk)'s [video on Git and GitHub](https://www.youtube.com/watch?v=apGV9Kg7ics), which is where I started (back in January-Feb of this year) as well!


[Git Cheatsheet made by GitHub Education](https://education.github.com/git-cheat-sheet-education.pdf) which you can refer to any time you need a refresher


# Summary 
In this blog we have learnt
- What is Git: a version control system
- What are branches in Git: Feature allowing collaboration without clashes 
- What is GitHub: A platform utilizing Git
- Difference Between Git and GitHub: same as the difference between P\*\*n and P\*\*nHub
- How to install Git: use their official site
- Creating a GitHub Repository: Just click new lmao
- Basic Git Commands: a list of 14 commands
- What is Open Source: Software whose code is openly available
- Fork a Repository: Create a separated copy of someone's repository
- What is a Pull Request and how to create one: Just select the branch you want to merge from and the branch you want to merge in. 
- Who are "contributors" : Everyone who has committed some changes to a repo
- Who are "owners" : People who have access to the main branch of a repo
- My Problem with GitHub: It is centralized
- Additional Resources: 2 helpful links

# Thank You

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1659811137342/1GNvr8fGm.png align="left")
Thank you so much for your reading this blog to the end! I hope you enjoyed and learned something new. I really value and appreciate your time! See you in the next blog 🙋‍♂️🙋‍♂️









