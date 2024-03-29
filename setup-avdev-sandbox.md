(optional) Run the following to change your shell to zsh/ohmyzsh
```
sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install -y git zsh curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Run the following to install the avdev sandbox on a new machine (preferably Ubuntu 22.04)

```
sudo apt-get update && sudo apt-get upgrade -y
sudo apt-get install -y git wget curl ffmpeg libsm6 libxext6 build-essential
curl -sSL https://install.python-poetry.org | python3 -
export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
export PATH="$HOME/.local/bin:$PATH"
mkdir -p ~/Documents/AVstack/sandboxes && cd ~/Documents/AVstack/sandboxes
git clone --recurse-submodules https://github.com/avstack-lab/avdev-sandbox/
cd avdev-sandbox
poetry install --no-root
poetry run python examples/hello_world/hello_import.py
```
