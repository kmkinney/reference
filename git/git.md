# Git Reference

## What is git
git is a versioning tool
Used for 4 main reasons

## Commands to remember
`git clone <url>`                 
    - clone repository into curr dir
    
`git checkout -b <new-branch>`    
    - create a new local branch
    
`git branch -a`                   
    - list all branches, * on current
    
`git fetch`                       
    - fetches HEAD pointer to new commits
    
`git pull`                        
    - applys current master commits to repository
    
`git push --set-upstream origin <new-branch>`
    - pushes a copy of the branch to the remote
    - need to do this before making a pull request from local branch
    
`git status`
    - check condtion of branch, what needs to be added, what has changed
    
`git commit -m "<your message>"`
    - commits changes that have been added to the origin branch
    
`git push origin master`
    - do this to make a pull request
    
