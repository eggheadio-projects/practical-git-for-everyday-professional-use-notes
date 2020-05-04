# [Use semantic versioning with git tag](https://egghead.io/lessons/tools-practical-git-use-semantic-versioning-with-git-tag)

## How `git tag` Works

We can create tags for commits using the `git tag` command. We type `git tag` followed by the name of our tag.

```bash
git tag v1.0.0
```

To check the tags associated with a repository, just run `git tag` by itself.

### Naming Tags

There is a specific way you'll see most people naming tags. This is called **semantic versioning**. With `v1.0.0`, there are three different numbers.

- v**1**.0.0 - The first numnber is incrememnted when a major release is made with breaking code changes.

- v1.**0**.0 - The second number is incremented when a minor release is made which is a minor feature that isn't breaking.

- v1.0.**0** - The third number is for when a patch release is made meaning a small bug fix.

Think, `vMajor.Minor.Patch`.

## Why Use `git tag`

`git tag` allows us to give a name to a commit. That name does not change. It's a great way to reference different versions of a project. This is why thr `vMajor.Minor.Patch` is the standard naming convention for tags.

## Adding Tags to Remote Repositories

We may want our tags to be on our remote repository as well. To do this we use the `--tags` flag.

```bash
git push --tags
```

### Annotating Tags

We can add notes to our tags too. We do this by using the `-a` (annotation) and `-m` (message) options.

```bash
git tag -a V2.0.1 -m "We fixed a small bug"
``
