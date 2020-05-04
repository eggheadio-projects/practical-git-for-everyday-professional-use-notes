# [Filter commit history with git log arguments](https://egghead.io/lessons/tools-practical-git-format-commit-history-with-git-log-arguments)

## Options for Filter `git log` Output

We can use options with `git log` to filter our results so that they're more specific.

- `git log -num` - Insert number of your choosing where `num` is. This will show us the `num` most recent commits. So `git log -3` will show us the 3 most recent commits.

- `--after` - Allows us to view commits that were made after a certain specified time. Here are some of the time frames we can specify
  - `--after="yesterday"`
  - `--after="30 minutes ago"`
  - `--after="last Tuesday"` - You can insert any day here
  - `--after="2 weeks ago"` - You can insert "months" or "years" too
  - `--after="3-15-16"`- You can insert any date here. It can also be formatted like "3/15/16"

- `--before`- Works like `--after`. Instead allows us to view commits that were made **before** are certain specified time frame. It follows the same dating format as `--after`.

- `--since` - Does the same thing as `--after`. You can use whichever you prefer.

- `--until` - Does the same thing as `--before`.

- `--author` - Allows us to filter out commits made by a specific person. Enter the name in quotes following the equal sign. `git log --author="Ceora"`
  - Can also search email addresses.

- `--grep` - Allows us to search commit messages. Formatted like `--author`. Place the message text you want to search in quotes after the equal sign. `git log --grep="copyright"`

- `--no-merges` - Only shows commits that are not merge commits.

- `git log filename` - Allows us to see commits made in reference to a specific file. Include the file name after `git log`.

### Options For Displaying Commits that Add/Remote Code

- `-S` - This filters down to commits that change (add or remove) a certain string in our code. It's formatted like so: `git log -S"Math"`. Notice that there is **no equal sign between the option and the value**.
This will show us all the commits that use the `"Math"` object. We'll only see the commit log and not the code changes.
  - If we want to see the code changes we can use the patch formatting option `-p`. `git log -p -S"Math"`

- `-G` - We can also make searches using Regular Expressions using this option. `git log -GMath\|Random`

### Flags

We can also combine options for even more efficient results. Here are some add on options that are often used to do this.

- `-i`- This is the ignore flag. This ignores the case of our searches. `git log -i --author="Jane"` will now show results that also include `jane`.

## Comnbining Options

Options can be combined!

```bash
git log -3 -i --author="ceora" README.md
```

This will output the last 3 commits made to the `README.md` file by someone named `"ceora"` or `"Ceora"` because case doesn't matter since we used the `-i` flag.
