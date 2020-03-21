# Git Branch Exercise

## Purpose

### Visualize How Branches Work

Using [Visualizing Git](http://git-school.github.io/visualizing-git/) we will get a visual representation of how commits and branches work.

### Practice Using git Commands

The Visualizing Git site uses Git Bash commands to affect changes on a practice repository.

## Instructions

1. Make a commit by typing `git commit` in the command line (in the bottom left corner of the site).
  -The `HEAD` marker can be thought of like a pointer to the commit that is the last commit made on the current branch. 
1. Make a new branch called 'feature' by typing `git branch feature`
  - Notice how there is a new branch name in addition to `master`. 
1. Make a new commit, typing `git commit`, without changing the branch, you should still be in master.
  - Notice the branch feature remains on the commit it was created from.  That is because we haven't added anything to that branch.
1. Change to the `feature` branch by typing `git checkout feature`.
  - The `HEAD` has no moved to the last commit that the `feature` branch knows about.
1. Make a few commits to the `feature` branch (`git commit`).
  - Notice that the new commits 'branch' off of the `master` branch.  The changes saved in these commits are not part of the `master` branch.  _Using branches allows you to make changes without affecting the `master` branch._
1. Merge the commit from the `master` branch into the `feature` branch by typing `git merge master`.
  - This adds the commit made after the `feature` branch was created into the `feature` branch.
1. Checkout the `master` branch and then merge the `feature` branch into the `master` branch.
  - This brings the commits made in the `feature` branch into the `master` branch.  After a merge it's as if you made the commits in the merged into branch itself. 

  ## Conclusion

  Using 'feature' branches to develop new features is one of the most safe and efficient ways to add new changes to your team's project repository.  Keeping your changes isolated in a feature branch will allow you to ensure that it doesn't effect others' work in unintended ways.