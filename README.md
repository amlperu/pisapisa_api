# pisapisa_api

# Create the repository in GitHub
```bash
git clone https://github.com/amlperu/pisapisa_api.git
cd pisapisa.api
```

## Setup virtual environment
```bash
python -m venv venv
source venv/Scripts/activate
```

## Install dependencies
```bash
pip install Django
```

## Create project configuration files
```bash
django-admin startproject config .
```

## Create the file and save dependencies
```bash
pip freeze > requirements.txt
```

## Test it works
```bash
python manage.py runserver
# open http://127.0.0.1:8000/ and verify if you see message "The install worked successfully! Congratulations!"
```

## Configure Timezone
```bash
#Open settings.py
change the line TIME_ZONE from 'UTC' to 'America/New_York'
```

## Update .gitignore
```bash
open .gitignore
add the following lines at the end:
venv/
.env
db.sqlite3
**__pycache__/ #to add the pycache fron any folder
```
## First commit
```bash
git add .
git status  # Verify venv/ is NOT listed
git commit -m "chore: initial Django setup"
git push origin main
```