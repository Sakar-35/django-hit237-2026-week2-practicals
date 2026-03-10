# project_blog

A Django project named project_blog.

## Quick installation (Windows PowerShell)

1. Create virtual environment:
	```powershell
	python -m venv .venv
	```

2. Activate venv (PowerShell):
	```powershell
	.\.venv\Scripts\Activate.ps1
	```

	If PowerShell blocks activation, run:
	```powershell
	Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
	```

3. Upgrade pip and install dependencies:
	```powershell
	python -m pip install --upgrade pip
	pip install -r requirements.txt
	```

	Or install Django directly:
	```powershell
	pip install --upgrade "Django"
	```

4. Create the Django project in the repository root (run once):
	```powershell
	django-admin startproject project_blog .
	```

5. Initialize the database:
	```powershell
	python manage.py migrate
	```

6. Start the development server:
	```powershell
	python manage.py runserver
	```

7. Verify in browser: http://127.0.0.1:8000/

Optional:
- Save exact installed packages:
  ```powershell
  pip freeze > requirements.txt
  ```
- Ensure `.venv/` is included in `.gitignore`.
- Do not create any Django apps — only the project `project_blog` is required.
# django-hit237-2026-week2-practicals