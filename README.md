## Installation

1. VS Code + Python Extension
1. Get RASA pro developer licence (add link)
1. Installation (link to the setup video)
    ```OSX
    brew install uv direnv
    eval "$(direnv hook zsh)"
    mkdir assistant && cd assistant
    git clone (link) .
    uv venv --python 3.11
    cat "RASA_LICENSE=YOURKEYHERE" > ~/.env
    direnv allow .
    uv pip install rasa-pro
    ```
1. Check it works with `rasa --version`

- TODO: Replace direnv with ".zshrc" env vars? Just add `source .env` in readme? 
- TODO: Add non-osx instructions