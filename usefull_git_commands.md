## Language Settings
To set your GIT language to (for example) english, you have to put the following line into your .bashrc file and remember to tell your shell updating its source via ```source ~./bashrc```:
```alias git='LANG=en_GB git'```

## Branch Managing

### Deleting a branch local and remote
First delete th branch locally:
```git branch -d branch_to_delete```
Afterwards push changes to origin:
```git push origin :branch_to_delete```
