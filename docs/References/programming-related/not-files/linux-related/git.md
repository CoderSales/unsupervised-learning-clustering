### Reference:
- Hard delete unpublished commits [git reset --hard 0d1d7fc32](https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit)

#### Excerpt from above reference:

```
Hard delete unpublished commits
If, on the other hand, you want to really get rid of everything you've done since then, there are two possibilities. One, if you haven't published any of these commits, simply reset:

# This will destroy any local modifications.
# Don't do it if you have uncommitted work you want to keep.
git reset --hard 0d1d7fc32
```

-------------------------

Previous attempts to delete unpublished commits, reconcile histories and progress on main branch:
-  `--allow-unrelated-histories` [Git refusing to merge unrelated histories on rebase](https://stackoverflow.com/questions/37937984/git-refusing-to-merge-unrelated-histories-on-rebase)

- `git config pull.rebase false` [Solved "fatal: Need to specify how to reconcile divergent branches"](https://www.cyberithub.com/solved-fatal-need-to-specify-how-to-reconcile-divergent-branches/)

- `git push -u origin head` [fatal: The current branch master has no upstream branch](https://stackoverflow.com/questions/23401652/fatal-the-current-branch-master-has-no-upstream-branch)

- `git checkout master` | `git checkout -- path/to/foo`` [How do I fix a Git detached head? | If you want to delete your changes associated with the detached HEAD](https://stackoverflow.com/questions/10228760/how-do-i-fix-a-git-detached-head)

 - `git branch alt-history` | `git checkout alt-history` | `git config advice.detached head false` [Git Detached Head: What This Means and How to Recover | How Do I Fix a Detached HEAD in Git? | Getting Rid of the “Git Detached HEAD” Message](https://www.cloudbees.com/blog/git-detached-head)
 ### How to remove big file wrongly committed
 - [git : How to remove a big file wrongly committed](https://thomas-cokelaer.info/blog/2018/02/git-how-to-remove-a-big-file-wrongly-committed/)