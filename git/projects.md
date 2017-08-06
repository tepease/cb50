### <a name='motivated'></a> git motivated

Git is an amazingly powerful tool for collaborative creation, known as a Version Control System. 
Like Google Docs, Git allows you to make things together while keeping track of who contributed what - but also WHEN they did it. 
Baked in to that *when* is the power to revert changes to any point in time for the project as a whole or only parts. 
You can do a lot with Git, but a little also goes a long way. 
Let's start by sharing what we want to get out of this course. 

##### Resources 

You may refer to Github's training material, like [this](https://guides.github.com/activities/hello-world/), for learning all about git. 
I'm going to provide step by step instructions for the git commands you need for this project though, so you don't need to worry about that for now if you don't want to.

##### Setup

Note: this project requires the use of your command prompt. Many people find this intimidating at first, but fear not! 
With practice, the lack of a *graphical interface* won't bother you at all. Don't be afraid to ask on Slack if you have any questions.

*If your computer is running Windows* download [Git bash for Windows](https://git-scm.com/download/win)

Open a *command prompt*, or git bash for Windows. The way to do this may vary depending on your operating system. Here's some shortcuts:

Linux: **super + t**

Mac: **cmd + space** to open search, then type 'terminal' and hit **enter**

Windows: open applications, select *git bash for windows*

##### Requirements

In your command prompt, navigate to your home folder, or directory, by typing ```cd ~``` and hitting enter

* Create a new directory called 'code' by typing ```mkdir code``` and enter

* Move into your new code directory by typing ```cd code``` and enter

* Back in your web browser, from the main page of this git repository, click the top right button **clone or download**, and copy the link exposed

* In your command prompt again, type ```git clone mylink```, but replace *mylink* with the link you copied above. hit enter.

Congratulations! You now have your own copy of our repo on your computer! Now go into it

* Type ```cd cb50``` and enter

* In your command prompt, type ```git branch myname-motivation``` where *myname* is your first name, and enter.

* Type ```git branch``` (enter) to see all the *branches* in this *repository*. You're on the *master* branch, but you want to be on your own branch...

* Type ```git checkout myname``` wait don't hit enter yet! hit **tab** instead. did the branch name auto-complete? Niice. Now hit enter. Depending on your unique console, you may not be able to tab complete. If it doesn't work, no worries, but you'll need to type the whole branch name: ```*myname*-motivation``` in the above command.

You're now on your very own branch.

* From a file explorer, open /Projects/0/motivation.txt in any text editor.

* Add another row of underscores, and write a bit about what you're hoping to achieve in the next few months in this course, and save.

* Back in the command line, type ```git status``` to see some information about what you've done. Some will make sense, some may seem a bit arcane for now.. feel free to ask or look up on your own anything you don't understand!

* Type ```git diff``` to see the changes you've made

* Type ```git commit -am 'Add myname motivation'``` - the '-am' part is known as a flag.

* Type ```man git-commit``` to see more information about what flags are available for this command. 
No need to understand them all now. You can type **man** before any command to see the documentation. 
(For Windows users in git bash, you'll have to type ```git commit --help``` instead!)
What do -a and -m do?

**Note** before you can do the next step you'll need to contact me in Slack and let me know you're ready to collaborate in GitHub. Then I can add you as a *collaborator*, and you'll be able to push to this repository!

* Type ```git push --set-upstream origin myname``` and again you can just type the first couple letters of your name before hitting tab, and enter.
 
 You are now a git command line guru. 
 
* Back in the browser git repo, you should now see your branch! You may need to refresh.. Hit the *compare and pull request* button

* You should see a comparison very much like the ```git diff``` you ran above. If you're satisfied, hit the *pull request* button! 

I'll merge it for you since I own the repo. You're done with part 0!



### <a name='stylish'></a> git stylish

We struggled a little last week. This week we're going to struggle a little more. 
Remember not to be hard on yourself if you're struggling! 
Look back at your command history. Did you do everything in order?
Take a break if you're getting frustrated. 
If you come back, leave, and come back a few times and can't make progress, ask a friend or mentor for help. 
Struggling, getting help, and understanding what you were missing is how we learn :] 

We added our motivation previously in motivation.txt.

You may notice that what you wrote there now apprears also in a new file - motivation.md! (from the git/ directory) 
A .md file is the same as a .txt, with the additional feature that a browser *renders* certain character patterns as styling.
Add some flair of your own to your motivation!

##### Requirements

* Check out this primer on [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

* In your console/command line/bash, navigate to your cb50 repository just like you did last week (starts with ```cd ~```, remember?)

* Switch to the master branch, where I merge the latest changes at the origin (```git checkout master```) 

* Run ```git fetch``` so your local repository knows what's going on at the origin repository

* Run ```git status```. Is your master branch up to date?

* If not, pull down the changes with ```git pull origin master```

* Create a new branch for your styling changes. Remember how? Reference the instructions from Project 0 if you're stuck! 

* Now open up projects/1/motivation.md and incorporate 1 or more elements of markdown styling into your motivation

Note that you won't be able to see your changes in a simple text editor - you'll have to push them up to github to see them for now.

* ```git diff``` to make sure no unexpected changes were made to other files being tracked by git.

* Commit your changes to the new branch, with ```git commit -am 'Your commit message here'``` just like before. Explain what changes you made in a few words instead of literally 'Your commit message here'.

* Send your updates up to our origin repository with ```git push origin mybranch-name```

* And then refer to last week's instructions for creating a pull request for me to merge 

Awesome work!



### <a name='artistic'></a> git artistic

Lets go to the git gym and flex our git skills! ᕙ(⇀‸↼‶)ᕗ 

#### Requirements

* Add some text based emoji to emoji.md, and send me a pull request when you're done

In order to do this you'll need to rely on the git workflow we've been starting to establish:

0.  ```cd``` to your repo

1.  ```git checkout master```

2.  ```git pull origin master```

3.  ```git branch my-branch-name```

4.  ```git checkout my-branch-name```

5.  edit and save your files

6.  ```git commit -am 'your commit message'```

7.  ```git push origin my-branch-name```

8.  go to the origin repo in your browser, locate your branch, and create a pull request

If you get any errors that don't make sense, don't suffer - send them my way in Slack!
