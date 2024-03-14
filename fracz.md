# Open a folder on vs-code and type this in terminal

```
git clone https://gitexercises.fracz.com/git/exercises.git
cd exercises
git config user.name "Jayesh"
git config user.email "jayeshverma1407@gmail.com"
./configure.sh
git start
```

# master
 ```
git start master
git verify
```
# commit-one-file
```
git start commit-one-file
git add A.txt
git commit -m "try-1"
git verify
```
# commit-one-file-staged
```
git start commit-one-file-staged
git commit -m "trying" A.txt
git verify
```

# ignore-them
```
git start ignore-them
touch .gitignore
```
Adding files that are to be igonred in .gitignore
```
git add .
git commit -m "ignored"
git verify
```
# chase-branch
```
git start chase-branch
git branch
git merge escaped
git status
git verify 
```

# git start merge-conflict
```
git merge
ls
cat equation.txt
2 + 3 = 5
git add .
git commit -m "trying-again"
git verify
```
# save-your-work
```
git start save-your-work
git stash
vim bug.txt
git stash pop
git add .
git commit -m "bug-fixed"
git verify
```

# change-branch-history
```
git start change-branch-history
git rebase hot-bugfix
```
