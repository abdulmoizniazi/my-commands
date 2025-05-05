``` bash
cd /c/enter/project/directory
python -m venv .venv
which python
source .venv/scripts/activate
which python
python -m pip install --upgrade pip
echo "*" > .venv/.gitignore
pip install "fastapi[standard]"
pip install sqlmodel
pip install -r requirements.txt
python main.py
deactivate
python main.py
---------------------------------------------------
---------------------------------------------------
Initialize git
git init
Add a remote repository
git remote add origin https://github.com/username/repository.git
Check status
git status
Add files to staging area
git add .                        git pull origin main --rebase
Commit the changes
git commit -m "Initial commit with analysis code"
Push the changes to the remote repository
git push origin main

Change directory to where you want to clone the repo
cd /c/Users/Dell/Desktop
Clone the repository
git clone https://github.com/username/repository.git
Navigate into the repository folder
cd repository   
---------------------------------------------------
---------------------------------------------------

Security
-4 security variables
-create security models
-hashing & token class instance
-> Hashing 
-> Matching 
-> Patching 

Database
-create models (class Hero)
-create engine (4 db variables)
-create tables (def)
-create session dependency (def)
-create database tables on startup (pof)
-create a hero (pof)
-read heroes (pof)
-read one hero (pof)
-delete a hero (pof)
-run the app (cli)

```
