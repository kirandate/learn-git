#A realtime senario that happens a lot in the real time projects

* Lets say you have a remote repo with main branch and branch for release 1.01

* Now you clone the repo and create a new branch 
```
git branch 1.02 origin/1.01
```

* You can switch to the branch using 

```
git switch 1.02
```

* Now you commit changes to the new branch 1.02 and you say I am all set I can push it to the remote repo.

* If you try to push it to the remote repo it will throw an error

* You have to run the command 
```
git push origin HEAD
```
