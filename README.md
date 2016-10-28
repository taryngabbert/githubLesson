## GitHub Lesson

We all know the basics of Git, but when you start working in group projects Git can become much more complicated. That's why it's important to understand how to use Git effectively.


### Branches
Branches are extremely important in working on a project. YOU SHOULD NEVER BE WORKING ON THE MASTER. LET ME REPEAT....

<b> YOU SHOULD **NEVER** BE WORKING ON THE MASTER</b>

... so let's get to learning... In the past we've been used to forking and then cloning down. Now, because we're all working on the same project, we will directly clone down from the same project.

When you clone down, you will automatically be on the **MASTER** branch. But we don't want to stay there...

We can create a branch, which will take your current branch and create a clone. Whatever changes you make there, will stay there, until you're ready to merge them with the master.


First let's create a new repo, call it TestProject.. Do this by going to github and pressing the button "Start a project", follow the command line instructions after that..


NOW, LET'S CREATE A BRANCH...
``git checkout -b [branchName]``

You can always check what branch your on by checking with the command ``git branch``

You will make all of your changes in your branch. You will want to make very component based branches. So, if you're creating a navBar create a branch called navBar complete it, and then **git add, git commit** and then ``git push origin [branchName]``...

### Compare and Pull Request

Want to get your changes from your branch on the master? Time to go to github. There you can compare the differences between the branches and do a pull request.

SOMEONE ELSE FROM YOUR GROUP SHOULD LOOK AT THE PULL AND DECIDE WHETHER OR NOT TO ALLOW THE MERGE.

**YOU SHOULD NEVER ACCEPT YOUR OWN MERGE REQUEST. PERIOD. END. OF. STORY**
After the branch is merged the branch should be deleted on github and locally. Whoever does the merge should delete on github. You can delete it locally by using `` git branch -D [new] ``.

### GIT PULL

Now checkout to your master and then do a ``git pull origin master``, you're master will now be updated with what is on GitHub.




** ACCIDENTALLY COMMIT ON MASTER? ** Sometimes it happens, but we can fix it. Do a ``git reset`` this will un-commit everything since your last push/pull. Then switch to a branch. The branch will have your changes and then you can commit and push to master.

You may have a little bit of difficulty getting the pull from master, but it can be done with a ``--force``.

This may not make complete sense now, but know that if you encounter this problem let one of us know and we will help you out.



#### Recommendations

1. Only work on branches!!!!!!!!!!!!!!!!!!!
2. Don't let your master get behind... pull when people merge...
**Don't go lone wolf**
3. Do not, do not, do not, **ever** merge your own branch.
4. Communication, keep it open. Let people know when you may be working on something that could create a conflict. 
