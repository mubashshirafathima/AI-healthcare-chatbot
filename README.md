# AI Healthcare Chatbot (Flask)

## Prerequisites (Windows)
- Install **Python 3.11+ (64-bit)** and make sure it’s available as `python` (or `py`).

Verify:
```powershell
python -V
pip -V
```

## Setup
From the repo root:
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you already have the included `tf_env` virtual environment working, you can use it instead:
```powershell
& .\tf_env\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Run
```powershell
python .\flask\app.py
```

Open:
- http://127.0.0.1:3000

## Notes
- The app uses `flask/database.db`, `flask/dataset.xlsx`, and `flask/model/random_forest.joblib`.
- On first run it will create missing DB tables automatically.
