
## 🔑 Creating a GitHub Personal Access Token (Classic)

**Path:** `Settings → Developer settings → Personal access tokens → Tokens (classic)`

### 1. Navigate

- Go to your GitHub profile.
- Click **Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)**.
- Click **Generate new token**.
### 2. Configure

- **Note:** Classic tokens are older; GitHub now recommends fine‑grained tokens for most use cases. Use classic only if required by tooling. 
	- fine grain are repo specific
- Give the token a descriptive name (e.g., _CLI access_).
- Set an expiration date (security best practice).

### 3. Select scopes

For typical CLI and repo management, check:
- `repo` → full control of private and public repositories.
- `read:org` → read access to organization membership and details.

_(Optional: add other scopes only if your workflow requires them, e.g.,_ `workflow` _for GitHub Actions.)_

### 4. Generate & store

- Click **Generate token**.
- Copy the token immediately — you won’t be able to see it again.
- Store it securely (e.g., in a password manager or environment variable).

[[gh clone repo]]

![[token-selection.png]]