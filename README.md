# DevOps Git Project

A small project that demonstrates a professional Git and GitHub workflow: branching, pull requests, tags, and documentation.

## Tech Used

- Git and GitHub
- Python 3
- Docker

## Project Structure

```
devops-task4/
├── app.py          # Simple Hello World app
├── Dockerfile      # Container image for the app
├── .gitignore      # Files Git should ignore
└── README.md       # Project documentation
```

## How to Run

**Locally:**

```bash
python3 app.py
```

**With Docker:**

```bash
docker build -t devops-task4 .
docker run devops-task4
```

Expected output: `Hello, DevOps!`

## Branching Strategy

| Branch | Purpose |
|---|---|
| `main` | Stable, production-ready code |
| `dev` | Integration branch where features are combined |
| `feature/*` | One branch per task (e.g. `feature/add-dockerfile`) |

## Workflow Followed

1. Create a `feature/*` branch from `dev`
2. Commit changes with clear messages
3. Open a pull request into `dev` and merge it
4. When `dev` is stable, open a pull request from `dev` into `main`
5. Tag the release on `main` (e.g. `v1.0.0`)

## Commit Message Convention

- `feat:` new feature
- `chore:` maintenance (e.g. .gitignore)
- `docs:` documentation changes

## Author

Mohd Ahmad
