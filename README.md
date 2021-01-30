How to remove node\_modules and prevent it from being pushed again after an accidental push


#### Instructions

1. Create a .gitignore file if it doesn't exist already

`touch .gitignore`

2. Add the line `**/node_modules` to the .gitinore file to prevent tracking  
_The `**/` a file or directory listed after the slash from being tracked no matter where it is in the repo_

`echo "**/node_modules" >> .gitignore`

3. Remove the currenty tracked node\_modules 

`git rm -r --cached node_modules`

4. Add .gitignore 

`git add .gitignore`

5. Commit now that nodei\_modules has been removed

`git commit -m "removed node_modules and added it to the .gitignore"`

6. Push the changes

`git push`


#### Hooray!!!
