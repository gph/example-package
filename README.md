# How to import your local package?

# Follow the steps below
1. [File structure](#package-structure)
2. [Create pyproject.toml](#create-pyprojecttoml)
3. [Install local package](#install-local-package)

## How to create a package?

### Package Structure
```commandline
packaging_tutorial/
├── LICENSE
├── pyproject.toml
├── README.md
├── src/
│   └── example_package_YOUR_USERNAME_HERE/
│       ├── __init__.py
│       └── example.py
└── tests/
```

### Create pyproject.toml
```toml
[project]
name = "example_package_YOUR_USERNAME_HERE"
version = "0.0.1"
authors = [
  { name="Example Author", email="author@example.com" },
]
description = "A small example package"
readme = "README.md"
requires-python = ">=3.7"
```

### Install local package
```commandline
pip install /path/to/project_directory
```

#### [pypa/sampleproject](https://github.com/pypa/sampleproject)