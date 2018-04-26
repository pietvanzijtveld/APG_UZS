# Git

## maak branch
Use a separate branch for each feature or issue you work on. After creating a branch, check it out locally so that any changes you make will be on that branch.
- eerst naar master switchen: `git checkout master`
- `git checkout -b new-feature`
- 
## Zie branches
`$ git branch -v`

## push branch
De eerste keer dat je een bepaalde branch pushed moet je ook de tracking opzetten, dus ipv simpelweg `git push` moet je doen:
`git push -u origin new-feature`

## Check of branch weg kan
branches on `git branch --merged` without a * are fine to delete (seen from the viewpoint of *)

## Delete branch
- `$ git branch -d <branch>` to delete a local branch.
- `$ git push -d origin <branch_name>` to delete a remote branch

## Git pull request vanaf command line
Eerst pushen.
- `git request-pull [-p] <start> <url> [<end>]`
https://git-scm.com/docs/git-request-pull
(nog verder uitzoeken)