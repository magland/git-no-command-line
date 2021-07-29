# Understanding staging, committing, pushing, and pulling

We are all getting used to realtime communication. For example, when you edit a live Google document, you don't need to worry about uploading or downloading versions; what you see in your browser is always exactly the same as what your colleague is seeing on the other end. However, when developing software in a collaborative environment, this is not desired modality.

With git, this process of sharing updates goes through a number of steps:

```
stage, commit, push, pull
```

or, more advanced but recommended:

```
branch, stage, commit, push, pull request, review, merge, pull
```

Why so many steps? There is a reason for this madness. Here's a breakdown of what these things mean.

## Staging

Staging can be considered as part of the commit step. In order to commit some updates (maybe a few files were added and a few other files were modified), you need to have some mechanism for first specifying which updates should be included in the next commit. So when you add a file (`git add <filename>`), you are not committing it directly, but you are marking that update as staged so that when you do commit, the modification will be included.

## Committing

A commit is the fundamental update step in a git repository, but it does *not* involve any information transfer between computers. Once you have staged one or more updates, you can commit those changes with a commit message. Your local repository has now been modified in that a commit has been added to your local branch. However, nothing has been uploaded yet to GitHub.

## Pushing

The push step is when you upload the changes you made to your local repository (ie, new commits) to the remote repository hosted on GitHub.

## Pulling

The pull step is when your collaborator downloads the changes made to the remote repository (on GitHub) to their local repository.
