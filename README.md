# Python Sample Project

This project was originally to learn Azure Pipelines.
But it has now evolved into a baseline for the boilerplate required for Python projects.
Eventually this will be used to update my Python Cookiecutter Template.

Features:
- Reproducible testing in any CI pipeline by leveraging containers.
- Continuos Integration preconfigured:
  - Azure Pipeline
- Pyproject.toml (PEP 517/518)
- Tests
  - Tox
  - Unit Testing (PyTest)
  - Linting (pytest)
  - Styling (Black and isort)
  - Typing (pytype)
  - Packaging (pyroma)

## Pipenv
### Aliases

* build       - creates source and binary wheel
* cleanup     - stops and destroys running containers and volumes, and deletes temporary files
* dockerbuild - updates docker images
* publish     - push wheels to PyPI
* tests       - runs tox (in a container if docker-compose is available)

#### Running tests

Example:
```sh
TOXENV=lint pipenv run tests
```

## To Dos

- [ ] Travis CI
- [ ] Gitlab CI
- [ ] Publishing to PyPI
- [ ] Testing to Test PyPI
- [ ] Sphinx doc generation
- [ ] setup.py [ tests, deploy ]
- [ ] Doctest
- [ ] Towncrier
- [ ] Contributors (from Git, ordered by commits)
- [ ] Manifest.in
- [ ] Github Templates
- [ ] Gitlab Templates