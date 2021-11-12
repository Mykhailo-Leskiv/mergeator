# mergeator
## Description
Checks whether the current branch has changes in the files that had been changed in the branches from PRs to the main branch
## Prerequisites
    $ curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo gpg --dearmor -o /usr/share/keyrings/githubcli-archive-keyring.gpg
    $ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null
    $ sudo apt update
    $ sudo apt install gh
    $ gh auth
## Install
    $ ./install.sh
## Usage
    $ mergeator <main_branch> (default master)
## Output example
**branch-1, branch-2** branches have changes in file(s) **src/api/default.py**
