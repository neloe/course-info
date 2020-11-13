---
title: Submitting Assignments with GitHub Classroom
category: assign-info
layout: default
---

If you have not yet [created a GitHub account](/commons/gh_act.html) and [installed GitHub Desktop](github_desktop.html), do so now.

## Getting an assignment

Your instructor should provide a link, which is an invitation link.
You may be asked to log into your GitHub account.

### App Authorization (first invitation ever)
The first time you accept an assignment invitation, you may see a screen that looks like this:

![App authorization](/assets/img/ghcr/appauth.PNG)

Choose the green Authorize GitHub button.  This should only happen the first time you accept an invitation in any course.

### Linking your name to your account (first invitation per course)

If this is the first time you are accepting an invitation in a given course, you will see a screen asking you to Join the classroom.
You will see a list of Identifiers; choose YOUR name from the list (not the instructor or TA/GA).  
If your name is not on the list contact your instructor; they can add you to the roster and you'll choose your name at a later date (or they can manually link your account to your name).

### Accepting the assignment

Continue until you see a screen with a big green button that says "Accept this assignment".  
Click the big green button that says "Accept this Assignment".
Eventually you should see a page similar to

![Assignment accepted](/assets/img/ghcr/success.PNG)

Select the link after it says "Your assignment repository has been created:"; this will lead you to your assignment repository page.

![Assignment repository](/assets/img/ghcr/repo.PNG)

Select the green button that says "Code", then choose "Open with GitHub Desktop".
Your web browser may ask if you want to open that file in GitHub Desktop.
It is a) safe to do so, and b) safe to "Always open these types of links in the associated app".
When GitHub Desktop opens, you should see a window that looks similar to:

![Clone pane](/assets/img/ghcr/github_desktop.PNG)

Do NOT touch the Repository URL.
However, you can change the Local path to wherever you want to work on your assignment.
I would create a folder somewhere that will store all of your GitHub Desktop Repositories.
Click the Clone button.
After loading, you see a window that looks similar to:

![Desktop repo](/assets/img/ghcr/cloned.PNG)

You can ignore this window for now, but we will use this program later.

## Write your Code

Complete the assignment as per the instructions provided by your instructor.

## Submitting your Assignment

After completing the assignment, go back to GitHub Desktop.
It should now look similar to this:

![Unstaged changes](/assets/img/ghcr/changes.PNG)

In the left pane, make sure that all of the files are selected.
In the bottom of that panel, leave a summary of your changes and a more detailed description (if appropriate).
Click the "Commit to master" button.
This creates a snapshot of your assignment (associated with a message) that indicates work you have done.
Congratulations! You've just made a commit to your repository!

Once you have committed your changes, you need to select the "Push origin" button that has appeared in the black toolbar at the top (right most button).
When the task is done, it will change to "Fetch origin".
At that point your assignment is submitted!

### Important

Your assignment has not been submitted until the "Push origin" task has completed.
You can always check to see exactly what has been submitted by going to your GitHub assignment repository page (or refresh it if you didn't close the tab).

### Multiple Submissions (and Commits)

You can commit to master as many times as you want between clicking "Push origin"; committing consists of selecting changes you want to keep, providing a message in the lower left pane, and clicking "Commit to master".
A commit is similar to a save/restore point.  
However, your work will not officially be submitted until you "Push origin".

You can push to origin as many times as you like too; all this operation does is make sure that your code on GitHub matches the code on your local computer.
