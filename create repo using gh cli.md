
```bash
gh repo create <repo-name>
```

This will prompt for:
- **Visibility** → public, private, or internal.
- **Location** → whether to create it under your account or an organization.
- **Clone options** → whether to clone it locally, add remote, or just create it online.

## Skip prompts by using flags:

### Create public repo:

```bash
gh repo create my-repo --public
```

### Create private repo:

```bash
gh repo create my-project --private
```

### Clone it locally immediately:

```bash
gh repo create my-project --public --clone
```

- creates an empty GitHub repo and clones this empty repo locally
- fresh start repo

### Add to current directory as remote:

```bash
gh repo create my-project --public --source=. --remote=origin
```

- `--source=.` tells GitHub CLI: _“Use the current local folder I’m in as the source for the new repo.”_
- It doesn’t make a new folder or clone anything. Instead, it takes your **existing local project** (files, commits, history) and connects it to the new GitHub repo.
- The `--remote=origin` part adds a remote named `origin` pointing to that new GitHub repo.
- basically creates the GitHub repo and pushes current directory to corresponding GitHub directory.

## After repo is created, then stage, commit, and push

[[git initial push]]
[[Add the remote to your local repo]]