# Django gitignore
A comprehensive and production-ready .gitignore template for Django projects.

MIT License - Free to use, share, and improve.

---

```gitignore
# ---------------------------------------------------
# Python
# ---------------------------------------------------
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
share/python-wheels/
*.egg-info/
.installed.cfg
*.egg

# ---------------------------------------------------
# Virtual Environments
# ---------------------------------------------------
venv/
env/
ENV/
.venv/

# ---------------------------------------------------
# Django
# ---------------------------------------------------
*.log
local_settings.py
db.sqlite3
db.sqlite3-journal
media/

# Static files (collectstatic output)
staticfiles/
static_root/

# ---------------------------------------------------
# Environment Variables
# ---------------------------------------------------
.env
.env.*
!.env.example

# ---------------------------------------------------
# Secrets / Certificates
# ---------------------------------------------------
*.pem
*.key
*.crt
*.csr
*.p12

# ---------------------------------------------------
# Testing
# ---------------------------------------------------
.coverage
.coverage.*
.cache
.pytest_cache/
nosetests.xml
coverage.xml
*.cover
*.py,cover
htmlcov/

# ---------------------------------------------------
# Type Checkers
# ---------------------------------------------------
.mypy_cache/
.dmypy.json
dmypy.json
.pyre/
.pytype/

# ---------------------------------------------------
# Linting
# ---------------------------------------------------
.ruff_cache/
.pylint.d/

# ---------------------------------------------------
# Jupyter
# ---------------------------------------------------
.ipynb_checkpoints

# ---------------------------------------------------
# IDEs
# ---------------------------------------------------
.idea/
.vscode/
*.swp
*.swo
*~

# ---------------------------------------------------
# OS Files
# ---------------------------------------------------
.DS_Store
Thumbs.db
desktop.ini

# ---------------------------------------------------
# Logs
# ---------------------------------------------------
logs/
*.log

# ---------------------------------------------------
# Celery
# ---------------------------------------------------
celerybeat-schedule
celerybeat.pid

# ---------------------------------------------------
# Docker
# ---------------------------------------------------
docker-compose.override.yml

# ---------------------------------------------------
# Poetry
# ---------------------------------------------------
poetry.lock

# ---------------------------------------------------
# uv
# ---------------------------------------------------
.uv/
uv.lock

# ---------------------------------------------------
# Pipenv
# ---------------------------------------------------
Pipfile.lock

# ---------------------------------------------------
# pyenv
# ---------------------------------------------------
.python-version

# ---------------------------------------------------
# Documentation Build
# ---------------------------------------------------
docs/_build/

# ---------------------------------------------------
# Temporary Files
# ---------------------------------------------------
tmp/
temp/
*.tmp

# ---------------------------------------------------
# Backup Files
# ---------------------------------------------------
*.bak
*.orig

# ---------------------------------------------------
# Node.js (for Django + Frontend projects)
# ---------------------------------------------------
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*
pnpm-debug.log*

# ---------------------------------------------------
# Frontend Build Outputs
# ---------------------------------------------------
.next/
.nuxt/
dist/
build/

# ---------------------------------------------------
# VSCode History
# ---------------------------------------------------
.history/
```

### Notes

In most production Django projects, you should **not commit**:

* `.env`
* `db.sqlite3`
* `media/`
* `staticfiles/` (the output of `collectstatic`)
* Virtual environments (`venv/`, `.venv/`, etc.)
* IDE settings (`.idea/`, `.vscode/`)

You should **usually commit migrations** to Git, so avoid adding `migrations/` to `.gitignore` unless you have a very specific workflow.

---

## License

MIT License

Copyright (c) 2026 Sajad Kholqi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
