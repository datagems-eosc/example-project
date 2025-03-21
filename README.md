# example-project

[![Commit activity](https://img.shields.io/github/commit-activity/m/datagems-eosc/example-project)](https://img.shields.io/github/commit-activity/m/datagems-eosc/example-project)
[![License](https://img.shields.io/github/license/datagems-eosc/example-project)](https://img.shields.io/github/license/datagems-eosc/example-project)

This is a template repository for DataGEMS Python projects that uses uv for their dependency management.


## Getting started with your project

### 1. Create a New Repository

First, create a repository on GitHub with the same name as this project, and then run the following commands:

```bash
git init -b main
git add .
git commit -m "init commit"
git remote add origin git@github.com:datagems-eosc/example-project.git
git push -u origin main
```

### 2. Set Up Your Development Environment

Then, install the environment and the pre-commit hooks with

```bash
make install
```

This will also generate your `uv.lock` file

### 3. Run the pre-commit hooks

Initially, the CI/CD pipeline might be failing due to formatting issues. To resolve those run:

```bash
uv run pre-commit run -a
```

### 4. Commit the changes

Lastly, commit the changes made by the two steps above to your repository.

```bash
git add .
git commit -m 'Fix formatting issues'
git push origin main
```

---

The uv-python cookiecutter was originally created in [https://github.com/fpgmaas/cookiecutter-uv](https://github.com/fpgmaas/cookiecutter-uv).
