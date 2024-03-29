Flake8 Typing Annotations Enforcement Plugin
============================================

Overview
--------

This Flake8 plugin is designed to enforce the usage of typing annotations in your Python code. By integrating this plugin into your Flake8 workflow, you can ensure that your codebase adheres to a consistent and explicit typing style, promoting better code readability and maintainability.

Features
--------

-   Type Annotation Enforcement: The plugin checks your Python code for functions, variables, and parameters that lack type annotations and raises warnings or errors accordingly.

-   Selective Ignoring: Use inline comments to selectively ignore the type annotation checks for specific lines or blocks of code.

Installation
------------

You can install this Flake8 plugin using pip:


`pip install flake8-enforce-type-annotations`

Usage
-----

After installation, the plugin becomes available as part of your Flake8 toolchain. Simply run Flake8 on your project to enforce typing annotations:


`flake8 your_project_directory`

### Configuration

You can configure the strictness of the enforcement by adjusting the plugin settings in your Flake8 configuration file (usually `.flake8`):


```[flake8]
per-file-ignores = 
    utils.py:ETA002,ETA001
```

### Inline Ignoring

If you need to bypass the type annotation checks for specific lines or blocks of code, you can use inline comments:


```# flake8: noqa
def unannotated_function():
    # ... code without type annotations
```

Contributing
------------

Contributions to this Flake8 plugin are welcome! If you encounter issues or have ideas for improvements, please open an issue or submit a pull request on the GitHub repository.

License
-------

This Flake8 plugin is distributed under the MIT License.
