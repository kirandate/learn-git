Let's assume we have two branches: `main` and `f1`. We'll consider a file named `file-1.txt` that exists in both branches.

Here's the content of `file-1.txt` in the `main` branch:

```
This is some content in the main branch.
```

And here's the content of `file-1.txt` in the `f1` branch:

```
This is some content in the f1 branch.
```

Now, let's say you attempt to merge the `f1` branch into `main` using the command `git merge f1`. However, Git encounters a merge conflict in `file-1.txt` because both branches have made changes to it.

When Git detects the conflict, it modifies `file-1.txt` to highlight the conflicting sections. The file might look like this:

``
<<<<<<< HEAD
This is some content in the main branch.
=======
This is some content in the f1 branch.
>>>>>>> f1
```

To resolve the conflict, you would manually edit `file-1.txt` to choose the desired final version. For example, you might decide to combine both changes, resulting in the following resolved content:

```
This is some content in the main branch.
This is some content in the f1 branch.
```

Once you've resolved the conflict, you would save the file and stage it using `git add file-1.txt`. Then, you can complete the merge by creating a new commit with `git commit`.