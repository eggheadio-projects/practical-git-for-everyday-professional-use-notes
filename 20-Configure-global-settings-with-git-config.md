# [20 - Configure global settings with git config](https://egghead.io/lessons/misc-practical-git-configure-global-settings-with-git-config)

## How `git config --global` Works

You might have a `.gitconfig` file in your root directory. `.gitconfig` contains some git settings like your name and email address. We can access some of these settings and change them using `git config --global`.

Here are some of the settings you can change using `git config --global`.

- `user.name` - We can use this followed by a name to set a new username. `git config --global user.name "Jane Doe"`

- `user.email` - We can use this followed by an email address to ad a new user email. ``git config --global user.email janedoe@whatever.com`

- `core.editor` - We can set our default editor for Git to open up whenever a text editor is necessary using this. Type this followed by the name of your code editor. `git config --global core.editor vim`

- `alias.` - Allows us to create an alias for a specifiec git command. We attach our preferred alias name to `alias.` followed by the git command wrapped in quotes. `git config --global alias.graph 'log --graph --oneline'`

- `--list` - This will show us the contents of our `.gitconfig` file.
