# WORK IN PROGRESS

## Branches

- Branch [`main`](https://github.com/HadesArchitect/RasaDevXie/tree/main) is all about the DevXie assistant
- Branch [`tutorial`](https://github.com/HadesArchitect/RasaDevXie/tree/tutorial) is for tutorial related content

## Tags

Use git tags to navigate between different stages of the assistant.

- `initial` - Installation complete, nothing is implemented
- `tutorial-1` - Initial state after `rasa init --template tutorial`
- `tutorial-2` - `tutorial-1` + `rasa train; rasa inspect`
- `tutorial-3` - `tutorial-2` + further modifications
- `devxie-1` - First MVP (report an issue)

## Installation

1. VS Code + Python Extension
1. Get RASA pro developer licence (add link)
1. Installation (link to the setup video)
    ```OSX
    brew install uv direnv
    eval "$(direnv hook zsh)"
    mkdir assistant && cd assistant
    git clone git@github.com:HadesArchitect/RasaDevXie.git .
    uv venv --python 3.11
    echo "RASA_LICENSE=YOURKEYHERE" > .env
    direnv allow .
    uv pip install rasa-pro
    ```
1. Check it works with `rasa --version`.

- TODO: Replace direnv with ".zshrc" env vars? Just add `source .env` in readme? 
- TODO: Add non-osx instructions
