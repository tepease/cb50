### Project 0

#### Part 0: Git

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

In your command prompt, navigate to your home folder, or directory, by typing **cd ~** and hitting enter

* Create a new directory called 'code' by typing **mkdir code** and enter

* Back in your web browser, from the main page of this git repository, click the top right button **clone or download**, and copy the link exposed

* In your command prompt again, type **git clone *link***, but replace *link* with the link you copied above. hit enter.

Congratulations! You now have your own copy of our repo on your computer! 

* In your command prompt, type **git branch *name-motivation*** where *name* is your first name, and enter.

* Type **git branch** (enter) to see all the *branches* in this *repository*. You're on the *master* branch, but you want to be on your own branch...

* Type **git checkout *name*** wait don't hit enter yet! hit **tab** instead. did the branch name auto-complete? Niice. Now hit enter. 

You're now on your very own branch.

* From a file explorer, open /Projects/0/motivation.txt in any text editor.

* Add another row of underscores, and write a bit about what you're hoping to achieve in the next few months in this course, and save.

* Back in the command line, type **git status** to see some information about what you've done. Some will make sense, some may seem a bit arcane for now.. feel free to ask or look up on your own anything you don't understand!

* Type **git diff** to see the changes you've made

* Type **git commit -am 'Add *name* motivation'** - the '-am' part is known as a flag. 

* Type **man git commit** to see more information about what flags are available for this command. No need to understand them all now. You can type **man** before any command to see the documentation.

* Type **git push --set-upstream origin *name*** and again you can just type the first couple letters of your name before hitting tab, and enter.
 
 You are now a git command line guru. 
 
* Back in the browser git repo, you should now see your branch! You may need to refresh.. Hit the *compare and pull request* button

* You should see a comparison very much like the **git diff** you ran above. If you're satisfied, hit the *pull request* button! 

I'll merge it for you since I own the repo. You're done with part 1!




#### Part 1: Scratch

##### Setup

* Sign up for an account on MIT's [Scratch](https://scratch.mit.edu/) site.

You can use some of these resources to get started, or just dive in if you're a already somewhat comfortable with the concepts.

##### Resources

First, the best resource you'll ever have when programming - [help documentation](https://scratch.mit.edu/help/). 
This can take many different forms, as you saw from the 'man' pages in git. 
Help docs are almost always the most *reliable*, *up-to-date* resource you'll have access to.
In many cases understanding help docs can be a skill all its own... but its a skill worth honing!

Don't worry though, you're not stuck with just the help pages today! You can also use:

* CS50 [video walkthrough](https://youtu.be/697pD31GCZg) from Zamyla 

* [Scratch getting started guide](https://cdn.scratch.mit.edu/scratchr2/static/__95f8025b5d5663c8eca07b96a66ef8d6__/pdfs/help/Getting-Started-Guide-Scratch2.pdf)

##### Requirements

In order to complete this project you'll have 

Your mission is, quite simply, to have fun with Scratch and implement a project of your choice (be it an animation, a game, interactive art, or anything else), subject only to the following requirements.

* Your project must have at least two sprites, at least one of which must resemble something other than a cat.

* Your project must have at least three scripts total (i.e., not necessarily three per sprite).

* Your project must use at least one condition, one loop, and one variable.

* Your project must use at least one sound.

Once finished with your project, click See project page in Scratch’s top-right corner. 
Ensure your project has a title (in Scratch’s top-left corner), some instructions (in Scratch’s top-right corner), 
and some notes and/or credits (in Scratch’s bottom-right corner). 
Then click Share in Scratch’s top-right corner so that others can see your project. 
Finally, take note of the URL in your browser’s address bar. That’s your project’s URL on MIT’s website, 
and you’ll need to know it later.
