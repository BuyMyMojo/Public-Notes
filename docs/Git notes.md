# Learning git

## Settings

Remember to set your name and email when setting up git!

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

## Creating a repo

To create a git repo jusr use this simple command in a repo:

```bash
git init
```

## Commiting from CLI

First thing to do is to check the status of your changes(ie; what files have changed and what new files there are)

```bash
git status
```

Next add the changes you want into staging to be commited, this can be done in a couple ways.

You can add all changes with

```bash
git add .
```

You can add a single file using

```bash
git add file.go
```

You can add multiple files using

```bash
git add file.go file2.go file3.go
```

To actually commit you use

```bash
git commit -m "Commit message"
```

the `-m` in this case adds a message to the commit.

If you have setup a [PGP/GPG](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key) key for git then add the `-S` flag to sign it

## Git history

To look at the history of a repo use

```bash
git log
```

to view the past commits, comments and authors

To go to back to a specific commit to view the code or to make a new branch from a past point use

```bash
git checkout <commit hash>
```

to go back to the current code use

```bash
git checkout master
```

## Branches

To make a new branch just use

```bash
git branch <Branch name>
```

To change the current branch you're in use

```bash
git checkout <Branch name>
```

To create a new branch and swap to it at the same time use

```bash
git checkout -b <Branch name>
```

To merge changes from a branch into the master branch use

```bash
git merge <Branch name>
```

Finally to delte a branch use

```bash
git branch -d <Branch name>
```

### Further reading

- [Free official git book](https://git-scm.com/book/en/v2)
- [Official git docs](https://git-scm.com/doc)
- [GitHub's docs](https://docs.github.com/en)
- [GitLab's docs](https://gitlab.com/help)
