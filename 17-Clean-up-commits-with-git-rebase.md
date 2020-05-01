# [Clean up commits with git rebase](https://egghead.io/lessons/tools-practical-git-clean-up-commits-with-git-rebase)

## How `git rebase` Works

`git rebase` combines changes made by several commits into one commit. Follow these steps to successfully `git rebase`.

1. First run `git fetch` and then `git log origin/master`.

2. Run `git rebase -i` followed by the branch we want to rebase off of. The `-i` stands for interactive.

3. Including `-i` wil open up an interactive rebase session. This will list out the the commits that are different between the local branch and the branch we're rebasing off of. Each commit will have the word `pick` in front. To clean up our commits, change the `pick` to match whatever action you want to take.

4. If you want to combine all commits into one, use the `squash` option. Save and close the file.

5. Git will continue the rebase and then take you to a screen where you can type in your new commit message (if you decided to use `squash`).

6. Save and exit the file and Git will finish the rebase.

These steps are specific to rebasing and then squashing your commits. The steps will vary depending on what option you want to use.

If you push to your remote branch, you'll see the rebase reflected in the commit messages.

## Why Use `git rebase`

Using `git rebase` gives us a clean commit history. It's good to use `git rebase` before pushing your commits if you want your commits to be nice and pretty.

## When **Not** to Use `git rebase`

`git rebase` is considered destructive because it **changes** your Git history. So **you shouldn't** use `git rebase` on code that's on the master branch on the remote repo that other developers might be uskng.

If for some reason you have to push code to a pull request branch after rebasing, you have to run `git push -f` to force Git to push the code since you're changing the history on the remote branch.

## Fixing Rebase Mistakes

If you realize you've made a mistake while rebasing, run `git rebase --abort`. This will stop the rebase and take your repo back where you starteed before rebasing.
