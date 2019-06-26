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
------------  ---------  ------------------------------------  ----------------------------------------------
pull request  can merge  Add first version of the git-pr tool  https://github.com/andersjohnsen/git-pr/pull/1
review        pending    No reviews reported
build         invalid    Revision not being built
------------  ---------  ------------------------------------  ----------------------------------------------
```
