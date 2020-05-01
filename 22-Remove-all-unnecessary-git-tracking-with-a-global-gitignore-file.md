# [Remove all unnecessary git tracking with a global .gitignore file](https://egghead.io/lessons/tools-practical-git-remove-all-unnecessary-git-tracking-with-a-global-gitignore-file)

## Creating a Global `.gitignore`

If we know that every repo on our machine will need to ignore a certain kind of file or folder, we can create a global `.gitignore`.

1. In your root directory, create a file called `.gitignore_global`. The name doesn't really matter but this is suggested.

2. Inside of the `.gitignore_global` file, type the name(s) of the file(s)/folder(s) that you would like to be globally ignored.

3. In the command line type `git config -- global core.excludesfile` follwed by the path to the `.gitignore_global` file. This might look like this:
`git config -- global core.excludesfile ~/.gitignore_global`.
