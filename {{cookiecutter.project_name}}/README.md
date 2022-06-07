[![PyPI - Downloads](https://img.shields.io/pypi/dm/{{cookiecutter.project_name}})](https://pypi.org/project/{{cookiecutter.project_name}}/)
[![Documentation](https://img.shields.io/badge/Documentation-{{cookiecutter.project_name}}-blue)]({{cookiecutter.documentation_url}})
[![Pipeline status]({{cookiecutter.project_url}}/badges/main/pipeline.svg)]({{cookiecutter.project_url}}/-/pipelines/latest)
[![Coverage report]({{cookiecutter.project_url}}/badges/main/coverage.svg)]({{cookiecutter.documentation_url}}/htmlcov)

{{cookiecutter.description}}

# Installation
```shell
pip install git+{{cookiecutter.project_url}}.git
```

Any bug reports and feature requests are very welcome (see [issue tracker]({{cookiecutter.project_url}}/-/issues)).

# Setting up local test environment
First clone the repository:
```shell
pip install {{cookiecutter.project_url}}.git
```

Then, we install the package in an interactive manner:
```shell
cd {{cookiecutter.project_name}}
pip install -e .
```

Development tools can be installed using:
```
pip install -r requirements_dev.txt
pre-commit install  # installs pre-commit hooks to keep the code clean 
```


## Running tests
Tests are run using the [pytest](https://docs.pytest.org) framework. They can be run from the project root as:
```shell
pytest src/tests
```

## Compiling documentation
The documentation is build using [sphinx](https://www.sphinx-doc.org/en/master/). After installation (`pip install sphinx`) run:
```shell
cd doc
sphinx-build source build
open build/index.html
```

## Contributing
[Merge requests]({{cookiecutter.project_url}}/-/merge_requests) with any bug fixes or documentation updates are always welcome. 

For new features, please raise an [issue]({{cookiecutter.project_url}}/-/issues) to allow for discussion before you spend the time implementing them.

## Releasing new versions
- Run `bump2version` (install using `pip install bump2version`)
- Push to gitlab
- Manually activate the "to_pypi" task in the [pipeline]({{cookiecutter.project_url}}/-/pipelines/latest) to upload to pypi



