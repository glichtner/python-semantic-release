# python-semantic-release [![Build status](https://github.com/relekang/python-semantic-release.svg)][last-build] [![Coverage status](https://ci.frigg.io/relekang/python-semantic-release/coverage.svg)][last-build]

Automatic semantic versioning for python projects

> **This is not usable, yet.**

## Install
```
pip install semantic-release
```

## Usage
The general idea is to have some sort of tag in commit messages that indicates certain types of changes.
If a commit message lack a tag it is ignored. Running release can be run locally or from a CI service.

Creating a new release: `$ semantic-release version`

### Configuration
All configuration described here belongs in `setup.cfg` in a section: `semantic-release`.

#### Tags
There are a set of tags used to evaluate the changes from commit messages. They can be configured
to meet what you want them to be. The different tags are listed below with their defaults.

* **Major change:** `:boom:` :boom:
* **Minor change:** `:sparkles:` :sparkles:
* **Patch change:** `:bug:` :bug:
* **Upgrade dependency:** `:arrow_up:` :arrow_up: (will trigger minor version change)


[last-build]: https://ci.frigg.io/relekang/python-semantic-release/last/