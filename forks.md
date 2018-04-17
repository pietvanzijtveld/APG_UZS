# Forks

When a repo is cloned, it has a default remote called `origin` that points to your fork on GitHub, not the original repo it was forked from.
To keep track of the original repo, you need to add another remote named `upstream`

`git remote add upstream git://github.com/user/repo.git`

You will use upstream to fetch from the original repo (in order to keep your local copy in sync with the project you want to contribute to).

`git fetch upstream`

(git fetch alone would fetch from origin by default, which is not what is needed here)

You will use origin to pull and push since you can contribute to your own repo.

`git pull`
`git push`

(again, without parameters, 'origin' is used by default)

You will contribute back to the upstream repo by making a `pull request`.

![local-origin-upstream](https://i.stack.imgur.com/cEJjT.png)

## Workflow with forks
[collaborative github flow](http://www.eqqon.com/index.php/Collaborative_Github_Workflow)

![setup](http://www.eqqon.com/images/a/a0/Distributed_repository_structure_on_github.png)
*******
![flow](http://www.eqqon.com/images/f/fc/Update_distribution.png)