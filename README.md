# Fantasy Name Generator

[![PyPI version](https://badge.fury.io/py/fantasynames.svg)](https://badge.fury.io/py/fantasynames)

A random name generator that produces names aligning (more or less) with common conventions for fantasy characters in fictional media such as Dungeons and Dragons or World of Warcraft.

## Installation

`python3 -m pip install fantasynames`

## Usage

The following name generating functions are provided for a variety of different stereotypical fantasy "races", as well as a few different "medieval-y" languages:

```python
import fantasynames as names

names.elf()
# Example outputs: 'Farathia Eaviel', 'Iethian Willowblossom'

names.dwarf()
# Example outputs: 'Thrunnor Ironfury', 'Lothuna Strongmail'

names.hobbit()
# Example outputs: 'Libby Honeyfoot', 'Flublius Sweetscone'

names.french()
# Example outputs: 'Auland Roublac', 'Rondri de Clardalle'

names.anglo()
# Example outputs: 'Brandin of Avonlyn', 'Kallem Davenmere'

names.human()
# Example outputs: 'Danric du Tourbloc', 'Sumia Sageholme'
```

Note that `human()` provides a diverse mix of different first and last name styles, including `anglo()` and `french()`...and more!

## Contributing

### Poetry

This package uses [Poetry](https://python-poetry.org/) for package management. After checking out the repo, use `poetry install` to install all the required dependencies. Anytime you need to add a package, instead of `pip install`, use:

```
poetry add <PACKAGE_NAME_HERE>
```

### Linting / Formatting

We do code formatting with [Python Black](https://github.com/psf/black). Before opening a PR, make sure to format your code by running:

```
poetry run black fantasynames
```

Please also run `flake8` to catch any remaining problems:

```
poetry run flake8
```

### Guides

For guides on how to make your own name generators, check out the [How to Add a New Name Generator Guide](docs/new-generator-guide.md). And then if you want to ramp up the complexity, take a look at the [Transformation Guide](docs/transformation-guide.md).