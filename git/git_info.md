# Git

## maak branch
Use a separate branch for each feature or issue you work on. After creating a branch, check it out locally so that any changes you make will be on that branch.
- eerst naar master switchen: `git checkout master`
- `git checkout -b new-feature`

## Zie branches
`$ git branch -v`
`git branch --all`

## push branch
De eerste keer dat je een bepaalde branch pushed moet je ook de tracking opzetten, dus ipv simpelweg `git push` moet je doen:
`git push -u origin new-feature`

## Check of branch weg kan
branches on `git branch --merged` without a * are fine to delete (seen from the viewpoint of *)

## Delete branch
- `$ git branch -d <branch>` to delete a local branch.
- `$ git push -d origin <branch_name>` to delete a remote branch

## Achteraf toevoegen tag
- `git tag <tagnaam> -m "commit message" <SHA1ID>`

## LOG commands
#### Wie heeft wat met file x gedaan?
- `git blame <file>`

#### samenvatting file wijzigingen
- `git log --stats`
- `git log --patch-with-stats`

#### status remote
- `git remote -v show origin`
- `git ls-remote`
