# salt-lsp

[![Continous Integration](https://github.com/dcermak/salt-lsp/actions/workflows/ci.yml/badge.svg)](https://github.com/dcermak/salt-lsp/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/dcermak/salt-lsp)](https://app.codecov.io/gh/dcermak/salt-lsp)

Salt Language Server Protocol Server


## Prerequisites

- Python >= 3.8
- VSCode (required for live testing the server from an editor)


## Setup

Setup & start the server:

```ShellSession
$ python3 -m venv .env3
$ . .env3/bin/activate
$ pip install -r requirements.txt -r dev-requirements.txt
```

Create the completion classes once:

```ShellSession
$ ./create_completion_classes.py
```

Start the server:

```ShellSession
$ ./lsp_server.py --tcp
```

Launch the client:

1. Run `yarn install`
2. Start VSCode and open this directory as the server
3. Open the Debug menu (Ctrl + Shift + D)
4. Select "Launch Client" drop down
5. Press F5
