# [Format commit history with git log arguments](https://egghead.io/lessons/tools-practical-git-format-commit-history-with-git-log-arguments)

## Passing Arguments to `git log`

To make our log info more meaninful and condensed, we can add arguments to `git log`.

### Commong Arguments to Know

- `--one line` - Condenses our commits and fit them onto one line.
![Image of git log --oneline output](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-format-commit-history-with-git-log-arguments/tools-practical-git-format-commit-history-with-git-log-arguments-oneline.png?1506025946)

- `--decorate` - Displays all references for our commits.
![Image of git log --decorate output](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_tools-practical-git-format-commit-history-with-git-log-arguments/tools-practical-git-format-commit-history-with-git-log-arguments-decorate.png?1506025946)

- `--graph` - Displays a graph of the branch structure for each commit

- `-p` - Stands for patch. Shows us the changes made by each commit.

- `--stat` - Shows us the number of additions (aka insertions) and deletions refor each commit made. Insertions are represented by pluses (+) and deletions are represented by minuses (-).

### Combining arguments

If you want to use more than one argument, you don't have to do a bunch of seperate `git log`'s. You can just chain them together! Order doesn't matter either.

```bash
git log --stat --oneline
```
