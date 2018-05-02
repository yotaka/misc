



# First time configuration options

## Read/Write Local/Global name and mail

Usually mandatory for push.

```
git config --local user.name "UsernameForThisRepoOnly"
git config --local user.email "EmailForThisRepoOnly"
git config --global user.name "UsernameSystemwide"
git config --global user.email "EmailSystemwide"
``` 

`--local` overwrites `--global` if set for the current repository. 
Whatever is active can be checked with `git config --get user.name`.

## Set push strategy to simple

`git config --global push.default simple`

## Activate long path support

> Git File or path name too long

`git config --system core.longpaths true`

# Misc

## Export last commit (-1 -> 1 commit, -10 -> 10 commits) into patch

`git format-patch -1 HEAD --stdout > last-commit.patch`


My `~/git.config`

```
[alias]
	ls = log -n 10 --pretty=format:"%C(yellow)%h%Cred%d\\ %Creset%s%C(bold\\ blue)\\ [%cn]" --decorate
	lg = log -n 10 --color --graph --abbrev-commit --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%C(bold blue)<%an>%Creset'
```

Can be set on windows: `c:\dev> git config --global alias.ci "commit -v"` where `ci` is the alias for `commit -v`.
On Linux, use single-quotes instead.
