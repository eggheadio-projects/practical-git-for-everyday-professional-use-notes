# [Capture code history snapshots with git add/commit/push](https://egghead.io/lessons/misc-practical-git-capture-code-history-snapshots-with-git-add-commit-push)

## `git status`

When we want to know whether or not our files have been added to the staging area or if we have any files to commit, we use `git status` to check this.

If running `git status` tells us that the working directory is clean, that means that no changes have been made.

If we do make a change, running `git status` will tell us that out changes are not staged to for commit.

## `git add`

We run the `git add` command when we would like to stage our changed files. We type `git add` followed by the name of the repository we would like to add.

### `git add -A`

Running `git add -A` will add all the files we've changed. This means we don't have to repeatedly add individual files.

## `git commit -m`

We use `git commit -m` to commit everything in our stagin area. We follow this command with a short message that summarizes what the purpose of the commit is. 

[Read this helpful article on commit messages](https://dev.to/yvonnickfrin/a-guide-on-commit-messages-d8n) if you want to know how to make great commit messages.

```bash
git commit -m "Add a missing bracket"
```

## `git push`

When all changed files have been added and commited, you can run `git push` to push those changes to the remote repository you're working with.

## Staging Explained

The term 'staging' was mentioned a lot. I found this hard to understand at first. But I like to think of it as an actual stage during a show or play or something like that.

When a change has been made to a file but it hasn't been added using `git add`, it's like an actor who's about to be on but isn't backstage yet.

Using `git add` to add a file to the staging area is like the actor finally making it backstage. They're in the staging area and almost ready to perform.

When we `git commit -m`, the actor is just about ready to go on stage. They're reading over their lines (the commit message) to make sure they know exactly what they're gonna do unstage. No fumbles or confusion!

Finally, `git push` is when the actor is finally on stage doing their thing. I hope that makes sense to you!
