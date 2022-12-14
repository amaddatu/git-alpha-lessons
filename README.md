# git-alpha-lessons

## Description

In this example you will need to checkout the ex_branch. From here you can check the history on the files. The commit numbers are listed so you can see what is going on.

### git log

Type:

```console
git log
```

Press arrow keys to move up and down. Hit `Q` to exit.

## Next make changes

Make any change to the `index.html`. You will see those changes in `git status`.

### git status

Type:

```console
git status
```

## Next stash changes

The stash holds changes temporarily.

### git stash

Type:

```console
git stash
```

## Next bring back those changes

You can bring back changes by using `pop`.

### git stash pop

Type:

```console
git stash pop
```

## Next clear the stash

If you stash changes and either never look at it again or delete the changes you will not be able to recover them.

### git stash clear

Type:

```console
git stash
git stash clear
```

## Use checkout filename

`checkout` can be used to restore files that are on the current version. If you happen to delete a file by accident. You can restore using git checkout.

### git checkout filename

Type:

```console
rm index.html
git checkout index.html
```

## Use checkout commit-number to get an entire commit version

`checkout` is used to move something known as a repo-pointer to different parts of history. So if you use the a commit number it will get the lastest version of the branch.

### git checkout commit-number

Type:

```console
git checkout 06aa6be45d24356ea3621128fe7001c19b187d0b
```

## Get the current version

`checkout` is used to move something known as a pointer. So if you use the branch name instead it will get the lastest version of the branch.

### git checkout ex_branch

Type:

```console
git checkout ex_branch
```

## Use show to see a previous commit

`Show` is used to see what a previous committed file looks like.

### git show commit-number:filename

Type:

```console
git show 06aa6be45d24356ea3621128fe7001c19b187d0b:index.html
```

## Use show to retrieve another version of a specific file in history

You can use `show` to also get the older file versions and compare them inside of VSCode very easily. Select both files and hit compare in the right-click menu.

### git show commit-number:filename > oldfile

Type:

```console
git show 06aa6be45d24356ea3621128fe7001c19b187d0b:index.html > index_old.html
```
