…or create a new repository on the command line

```
echo "# testmerge" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/hello0zai/testmerge.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin https://github.com/hello0zai/testmerge.git
git branch -M main
git push -u origin main
```


how to merge branch

```
git checkout main
git pull
git merge beta/1.0.0/windows
git push
```

To delete a Git branch locally and remotely:

1. Delete local branch

```
git branch -d branch-name
```

If the branch has unmerged changes and you intentionally want to force-delete it:

```
git branch -D branch-name
```

2. Delete remote branch

```
git push origin --delete branch-name
```