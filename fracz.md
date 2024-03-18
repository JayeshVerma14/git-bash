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
Used git master to start the master exercise. Then used git verify to check if the exercise has been done.
 ```
git start master  *start git master
git verify
```
# commit-one-file
git add stages changes, preparing them for commit. 
```
git start commit-one-file
git add A.txt
git commit -m "try-1"
git verify
```
After using git reset, all files are removed from the staging area. Next, B.txt is added to the staging area with git add B.txt. Then, git commit -m "Add only B.txt" is used to commit only B.txt with an appropriate message.

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
I created a .gitignore file by running touch .gitignore, then added the following patterns to it: ".o", ".exe", "*jar" to ignore files with those extensions, and "library/" to ignore the "library" directory. After that, I staged and committed the changes. Git respects the rules defined in .gitignore and does not track files or directories specified in it.

# chase-branch
First getting all the list of branches and then merging them.
```
git start chase-branch
git branch
git merge escaped
git status
git verify 
```
On 'chase-branch', I merged 'escaped' using git merge escaped. It was a fast-forward merge, bringing 'chase-branch' up to date with 'escaped'.

# git start merge-conflict
Checking first what is causing merging conflict and then deleting unneccessary lines.
```
git merge
ls
cat equation.txt
2 + 3 = 5
git add .
git commit -m "trying-again"
git verify
```
Resolved a merge conflict in 'equation.txt' by modifying line 1 to '2 + 3 = 5'. After staging and committing the changes, the branches were successfully merged.

# save-your-work
Using git stash to save the work.
```
git start save-your-work
git stash
vim bug.txt
git stash pop
git add .
git commit -m "bug-fixed"
git verify
```
Saved work in progress using git stash, then removed a bug, staged, and committed the changes. Retrieved the saved work with git stash pop, made further modifications, staged, and committed the changes.

# change-branch-history
```
git start change-branch-history
git rebase hot-bugfix
```

Applied git rebase hot-bugfix to merge the commit history of 'change-branch-history' into 'hot-bugfix', effectively appending the former onto the latter.

# remove-ignored
Using git rm to remove files.
```
git start remove-ignored
git rm ignored.txt
git add .
git commit -m "changed"
git verify
```
Executed git rm --cached ignored.txt to cease tracking the 'ignored.txt' file. Subsequently, committed the changes to reflect the removal of tracking for the file.

# case-sensitive-filename
```
git start case-sensitive-filename
git mv File.txt file.txt
git add .
git commit -m "lowercase-done"
git verify
```

Renamed a file using git mv File.txt file.txt and then committed the changes.

# fix-typo
```
git start fix-typo
cat file.txt

```
Correct spelling mistake

```
$ vim file.txt
git add .
git commit --amend -m "Add Hello world"
git verify

```

Staged changes and used git commit --amend to modify the last commit message.

# forge-date
```
git start forge-date
git commit --amend --date="1987" -m "date"
git verify
```
Utilized git commit --amend --date=1987-07-07T20:20:20 to modify the date of the commit. This command opened the commit in the editor with the updated date, allowing me to save the changes.


