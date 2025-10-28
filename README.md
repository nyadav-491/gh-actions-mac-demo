# GitHub Actions CI Demo (macOS)

Minimal repo to demonstrate CI with GitHub Actions and pytest.

## Local (macOS)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pytest -q
```

## Push to GitHub
```bash
git init
git add .
git commit -m "Add minimal CI"
git branch -M main
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```

## Break & Fix (for demo)
Change `return a + b` to `return a + b + 1` in src/app.py. Commit & push (CI fails). Revert & push (CI passes).
