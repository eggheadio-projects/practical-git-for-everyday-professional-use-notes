# [Show who changed a line last with git blame](https://egghead.io/lessons/tools-practical-git-show-who-changed-a-line-last-with-git-blame)

## How `git blame` Works

`git blame` shows us how each line was last changed inside of a specified file. We have to pass a file name to the command like this `git blame filename.js`.

When we run `git blame`, we can see the commit ID of the last line change, who made that change, and when that change was made.

![Image of git blame output](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-show-who-changed-a-line-last-with-git-blame/tools-practical-git-show-who-changed-a-line-last-with-git-blame-git-blame-command.png?1506026184)

### Using `git blame` Output with Other Git Commands

The output of `git blame` could be very helpful when used along side other Git commands. One example is `git log`.

We can pass one of the commit ID's we get with `git blame` in to `git log` for information on the commit.
