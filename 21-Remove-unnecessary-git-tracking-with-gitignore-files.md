# [21 - Remove unnecessary git tracking with .gitignore files](https://egghead.io/lessons/tools-practical-git-remove-unnecessary-git-tracking-with-gitignore-files)

## Why We Need `.gitignore`

Sometimes we'll have files and folders that we don't want tracked by git. That's where `.gitignore` comes in.

### Creating and Adding to a `.gitignore` File

Create a `.gitignore` file by running `touch .gitignore`.

For a file or folder to be untracked, we have to type the name of the file or folder inside of the `.gitignore` file.

### What to Put Inside of `.gitignore`

Every project will require that certain files be ignored. But generally, you'll want to exclude anything that's **automaticall generated** or **user specific**.
