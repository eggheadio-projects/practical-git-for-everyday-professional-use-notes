# [Resolve merge conflicts with git status](https://egghead.io/lessons/tools-practical-git-resolve-merge-conflicts-with-git-status)]

## What Are Merge Conflicts?

Running `git pull` to sync remote and local repositories might not always work. We might get a merge conflict error message.

What is a merge conflict? Merge conflicts happen when local changes and remote changes can't be merged automatically by Git. If there's been a change in same place on both the local and remote branch, you'll get a merge conflict.

Once we fix the merge conflicts, we can successfully push our code to Github without any errors.

## How to Resolve Merge Conflicts

Follow these steps to fix merge conflicts.

1. Run `git status` to see where the conflict is comming from. This will show a `Unmerged paths` which will point to the file that needs to be fixed.
![Image of command line git status unmerged paths error](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-resolve-merge-conflicts-with-git-status/tools-practical-git-resolve-merge-conflicts-with-git-status-conflicting-files.png?1506026075)

2. Open the files that have conflicts in your text editor. Git will show you where the conflicts are.
![Image of merge conflicts in file](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-resolve-merge-conflicts-with-git-status/tools-practical-git-resolve-merge-conflicts-with-git-status-git-modfies-file.png?1506026075)
The section marked as `HEAD` are the changes we made. Right below that is the code from the remote repository.

3. Now you need to determine what you want to keep and want you want to delete. Sometimes, you'll choose to keep your changes. Other times you'll choose to keep the remote changes. You can even combine the remote and local changes.

4. Now that you know what to keep and get rid of, delete the markers that Git put in your file, `<<<<<<< HEAD`, `>>>>>>> {numbers}`, etc. Make whatever alterations you think are necessary.

5. You can now proceed business as usually and stage, commit, and push your files.
