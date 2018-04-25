# Git

## maak branch
Use a separate branch for each feature or issue you work on. After creating a branch, check it out locally so that any changes you make will be on that branch.
- eerst naar master switchen: `git checkout master`
- `git checkout -b new-feature`
- 
## Zie branches
`$ git branch -v`

## Check of branch weg kan
branches on `git branch --merged` without a * are fine to delete (seen from the viewpoint of *)

## Delete branch
- `$ git branch -d <branch>` to delete a local branch.
- `$ git push -d origin <branch_name>` to delete a remote branch