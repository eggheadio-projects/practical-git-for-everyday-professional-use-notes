# [Create local repos with git init](https://egghead.io/lessons/misc-practical-git-create-local-repos-with-git-init)

## Turning a Folder Into a Git Repo

Follow these steps to turn a folder into a git repository.

1. In the command line, navigate to the folder you want to make a git repo.

2. Run `git init`. This starts or initializes an empty Git repo

### `.git`

To get a view of how this works under the hood, run `ls -a`. There should be a `.git` folder listed.

Running `cd .git` will show us what's inside. All the information and settings Git needs to run are inside of this `.git` folder.

### Removing `.git`

Without `.git`, Git won't track our project. If we don't want Git to track our project anymore, just delete the `.git` folder using this command: `rm -rm .git/`.

## Creating a Repo on GitHub

The point of using Git is to be able to sync up our local repo with a remote repo. We need a service like Github for that. The first step to doing this is creating a repo on Github.

1. Log into your Github account, click the plus symbol in the top right hand corner and select "New Repository".

2. Give your repo a name. It's best practice to give it the same name as the folder you're trying to upload.

3. Give your repo a description.

4. Click the "Create Repository" button.

## Syncing Local Repositories with Remote Repositories

After creating the remote repo, you'll want to follow these steps to actually sync your local repo with your remote repo.

1. Once the repo is created on Github, there will be a URL available. Copy this URL.
![Image of Github Remote Repository URL](https://d2eip9sf3oo6c2.cloudfront.net/asciicasts/Practical%20Git%20for%20Everyday%20Professional%20Use/original_misc-practical-git-create-local-repos-with-git-init/misc-practical-git-create-local-repos-with-git-init-git-url.png?1506025680)

2. Back in the command line, type `git remote add origin` followed by the URL that you just copied. `origin` is the name of the remote repository.

3. To verify that the remote repo was added correctly, run `git remote -v`.
