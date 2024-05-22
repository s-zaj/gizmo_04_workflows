# Workflows

## Some examples of "Contributing" guidelines

### LLVM

Excerpt from the [LLVM Contributing guide](https://llvm.org/docs/Contributing.html#how-to-submit-a-patch)

A patch should:

* not contain any unrelated changes
* be an isolated change. Independent changes should be submitted as separate patches as this makes reviewing easier.
* have a single commit (unless stacked on another Differential), up-to-date with the upstream origin/main branch, and don’t have merges.

Once a patch is reviewed, you can select the “Squash and merge” button in the GitHub web interface.
You might need to rebase your change before pushing it to the repo.
LLVM currently has a linear-history policy, which means that merge commits are not allowed. 
The llvm-project repo on github is configured to reject pushes that include merges, so the git rebase step above is required.

### Git

Excerpt from the [Git Contributing guide](https://github.com/git/git/blob/master/Documentation/SubmittingPatches)

We should point out that "habitually" (regularly for no real reason)
merging an integration branch into your topics -- and by extension,
merging anything upstream into anything downstream on a regular basis
-- is frowned upon.
