# Project Documentation Setup

## Prerequisites
- Python installed
- Poetry installed

---

## Getting Started

### 1. Initialize the Project
```bash
poetry init
```

### 2. Create Virtual Environment Inside Project Folder
```bash
poetry config virtualenvs.in-project true
poetry config virtualenvs.in-project true --local
```

### 3. Activate the Virtual Environment
```bash
eval $(poetry env activate)
```

### 4. Add MkDocs Material Dependency
```bash
poetry add mkdocs-material
```

---

## Development

### Build Documentation
```bash
mkdocs build
```

### Run Documentation Locally
```bash
mkdocs serve --watch-theme --dev-addr 0.0.0.0:8080
```

> **Tip:** Open `http://0.0.0.0:8080` in your browser to preview.  
> Run `mkdocs -h` to print help and exit.

---

## Git Setup

### New Repository (First Time)
```bash
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin git@github.com:rs2151/rs2151.github.io.git
git push -u origin master
```

### Existing Repository
```bash
git remote add origin git@github.com:rs2151/rs2151.github.io.git
git branch -M master
git push -u origin master
```

### Push Code Changes
```bash
git remote -v
git add .
git commit -m "your commit message here"
git push
```

Note: Update the Repo

`git remote set-url origin git@github.com:rs2151/ramsharma.git`

---

## Deploy to GitHub Pages

```bash
mkdocs gh-deploy --force
```

> After deploying, wait **2 minutes** and refresh your GitHub Pages URL.  
> Site will be live at: `https://rs2151.github.io/`