# C6-GIT-Collaboration

The goal of this activity are to enhance your work collaboration using GIT best practice efficiently.
Activity will be guided step by step, make sure you are following each one of them correctly.

If you have any doubt, please reach mentor and ask for the help.

## What you will experiencing
##### Create git ignore file
##### How to clone, pull, push, commit
##### Do's & Dont's rules working in a team
##### How to work in personal branch
##### How to deliver a task in GIT
##### How to request and do Code Review
##### How to do Rebase operation

## Activity Instructions:

##### STEP 1 - Configuration
- Work in a group consist of 5 people
- Clone this empty project from 
    - https://github.com/AdaGOP/C6-GIT-Collaboration.git
- Create your team repository in GIT and store the project
- Invite your team member to the repository
- Make sure everyone in a team clone the project from the same repository


##### STEP 2 - Define git ignore rules
- Create git ignore file
- Define rules in git ignore
- Push the git ignore file to the repository
- Make sure everyone pull the git ignore from repository
- These are the template that you can customized:
###
.DS_Store

.Trashes

*.swp

*~.nib

DerivedData/

build/

*.pbxuser

*.mode1v3

*.mode2v3

*.perspectivev3

!default.pbxuser
!default.mode1v3
!default.mode2v3
!default.perspectivev3

*.xccheckout

xcuserdata/

xcuserdata/**/*

!xcuserdata/**/xcschemes/*

*.moved-aside
###


##### STEP 3 - Define team member access role and rules
- Define who's the person handle master branch
- Every team member should follow clear and descriptive commit message, sample below:
    - ECEB120 : Implemented Email to Payment store API
    
    Done : 
    - Implement API parameter to store email
    - Implement UI to display alert response from API
    - Implement Logic from response handling
    Action :
    - Need review request from ECEB121, ECEB119

-  Work on your own branch based on ticket assigned to you, make sure naming your branch explicitly to describe the task you were assigned. Sample below on how create our own branch:
    - `git branch ECEB_120_Implement_Email_Payment_API` 
    
    

##### STEP 4 - Now everyone please work based on these task
- Create your own branch and name it based on following task
    - Person 1 -> Create a Button with an action to display alert
    - Person 2 -> Create a Text to display something
    - Person 3 -> Create an Image to display some picture
    - Person 4 -> Create segmented picker
    - Person 5 -> Create simple List to diplay static text
    
- Everyone in a team should create your own branch and name the branch based on the task you have.
- Work your task on your own branch
- Don't forget to commit regularly your work to your local branch to avoid losing it.
- After finish, commit and push your work to your own branch. And make sure do `squash commit` before push it. Sample `git squash commit`
    - git reset --soft HEAD~N
    - git commit -m "explain your commit message properly here, refer to step 3"
`git squash` is useful when you have multiple commit works and you want to push to remote branch without confusion, so instead you store multiple commits it will make your team confuse about what exactly you are working on, you need to squash all your working into 1 single commit.
- Everyone should create a review request / `Pull Request` to everyone in a team to review your work
- Your work need to approved by at least 3 person including the person who incharge as a Lead / Master
- After your work has got approval, Lead / Master will merge your work into `Master Branch`


##### STEP 5 - Standby for any task and make sure your local repository always updated using `REBASE`
- Align your local code base with remote code base using `git rebase` operation
