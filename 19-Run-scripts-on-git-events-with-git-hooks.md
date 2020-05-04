# [19 - Run scripts on git events with git hooks](https://egghead.io/lessons/tools-practical-git-run-scripts-on-git-events-with-git-hooks)

## Finding git hooks

Inside of the `.git` folder is a `hooks`. This folder has scripts inside. These scripts won't run though becuase the `.sample` extension makes them dormant.

Without the `.sample` extension, scripts will run based on their name.

## Creating Scripts in `hooks`

Follow these steps to create a script in `hooks`.

1. Create a file inside of the `hooks` folder that has a name that matches the command you would like the script to run with. For example, `pre-commit` being created within the `hooks` folder will run whenever we try to commit something.

2. Once the file is created (`pre-commit` in this example), open it up in your text editor and add your script.

3. Run this command in terminal while in the `.git folder`. If you're not in the `.git` folder, you'll have to include the relative path to your script in `hooks`.

```bash
chmod +x hooks/pre-commit
```

FYI, `chmod` stands for change mode. This allows us to change the permissions of a file. The `+x` option means we want a file executable as a program.

Now when we run `git commit`, the script will run automatically.

**REMEMBER** adding scripts to `hooks` manually means those scripts are only accessible locally.

## More On Scripts

Here are two articles that talk about creating scripts if that's something you want know more about.

- [How to Create and Use Bash Scripts](https://www.taniarascia.com/how-to-create-and-use-bash-scripts/)

- [Writing a Simple Bash Script](linux.com/training-tutorials/writing-simple-bash-script/)
