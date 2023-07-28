# practical assessment

1) Creating and switching to feature branch <br>
   => `$ git checkout -b feature` <br>
   Creating pull-request.html file <br>
   => `$ touch pull-request.html` <br> 
   Adding the file  to the staging area <br>
   => `$ git add . ` <br> 
   Displaying the state of the staging area and working directory <br>
   => `$ git status` <br>
   Commiting the changes <br>
   => `$ git commit -m "adding feature for making a pull request"` <br> 
   Pushing the feature branch to my remote repository <br>
   => `$ git push -u origin feature` <br> 
   Making a Pull request <br>
   => (Web-ui - make pull request) <br> 
   Switching to main branch <br>
   => `$ git checkout main` <br> 
   Merging the Feature branch with the Main branch <br>
   => `$ git merge feature` <br> 
   Pushing the changes to the remote repository <br>
   => `$ git push -u origin main` <br> <br>


2) Creating and switching to new-feature branch <br>
    => `$ git checkout -b new-feature `<br> 
   Creating rebase.html file <br>
    => `$ git touch rebase.html `<br> 
   Displaying the state of the staging area and working directory <br>
    => `$ git status `<br> 
   Adding the file to the staging area <br>
    => `$ git add . ` <br>
   Committing the changes <br>
    => `$ git commit -m "Rebaseing new-feature branch with master branch"` <br>
   Switching to main branch <br>
    => `$ git checkout main` <br> 
   Rebaseing the new-feature branch with main branch <br>
    => `$ git rebase new-feature` <br> 
   Pushing the changes to the remote repository <br>
    => `$ git push -u origin main`<br> <br>
   
   
3) Switching to feature branch <br>
    => `$ git checkout feature `<br> 
   Creating change-commit-msg.html file <br>
    => `$ touch change-commit-msg.html `<br> 
   Displaying the state of the staging area and working directory <br>
    => `$ git status `<br> 
   Adding the file  to the staging area <br>
    => `$ git add . `<br> 
   Committing the changes <br>
    => `$ git commit -m "initial commit"` <br> 
   Pushing the changes to the remote repository <br>
    => `$ git push -u origin feature` <br> 
   Committing the changes <br>
    => `$ git commit --amend -m "changing the commit message"` <br>
   Pushing the changes to the remote repository <br>
    => `$ git push --force origin feature` <br> <br> 
   

4) Switching to feature branch <br>
    => `$ git checkout feature` <br> 
   Creating cherry-pick-file.html file <br>
    => `$ touch cherry-pick-file.html` <br> 
   Adding the file  to the staging area <br>
    => `$ git add . `<br> 
   Committing the changes <br>
    => `$ git commit -m "adding a feature to be cherry-picked"` <br> 
   Displaying the output as one commit per line and copying the commit hash of the commit we want to apply to the main branch <br>
    => `$ git log --oneline` <br> 
   Switching to main branch <br>
    => `$ git checkout main` <br> 
   Cherry-picking the respective commit whose commit hash we copied <br>
    => `$ git cherry-pick f7f9db4` <br> 
   Displaying the output as one commit per line and the output shows that selected commit whose commit hash we copied from the feature branch has been successfully applied to the master branch <br>
    => `$ git log --oneline` <br> <br>
   

 5) Switching to feature branch <br>
     => `$ git checkout feature` <br> 
    Displaying the output as one commit per line <br>
     => `$ git log --oneline` <br> 
    HEAD is pointing to "adding a feature to be cherry-picked" commit message.
    Dropping the respective commit <br>
     => `$ git reset --hard HEAD~1` <br> 
    Displaying the output as one commit per line and the output shows that the commit has been successfully dropped. <br>
     => `$ git log --oneline`

