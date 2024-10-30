
Working Directory ---> Staging Area ---> Remote Directory

| command | Description |
|--|--|
| git reset --soft HEAD~1 | just fix and recommit |
| git reset --hard HEAD~1 | undo everything/no need of last changes |
| git fetch --all --prune | prunes (deletes) references to old branches that deleted from the remote|
| git commit --amend | fix mistakes instantly without cluttering your commit history |
|git stash  | Use `git stash save "description"` to add a description |
|git stash pop  | Use `git stash apply` if you want to apply  |
| git cherry-pick <commit-hash> | bring in individual features from any branch |
| git branch -d <branch-name> |  |
|  |  |
|  |  |
|  |  |



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0MzUyMDI4Niw4MjQ5NDA4OTEsMTM0MT
IzNzA1N119
-->