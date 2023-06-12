DO NOT USE YET

# RepoChainSync

coming

## Features

- Compare bytecodes of contracts with on-chain deployed contracts.
- Supports checking runtime bytecode with or without appended CBOR bytecode hash metadata.
- Automatically extracts contract names and addresses from deployment transactions.
- Interactive conflict resolution for duplicate contract addresses.
- Easily extensible to support additional contract comparison features.

## Installation

Setup a virtual environment first

```zsh
pip install virtualenv
virtualenv .venv
source .venv/bin/activate
```

Now install dependencies

```zsh
pip install -r requirements.txt
```

## Usage

Check the last cell in the ipynb for an example. Replace values accordingly.

```zsh
jupyter nbconvert --to script compare_bytecode.ipynb
```

```zsh
python compare_bytecode.py
```
