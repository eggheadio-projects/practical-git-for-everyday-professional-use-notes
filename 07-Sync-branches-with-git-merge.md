# [Sync branches with git merge](https://egghead.io/lessons/tools-practical-git-sync-branches-with-git-merge)

## How `git merge` Works

When we want to move changes made on one branch to another, we use `git merge`. Based on the changes made, Git determines what typeo of algorithm to use to merge the two branches together.

### Syncing Branches

Once the changes the changes made on your branch are stablr, follow these steps to sync your branches with each other

1. Checkout the branch you want the new features moved to. For example, if you want them to be moved to master, run `git checkout master`.

2. Run `git merge` followed by the name of the branch with the new features. For example, `url-slugs` has new features so we run `git merge url-slugs`.

3. Your code editor will automatically pop up. Just save and close the file.

4. Run `git status` to make sure everything's all good.

5. Run `git push` to move your changes to your remote repo.

## Deleting Branches

If you want to delete a branch, run `git branch -d` followed by the branch name. So, `git branch -d url-slugs`.
