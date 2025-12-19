
```bash
# Initialize a brand new local repo
git init
git add README.md   # optional, or add all files with `git add .`
git commit -m "initial commit"

# Ensure branch name is 'main' (modern Git defaults to main, so this may be optional)
git branch -M main

# Link local repo to GitHub remote (only needed if you created the repo manually on GitHub)
git remote add origin https://github.com/TotalEnnui/<my_project>.git

# Push local commits to GitHub and set upstream tracking
git push -u origin main
```

## When `git remote add origin` is **not needed**

- If you used:
    - `gh repo create my-project --public --clone`   
    - `gh repo create my-project --public --source=. --remote=origin`
- In both cases, GitHub CLI already sets up the remote named `origin` for you.
    
- You can confirm with:

```bash
git remote -v
```

## Key reminders

- `origin` → just an alias for the GitHub repo URL (default remote name).
- `-u` **/** `--set-upstream` → tells Git to track your local branch (`main`) against the remote branch (`origin/main`), so future `git push` and `git pull` commands don’t need extra arguments.