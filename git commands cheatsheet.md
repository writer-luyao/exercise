# Git commands cheatsheet
|Command|Description|
|--|--|
|git add .|Change the files in current directory to staged.|
|git commit -m|Commit the staged files to local repository.|
|git push origin|Push the commits to master repository.| 
|mv A B|Chang the name A to name B
|vi A|Open the file in vi editior. To edit it, press <kbd>i</kbd>. To save the edits and exit vi editor, press <kbd>esc</kbd> to exit the editing mode, and then press <kbd>:</kbd>, then enter <kbd>x</kbd>, and press <kbd>enter</kbd>.|
|rm A|Remove the file A|
|git log|Show the log|
|git log --oneline|Show each entry in one line.|
|git tag -a A -m B|Add a tag A with B as the description.|
|git tag|List all tags|
|git checkout tags/A|Check out tag A.|
|git push origin A|Push tag A.|
|git checkout -b A|Create branch A and move to the branch.|
|git branch|Show all the branches|
|git push --set-upstream origin A|Push branch A to the remote repository.|s
|git branch -d A|Delete branch A.|
|git stash|Create a new stash.|
|git stash list|Show the most recent stashes.|
|git stash pop|Rstore the changes to the most recent stash on the list.|
|git stash save "A"|Save the stash under the name A.|
|git diff A...B|Compare branch A with B|
|git merge A|Merge branch A to the brunch that you are currently on.|
|git clone A|Clone the repository to the location where you are. A is the URL of a repository.|
|git rebase A|rebase your branch to branch A.|


**Note** Git pull is to pull back the remote repository to your local repository. *git pull* covers both *git fetch* and *get merge*.


To keep some files only for local, go to the top level of your local repository, enter the following,  save it as .gitignore, and then push the file to the remote repository.
.gitignore
#Ignore the file notes.text in the temp folder
temp/notes.txt

#Ignore the whole temp folder
temp/

*Ignore all text files in the temp folder
temp/*.txt
