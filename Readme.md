## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we wanteds to create a git repo in a new project we've to create the folder and then initalize that repo using `git init`

```sh
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new/project
git init
touch Readme.md
code Readme.md
git status
git Readme.md
```

# Make changes to Readme.md

git commit -a -m "Add Readme file"

## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we're using Github Codespaces we'll create a temporary directory in our workspace

### HTTPS

```sh
git clone https://github.com/machius/github-examples.git
```

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## Commits

When we want to commit code

```
git commit -m "First Commit"
```

## Gitconfig file

The gitconfig file is waht stores your global configurations for git such as name, email, editor and more.

Show current git configuration

```
git config --list
```

When you first install git ona machine you are supposed to set up your name and email.

```sh
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"
```

Set the global editor

```sh
git config --global core.editor code
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included i.n the commit we can use the . to add all possible files

```
git add .
git add Readme.md
```

## Reset

Reset allows you to move staged changes to be unstaged.
This is useful when your want to revert all files not to be commited.

```
git add .
git reset
```

git reset will revert a git add.

## Status

git status shows you what files will or won't be commited.

```
git status
```

## Log

git log show recent git commits to the git tree

```
git log
```

## Push

When we want to push a repo roto our remot origin
