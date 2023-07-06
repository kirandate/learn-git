We all make mistakes. One of the major advantage of using git is that we can roll back using simple git commands

Suppose we have 4 lines added in a file with different commit id's we can run the below command to see the log
```
git log --oneline
```
To revert a particular commit we run 
```
git revert <commit-id>
```
It will open up the console just press ":q" to save

We can revert multiple commits by running
```
git revert <parent commit> .. <latest commit>
```
