Cookiecutter to create a python package uploaded to the WIN/FMRIB gitlab server.

# Features
Gitlab continuous integration with
- pytest runner with coverage
- documentation deployment
- manual uploading to pypi

# Usage
```shell
cookiecutter https://github.com/MichielCottaar/cookiecutter-pypackage.git
```

Afterwards enter the repository and create the initial commit:
```shell
cd <project_name>
git init
git add .
git commit -m "Files from cookiecutter"
```

Then, set up pre-commit to check for any style errors:
```shell
pre-commit install
pre-commit autoupdate
pre-commit run --all-files
```
