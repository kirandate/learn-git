* When you are working in a real time senirio you dont create a folder and start working in it.
* You clone the remote repo and start working. To clone clone the repo you run the following command
```
git clone < url of repo>
```
when you clone a repo git automatically creates a new additional branch origin/main. You cannot switch or commit in local

* This branch is for tracking only

* origin is a shortend name for original repo url

* The remote branches can be seen using the following command
```
git branch -r
```

* If someone from you team added a new file in the remote repo, you local repo is out of sync with the remote repo

* To get the change from remote to local you have to run 
```
git fetch origin
```

* The branch origin/main moved one commit ahead of your local repo. To sync up main you can run the following command
```
git merge origin/main
```

* Since there is no change in the local repo this will result in a fast forward merg

* If there is a new file added in the local an additional branch will be created. This will result in a three ways recurssive merge

* Instead of running these two commands you can simply run 
```
git pull
```