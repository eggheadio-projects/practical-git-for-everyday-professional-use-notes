# [Compare file changes with git diff](https://egghead.io/lessons/tools-practical-git-compare-file-changes-with-git-diff)

## How `git diff` Works

`git diff` shows us the change between two references. The references default to the last commit and the current working directory. We'll see that we can use options to change this default.

## Undestanding `git diff` Output

Each `diff` block that starts with `diff` goes through the sentax changes between our two references. It also tells which references we're comparing. For example `diff --git a/getURLSlub.js b/getURLSlug.js` tells use where comparing two references of the same file (almost like two different versions of the same file).

There will be a some minus and plus symbols.

- `+++` or `---` - refers to a file

- `+` or `-` - refers to a line of code

### Using Options with `git diff`

- `--stat` - Condenses the results and only shows the lines that have been changed and the number of files changed, additions and deletions.

- `--cached` - Shows the difference between the working directory and the staging area.

- `git diff HEAD` - Shows changes between the working directory and the staged changes COMPARED with our last commit. So we see ALL uncommited changes compared with our last commit.

- `git diff {branch}` - We can also specify a branch. This is great for comparing our working directory with a remote branch. `git fetch` your remote branch and then run `git diff origin/master` or whatever the name of your remote branch is.
