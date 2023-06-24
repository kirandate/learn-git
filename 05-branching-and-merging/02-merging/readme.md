* Now you created a branch 
* Switched to it and made some changes and commited to the local repo
* You have to merg the changes in the main/master branch
* To achive that you have to first switch to master branch
```
git switch master
```
* after switching you have to run 
```
git merge <name of the branch>
```
* In our case the name of the branch was f1
```
git merge f1
```
* You just carried out fast forward merge
* In a senerio where there are changes in the master branch and your branch git carries out a three way recursive merge
* On the bright side you need not worry if it a three way recursive merge or a fast forward merge, git automatically does it for you.
* You dont need any other commands apart form the one at the top to carry out a three way recursive merge
* Post your changes you can delete you branch using the command 
```
git branch -d <name of the branch>
```
* In our case the name of the branch was f1
```
git branch -d f1
```