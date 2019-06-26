# git-pr
Git utility for working with GitHub Pull Requests

## Install

To install put the tool into your path, e.g.:

```
$ ln -s `pwd`/git-pr ~/.local/bin/git-pr
```

The tool can now be invoked by saying

```
$ git-pr
Usage: git-pr [OPTIONS] COMMAND [ARGS]...
[...]
```

## Using

Simple quide to using the `git-pr` tool.

### Create pull request

Create a branch you want to use for the pull request. Now invoke

```
$ git pr create
```

and a pull request will be created.

### Get status

Type out

```
$ git pr status
```

and to get the list of your open pull requests, use
```
$ git pr list
```

and for all open pull requests associated to the repository

```
$ git pr list --all
```

### Updating

When you have committed new changes locally to your branch, run
```
$ git pr update
```

to update the remote pull request with your latest changes.

If you changed your history, e.g. by using rebase, you can force push your changes by using

```
$ git pr update -f
```


### Landing

Finally, you can now do

```
$ git pr land
```

This will `squash-merge` your change, delete the remote branch, update local master, and delete local branch if pointing to the new master.
