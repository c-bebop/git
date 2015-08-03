## Undo Changes 

### Unadded changes

If you've made unintendet changes and you did not add them for the next commit, you can do the following:

```bash
git checkout <file>
``` 

### Already commited changes

There is no 'good' way to undo changes that have already been commited due to the fact that by undoing commits we would change the history of the repository (and changing history is never a good idea). What can be done is to revert the commit which initialises a new commit with all the reverted changes:

```bash
git revert <commit_hash>
```

There is a good article about this topic: http://christoph.ruegg.name/blog/git-howto-revert-a-commit-already-pushed-to-a-remote-reposit.html

## Language Settings
To set your GIT language to (for example) english, you have to put the following line into your .bashrc file and remember to tell your shell updating its source via ```source ~./bashrc```:
```alias git='LANG=en_GB git'```

## Branch Managing

### Deleting a branch local and remote
First delete th branch locally:
```git branch -d branch_to_delete```
Afterwards push changes to origin:
```git push origin :branch_to_delete```

## Miscellaneous

If the repository moved to another location (URL):
```bash
git config remote.origin.url git@bitbucket.org:username/website.git
```
Found at: http://stackoverflow.com/questions/14465326/how-do-i-fix-the-path-of-my-local-git-repo-after-move