# [Save uncommitted changes with git stash](https://egghead.io/lessons/tools-practical-git-save-uncommitted-changes-with-git-stash)

## Why and When to Use `git stash`

If we are in the middle of a making some updates to our code but we need to suddenly switch gears and fix a bug for instance, we want to still save our code updates.

We don't want to immediately create a new branch for the bug fixes because that would save our updates to that branch. We want to isolate features and bugs so we don't wanna do that.

We don't want to commit our new updates just yet either since we're not done making them. This is why we use `git stash` to stage our changes without commiting them.

So `git stash` has a very specific use case.

## How `git stash` Works

`git stash` allows us to save uncommitted changes. Before using `git stash` make sure to run `git add -A`.

Once we're ready to get back to our uncommitted changes and continue making updates, we can run `git stash apply`. This will bring back our changes that we made. We can now continue business as usual.

### `git stash apply` conflicts

You might run into conflicts when you run `git stash apply` just like with `git merge`. If the changes we made to our code are in the same place as our `git stash` code, we'll get conflicts.

We fix the `git stash apply` conflicts just like we fix `git merge` conflicts. Follow the same process.
