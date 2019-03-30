# repo_help
Github repository commands and usages

The readme.md is an update of file https://gist.github.com/collodi/9db7d4cb9f5e33c04d64f2eac8a5d84b

# Useful Git Commands
```
git status
```

```
git add file
```

```
git commit -m "..."
```

```
git push origina master
```

```
git pull origin master
```

``` 
git clone <url>
```

```
git remote add origin <url>
```

```
git init
```

```
git reset --hard
git pull
```


# Process to initialize a Git repository

Git is a simple version control program. We'll talk about hor to set up a remote repository.
You must first make an empty repository in github.com, which will give an url for the repository.
For example, after make a Topsim repository under FSU-CS-EXPLORER-LAB on github.com, the url would be 

https://github.com/FSU-CS-EXPLORER-LAB/Topsim.git

After the url is there, the follow command sequence initializes and populates the repository (from local files)

## Init
First, you need to initialize the project as a git repo. You can do this by typing
```
git init
``` 
in your project root directory.

## Commits
Git keeps track of *commits*. We are going to create an initial commit. Before we can create a commit, we need to stage the files we want to commit. To
 see the current status of files, you can type
```
git status
```

Staging files is done with
```
git add <files>
```
command, or if you want to commit everything in the repository, say
```
git add -A
```

Now, if you type `git status`, you can see that your files are staged. To commit the changes in the stages files, you say
```
git commit -m <message>
```
where <message> says something useful. Since this is the initial commit, you can say
```
git commit -m 'init'
```

## Remote
Now that we are finished with all the local commits, we want to push these changes to the remote repo so that others can see them.

First, we have to add the remote repo as our origin. You do this by typing
```
git remote add origin <url>
```

You can get <url> from the remote repo's website. In case of Topsim, it is
```
https://github.com/FSU-CS-EXPLORER-LAB/Topsim.git
```

And finally, we can push our commits to the remote repo by typing
```
git push -u origin master
```

This pushes all commits to the master branch of the remote repo, and the `-u` option makes this `origin/master` branch as your default push branch. So,
 the next time you need to push your commits to the remote repo, you can just type
```
git push
```
<diablo:1003> more git-commands.md 
# Git Commands

Git is a simple version control program. We'll talk about remote repositories, but most of git is made for local uses.

## Init
First, you need to initialize the project as a git repo. You can do this by typing
```
git init
``` 
in your project root directory.

## Commits
Git keeps track of *commits*. We are going to create an initial commit. Before we can create a commit, we need to stage the files we want to commit. To
 see the current status of files, you can type
```
git status
```

Staging files is done with
```
git add <files>
```
command, or if you want to commit everything in the repository, say
```
git add -A
```

Now, if you type `git status`, you can see that your files are staged. To commit the changes in the stages files, you say
```
git commit -m <message>
```
where <message> says something useful. Since this is the initial commit, you can say
```
git commit -m 'init'
```

## Remote
Now that we are finished with all the local commits, we want to push these changes to the remote repo so that others can see them.

First, we have to add the remote repo as our origin. You do this by typing
```
git remote add origin <url>
```

You can get <url> from the remote repo's website. In case of Topsim, it is
```
https://github.com/FSU-CS-EXPLORER-LAB/Topsim.git
```

And finally, we can push our commits to the remote repo by typing
```
git push -u origin master
```

This pushes all commits to the master branch of the remote repo, and the `-u` option makes this `origin/master` branch as your default push branch. So,
 the next time you need to push your commits to the remote repo, you can just type
```
git push
```
