# Working with Git

The repository and index may be shared. Before changing Git state, inspect status and staged and unstaged diffs; identify this operation's edits and apply the repository's branch and commit conventions.

Stay within the agreed scope and working mode. Editing or staging permission does not authorize a commit or later work. When commits are authorized, keep coherent revert points.

Stage explicit paths, never `git add -A` or `git commit -a`. Check ownership before including a file that may contain others' edits; resolve uncertainty first.

Commit with `git commit --only -- <paths>`. A plain commit can take others' staged work. Path-limited commits take current file contents, so first review the full diff against HEAD, including unstaged edits.

Verify committed paths and diff, then the remaining state. Never reset, discard, or unstage others' work to make the tree or index clean.

links: is↑ [my-cognition-method](../topics/my-cognition-method.md)
