A major problem with git revert is with commit id's. Each revert generates anew commit id and the history gets messy. In order to address this we can use 
```
git reset <commit-id where you want to reset>
```
This will remove the changes from the local repo and the staging area not from the working area. This is just a precautionary measure by git.

If you want the changes to be removed even from the working area run the following command
```
git reset <commit-id where you want to reset> --hard
```