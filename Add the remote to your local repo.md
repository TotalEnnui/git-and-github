
## HTTPS

```bash
git remote add origin https://github.com/USERNAME/REPO-NAME.git
```

## SSH

```bash
git remote add origin git@github.com:USERNAME/REPO-NAME.git
```

### 🔑 Core Differences Between HTTPS and SSH in GitHub

|Feature|HTTPS|SSH|
|---|---|---|
|**Authentication**|Username + password or Personal Access Token (PAT)|SSH key pair (public key on GitHub, private key on your machine)|
|**Ease of Setup**|Very easy, no extra tools needed|Requires generating and adding SSH keys|
|**Security**|Secure via SSL/TLS, but relies on tokens/passwords|Stronger security with public-key cryptography|
|**Convenience**|Prompts for credentials unless cached|No repeated login—keys handle authentication automatically|
|**Firewall Compatibility**|Uses port 443 (almost always open)|Uses port 22 (may be blocked by corporate firewalls)|
|**Best For**|Beginners, occasional use, environments where SSH is blocked|Frequent pushes/pulls, automation, CI/CD pipelines|