# Git Cheat Sheet

To make any changes to this repo:

1. Before you start working, pull the latest code from the `main` branch and create your own branch.

```
cd gw-rml-group4
git checkout main
git pull
git checkout -b new-branch-name
```

2. Commit and push your edits.

```
git status
git add .  # this adds everything.  add individual files instead, if needed
git commit -m "tuned XGB parameters"
git push origin new-branch-name
```

3. Make a pull request. A pull request is how we apply your changes to the main branch.

    - When you `git push`, your terminal will give you a link to create the pull request on GitHub.

    - Make sure the target branch is `main`.

    - Add Chip as a reviewer to the pull request.

    - Hit Create Pull Request.

4. Ask Chip to review & merge.

