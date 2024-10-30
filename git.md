
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
| git branch -d <branch-name> | delete the branch |
| git branch -D <branch-name> | if you need to force-delete a branch |
| git log -- <file> | certain changes were made over time |
| git blame <filename> | way to track down who made a change and when, especially when debugging issues |
| git merge --abort | quick exit from a tricky situation |
| git log --grep="search term" |  |
| git log --author |  |
| git tag -a v1.0 -m "Version 1.0 release" |  |
| git clean -fd |  |
| git reflog |  |
| git bisect start 
  git bisect bad 
  git bisect good <older-commit-hash> |  |



<!--stackedit_data:
eyJoaXN0b3J5IjpbOTA2Mzc4NTk0LDYxOTI0MDMxNiw4MjQ5ND
A4OTEsMTM0MTIzNzA1N119
-->