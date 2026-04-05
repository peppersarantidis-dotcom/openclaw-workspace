# Setup

## Machine context

- Host: `vmi3105350`
- Workspace: `/root/.openclaw/workspace`
- GitHub owner: `peppersarantidis-dotcom`

## Git

Installed and configured.

### Verify
```bash
git --version
git config --global user.name
git config --global user.email
```

## SSH authentication with GitHub

SSH access to GitHub is working.

### Verify
```bash
ssh -T git@github.com
```

Expected result:
```text
Hi peppersarantidis-dotcom! You've successfully authenticated, but GitHub does not provide shell access.
```

## GitHub CLI

GitHub CLI is installed and authenticated.

### Verify
```bash
gh --version
gh auth status
```

Current expected account:
- `peppersarantidis-dotcom`

## Repository

Local repository is connected to:

```bash
git@github.com:peppersarantidis-dotcom/openclaw-workspace.git
```

### Verify
```bash
git remote -v
git branch --show-current
git status
```

Expected branch:
- `main`

## Git workflow

### Push changes
```bash
git add <specific-files>
git commit -m "Describe changes"
git push
```

### Pull changes
```bash
git pull
```

## Notes

- `.openclaw/` is ignored from git.
- `tmp/` is ignored from git.
- This repository is an operational workspace repo for Pepper, not a conventional application codebase.
- Do not commit secrets, tokens, or machine-specific runtime state.
