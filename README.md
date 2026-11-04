# ai-instrument-dev
Lidke Lab: AI-driven instrument development

## Add your GitHub username

Add one file, `usernames/<your-github-username>.txt`, that holds your GitHub
username, and open a pull request. One file per person, so pull requests never
conflict. Once the list is complete the repository goes private and everyone on
it is added as a collaborator.

You cannot push to this repository directly yet; you push to your own fork and
open a pull request from it.

### In the browser

1. Open https://github.com/LidkeLab/ai-instrument-dev/tree/main/usernames
2. Click **Add file > Create new file**. GitHub makes a fork for you.
3. Name the file `<your-github-username>.txt` and type your username in it.
4. Click **Commit changes** (or **Propose changes**), then **Create pull request**.

### From a terminal, with the GitHub CLI (`gh`)

```bash
gh repo fork LidkeLab/ai-instrument-dev --clone
cd ai-instrument-dev
git checkout -b add-$(gh api user --jq .login)
gh api user --jq .login > usernames/$(gh api user --jq .login).txt
git add usernames
git commit -m "Add $(gh api user --jq .login)"
git push -u origin HEAD
gh pr create --repo LidkeLab/ai-instrument-dev --fill
```

This repository is public: put nothing in it except your username.
