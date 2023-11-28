# Project Descriptions

This guide will get you started with perception models. Each of the projects you can choose from will have you exploring perception models of different sorts.

## Getting started using AVstack

1. Install the `poetry` dependency manager: `curl -sSL https://install.python-poetry.org | python3 -`

1. Clone the `avdev-sandbox`.
```
git clone https://github.com/avstack-lab/avdev-sandbox.git --recurse-submodules
```

1. Install the python environment in the `avdev-sandbox` with `poetry install`.

1. Verify that some of the examples work:

1. Execute some of the basic tests to verify it works.
```
cd examples/hello_world
poetry run python hello_import.py
```

#### Troubleshooting

- If you install poetry but your systems says it is not found, you may need to add the poetry path to your path. On linux, this would be: `export PATH="$HOME/.local/bin:$PATH"`. I recommend adding this to your `.bashrc` or `.zshrc` file.
- Through an ssh connection, poetry may have keyring issues. If this is true, you can run the following: `export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring`



