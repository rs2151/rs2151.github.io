Initialize the Project

```commandline
poetry init
```

Run the below to create the VENV inside your project folder

```commandline
poetry config virtualenvs.in-project true
```

```commandline
poetry config virtualenvs.in-project true --local
```

```commandline
eval $(poetry env activate)
```

```commandline
poetry env info --path
```

To activate a virtual environment (venv) managed by Poetry

For more info visit [Poetry ENV](https://python-poetry.org/docs/managing-environments/#bash-csh-zsh)

List the ENV

```commandline
poetry env list
```

```commandline
poetry install
```

Add Django Dependency

```commandline
poetry add django
```

### Install the mkdocs-material (for new project)

```
pip install mkdocs-material
```

### Install the all requirements with the below CMD if already developed

- pip install -r requirements.txt

---

### Bulid your DOC pages

- mkdocs build

---

### Run the DOC

- mkdocs serve --watch-theme --dev-addr 0.0.0.0:8080
- mkdocs -h - Print help message and exit.
---

### Sync the code github master branch newly created

- git init
- git status
- git add .
- git commit -m "Some Msgs"
- git remote add origin git@github.com:rs2151/rswiki.git
- git push -u origin master / git push

### Sync the code github master branch already created

- git remote -v
- git add .
- git commit -m "Your commit message here"
- git push -u origin master / git push

### How to Deploy the webiste on github

<!-- - mkdocs gh-deploy  for newly deployment-->
- mkdocs gh-deploy --force
- After that wait for 2 mins and refresh the Pages.

### How to freeze the packages of this env

```
pip freeze > requirements.txt
