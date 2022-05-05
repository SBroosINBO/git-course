---
description: "Git collaborative workflow for Rstudio"
title: Workflow Rstudio
output:
  html_document:
    toc: true
    toc_depth: 2
    toc_float: true
---

------------------------

# BEFORE I START WORKING

------------------------

## STEP 1: Update your code

**Choose your option:**

### OPTION 1A: *I'll make a new branch to work with*  
Create a new topic branch from main

Make sure you are working on the main branch:
![](./static/images/workflow_rstudio_1.png)

Update the main branch to make sure it is aligned with the remote main: Click `Pull`:
![](./static/images/workflow_rstudio_2.png)

Create a new branch: click on `New branch` and fill in a branch name:
![](./static/images/workflow_rstudio_2b.png)

### OPTION 1B:  *I already have a branch I want to continue working on*:  

Switch to existing topic branch:
![](./static/images/workflow_rstudio_3.png)

Update the topic branch to make sure is is aligned with the remote main: 
In the Git shell, type:
```
git pull origin main
```
![](./static/images/workflow_rstudio_4.png)


------------------------

# WHILE EDITING

------------------------

## STEP 2.x: adapt in md, R-code,... (multiple times!)

### Add new files

Stage the new file with checkbox and click `Commit`
![](./static/images/workflow_rstudio_5.png)

Provide clear and understandable message about adaptations
![](./static/images/workflow_rstudio_6.png)

### Change files:

Stage the adaptations with checkbox and click `Commit`
![](./static/images/workflow_rstudio_7.png)

Provide clear and understandable message about adaptations
![](./static/images/workflow_rstudio_8.png)


## STEP 3: Push your changes to GitHub.

Update the remote version of the topic branch. Click `Push`:
![](./static/images/workflow_rstudio_9.png) 

------------------------

# EDITS ON BRANCH ARE READY

------------------------

## STEP 4: Pull request to add your changes to the current main. 

Update the remote version of the topic branch. Click `Push`:
![](./static/images/workflow_rstudio_9.png)

Go to your repo on Github.com and click the `Compare & pull request` button. 

![](./static/images/workflow_rstudio_github_1.png)

Add information about the Pull request, add reviewers, labels,... Finally, `Create pull request`:
![](./static/images/workflow_rstudio_github_2.png)

## STEP 5: Code review!

You and collaborators can make comments about the edits, review the code and adapt if required (create additional commits and `Push` them to GitHub) .

If everything is ok, click the  `Merge pull request`:

![](./static/images/workflow_rstudio_github_3.png)

followed by `Confirm merge`:

![](./static/images/workflow_rstudio_github_4.png)

Delete the online branch after merge, since obsolete, click `Delete branch`

![](./static/images/workflow_rstudio_github_5.png)

## STEP 6: Update the main branch on my PC

Make sure you are working on the main branch:
![](./static/images/workflow_rstudio_1.png)

Remove the local branch, since obsolete. In the Git shell, type:
```
git branch -d analysis-script
```
![](./static/images/workflow_rstudio_4.png)

Update the local main branch: Click `Pull`:
![](./static/images/workflow_rstudio_2.png)
