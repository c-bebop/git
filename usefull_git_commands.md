## Language Settings
To set your GIT language to (for example) english, you have to put the following line into your .bashrc file and remember to tell your shell updating its source via ```source ~./bashrc```:
```alias git='LANG=en_GB git'```

## Branch Managing

### Deleting a branch local and remote
First delete th branch locally:
```git branch -d branch_to_delete```
Afterwards push changes to origin:
```git push origin :branch_to_delete```
<<<<<<< HEAD

## Miscellaneous

If the repository moved to another location (URL):
```bash
git config remote.origin.url git@bitbucket.org:username/website.git
```
Found at: http://stackoverflow.com/questions/14465326/how-do-i-fix-the-path-of-my-local-git-repo-after-move
=======
>>>>>>> 80f19e70fb0cbb736ff6f17a3d163ba4f0a772a3
