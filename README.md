# Session 17 - DevSecOps Pipeline (Python / Flask)

Practice repository for the Session 17 assignment of
[devops-heros](https://github.com/Ishan007-bot/devops-heros/tree/main/session-17-devsecops).

```text
Unit Tests ─┐
SAST (CodeQL) ─┼─► Docker Build ─► Trivy Image Scan (gate) ─► Push to GHCR ─► Deploy to Kubernetes (Kind)
SCA (pip-audit)┘
```

Run locally:

```powershell
python -m venv .venv
.venv\Scripts\python -m pip install -r requirements-dev.txt
.venv\Scripts\python -m pytest --cov=app
.venv\Scripts\python app\app.py        # http://localhost:5001
```
