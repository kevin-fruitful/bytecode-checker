# CompareBytecode

CompareBytecode is a Python package designed to aid Ethereum blockchain developers and auditors. Its primary feature is to compare the bytecodes of contracts, both locally and on-chain, to ensure consistency and aid in contract upgradeability verification.

CompareBytecode uses the Web3.py library. It is currently primarily designed to work with Diamond Standard contracts (EIP-2535) but can be used with any Ethereum contract.

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
