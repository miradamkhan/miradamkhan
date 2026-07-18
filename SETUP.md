# Adam Khan — GitHub profile README

Built with [readme-aura](https://github.com/collectioneur/readme-aura) (PurpleGlow-style).
This folder is **not** part of the readme-aura repo — copy it into your profile repo.

## Contents

| File | Purpose |
|------|---------|
| `readme.source.md` | Editable source (JSX cards) |
| `README.md` | Generated output for GitHub |
| `.github/assets/avatar.png` | Your profile photo |
| `.github/assets/*.svg` | Generated card images |
| `.github/workflows/readme-aura.yml` | Auto-rebuild on push / daily |

## Stats card

- **Repos** — public repo count  
- **Contributions** — total commits across your repos (live via GitHub API)  
- **Languages** — distinct primary languages (third pick: better than stars/followers while those are low)

## Publish to your profile

Your profile README must live in a repo named **`miradamkhan/miradamkhan`** (special GitHub profile repo).

```bash
cd ~/Downloads/miradamkhan-profile
git init
git remote add origin https://github.com/miradamkhan/miradamkhan.git
git add .
git commit -m "feat: purple-glow profile README"
git branch -M main
git push -u origin main
```

If the repo already exists with a README, clone it, copy these files in, then push.

## Rebuild locally

From this folder (with readme-aura available):

```bash
# needs a token for real stats (otherwise mock numbers)
set GITHUB_TOKEN=ghp_...
npx readme-aura build -g miradamkhan
```

Or using the local clone of readme-aura:

```bash
node path/to/readme-aura/dist/cli.js build -g miradamkhan
```
