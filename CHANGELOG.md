# Changelog

## 0.1.1 - 2020/01/03 - HOTFIX collections.abc import error

- Though accessing the collection interfaces via `collections.abc`, the import was `collections` alone which meant that
abc became unaccessible in python 3.8.0.
- Now explicitly importing `collections.abc`

## 0.1.0 - 2020/01/03 - Initial build of pyini

- Implemented the base functionality of the ini config standard.
- Extended the standard to allow for nested sections via intentation.
- Extend standard to define a typing system for settings.
- Extend typing system to allow for sub-typing of container classes - allowing for initialisation and loading of container objects with complex objects.
- Add functionality to write config, either to string, filepath or handle given.
- Add interpolation of settings within the config
- Add eval as an type to allow for dynamically defined settings - along with a safetly parameter to ensure that malicious no arbitary code execution is performed.
