Lets first create new branch
```
git branch f1
```
switch to the new branch
```
git switch f1
```

add few commits int the f1 branch

while we make the changes in the f1 branch there could be a possibility that there are new releases in the main branch

To mimic this we will switch to our remote repo and add a new file to the main branch

we need to switch to the main branch and pull the changes from the remote repo

```
git switch main && git pull origin main
```

At this point if we run the command `git rebase f1` this will insert the commit id's in between the existing commits and when we try to push our code in the remote repo it will throw errors

To avoid that we need to switch to `f1 branch` and rebase the main

```
git switch f1 && git rebase main
```

Now we need to get these changes to the main branch as well, to achive that we need to switch to the `main branch` and rebase again

```
git switch main && git rebase f1
```

To see the changes we can run

```
git log --oneline
```
