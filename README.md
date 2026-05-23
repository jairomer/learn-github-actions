# Learning GitHub Actions

> A sandbox repository for experimenting with and learning about GitHub Actions.

---

## Workflow: Check Bats Version

**File:** `.github/learn-github-actions.yml`

| Trigger | Runs on |
|---------|---------|
| `push`  | Any branch |

This workflow performs the following steps:

1. **Checkout** the repository — uses `actions/checkout@v6`
2. **Setup Node.js 20** — uses `actions/setup-node@v4`
3. **Install Bats** — runs `npm install -g bats`
4. **Print version** — runs `bats -v`
