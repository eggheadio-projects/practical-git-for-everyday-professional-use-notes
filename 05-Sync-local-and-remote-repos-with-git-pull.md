# [Sync local and remote repos with git pull](https://egghead.io/lessons/tools-practical-git-sync-local-and-remote-repos-with-git-pull)

## Pulling Changes from Remote Repos

If you're working on a project with other developers and someone makes a change, you can get those changes on your local repo by running `git pull`.

`git pull` pulls changes from a remote repository onto your local repository. 

This is different from `git clone` because we already have been working with this remote repo and now we our local repo to be in sync with the remote version. `git clone` is used to download repos we've never touched or used.

`git pull` is actuall a combination of the `git fetch` and `git merge` commands.

### git fetch

`git fetch` grabs the latest changes from the remote repo and stores them locally. But it doesn't actually add those changes to our code.

### git merge

`git merge` picks up where `git fetch` leaves off and adds those changes to our code.
