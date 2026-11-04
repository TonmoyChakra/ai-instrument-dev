# ai-instrument-dev
Lidke Lab: AI-driven instrument development

## How changes land

Nobody pushes to `main`. Make a branch from `main`, push the branch to this
repository, and open a pull request into `main`.

## Add your GitHub username

Add one file, `usernames/<your-github-username>.txt`, that holds your GitHub
username, on your own branch, and open a pull request. One file per person, so
pull requests never conflict.

```bash
git clone https://github.com/LidkeLab/ai-instrument-dev.git
cd ai-instrument-dev
git checkout -b add-<your-github-username> main
echo <your-github-username> > usernames/<your-github-username>.txt
git add usernames
git commit -m "Add <your-github-username>"
git push -u origin add-<your-github-username>
gh pr create --fill        # or open the pull request on github.com
```

Pushing a branch needs write access to this repository. If your push is
refused, ask Keith Lidke to add you as a collaborator.

This repository is public: put nothing in it except your username.
