# [06- Isolate feature development with git branch](https://egghead.io/lessons/tools-practical-git-isolate-feature-development-with-git-branch)

## Why Branches are Useful

Git branches are great becuase it allows us to develop features on their own. This means that we can make changes and different versions of our project without ruining the whole codebase if something goes wrong.

Once the changes we've made on a branch are finished and we know they're stable, we can merge them into the central branch.

## Creating a New Branch

We can create a new branch by running `git branch` followed by the name of our new branch.

If we want to check what branch we're working on, we just type `git branch` into the command line. The branch we're on will have an asterisk in front of it. If we commit, the changes will be added to whatever branch we're currently on.

![Image of command line git branch](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-isolate-feature-development-with-git-branch/tools-practical-git-isolate-feature-development-with-git-branch-master-checked-out.png?1506025997)

## Switching Between Branches

We can switch between branches by using `git checkout` followed by the branch name we want to switch into.

### `git checkout -b`

`git checkout -b` combines `git checkout` and `git branch` into one. We run `git checkout -b` followed by the name of the branch we would like to create and it creates that branch and switches us into it.

### `git checkout -`

`git checkout -` will switch to the branch we checked out last.