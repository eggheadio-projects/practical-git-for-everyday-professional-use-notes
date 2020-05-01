# [10- Navigate git command pager output with Unix less commands](https://egghead.io/lessons/tools-practical-git-navigate-git-command-pager-output-with-unix-less-commands)

## Pager Outputs and How to Navigate Them

Some git commands and other terminal commands will print a lot of information to the screen. `git log`, `git diff`, and `git blame` are all good examples of this.

These types of commands open up **Terminal Pager**. You're probably using the **Unix less** pager and less gives us a lot of helpful commands. Here is a quick list of some of them.

- `q`- Stands for quit. Clears the screen and takes you back to your normal CLI

- `j` or `k`- Moves up or down one line at a time.

- `Ctrl F`- Stands for forward. Moves forward a screenful.

- `Ctrl B`- Stands for backward. Moves backward a screenful.

- `/`- Allows us to search for specific terms. Once you press enter, it will show you the results for said term.

  - `n`- Stands for next. Allows us to navigate to next search result.
  - `N`-  Allows us to naviage to previous search result.
