# Git Workflow Documentation

## Commands used

```bash
git init
git branch -M main
git remote add origin <repo-url>
git push -u origin main
git checkout -b dev
git checkout -b feature/<name>
git add <file>
git commit -m "type: message"
git push -u origin feature/<name>
git tag -a v1.0.0 -m "First stable release"
git push origin v1.0.0
```

## Branching strategy

- `main`: stable code
- `dev`: integration branch
- `feature/*`: one branch per task
