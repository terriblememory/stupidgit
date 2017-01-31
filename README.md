# StupidGit

Note that these scripts haven't exactly been tested rigorously.

Since I'm bad at Git and bad at Bash you should set your expectations accordingly!

## Installation

These are bash scripts so just clone this repository into a subdirectory and add that directory to your bash path in your .bashrc.

If, like me, you don't know bash, this is the command to add to .bashrc:

```export PATH="/c/code/stupidgit:$PATH"```

Obviously substitute the actual path for your case.

## Basics

Note: [repo] is the URL of a repository, e.g. https://github.com/terriblememory/stupidgit.

### GINIT [repo]
* Creates a local repo in the current directory.
* Adds all of the files in the directory tree in an initial commit to the local repo.
* Pushes the local repo to <repo>
* Makes <repo> the origin remote for this working copy.

### GCLONE [repo]
* Clones <repo> into the current directory.
* Makes <repo> the origin remote for this working copy.

### GPULL
* Updates the working copy from the origin remote.
* May require merge conflict resolution.

### GPUSH
* Adds all new files, changes and deletions.
* Pushes these changes to the origin remote.

## Subtrees!

### GSCLONE [subdir] [repo]
* Clones a repo as a subtree into the current subdirectory of a working copy.
* Makes <repo> the subtree origin remote.

### GSPULL
* Updates the subtree from the suntree origin remote.
* May require merge conflict resolution.

### GSPUSH
* Pushes subtree changes to the subtree origin remote.

### GSLIST
* Lists all of the subtrees in this repo.
