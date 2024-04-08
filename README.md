# staking-deposit-cli

> [!IMPORTANT]  
> This CLI tool is a forked version specifically for **Endurance Network**. You can choose the **mainnet** as a parameter for use with Endurance.

#### Build `deposit-cli` with `virtualenv`

##### Step 0. Python version checking

Ensure you are using Python version >= Python3.8:

```sh
python3 -V
```

##### Step 1. Installation

For the [virtualenv](https://virtualenv.pypa.io/en/latest/) users, you can create a new venv:

```sh
pip3 install virtualenv
python3 -m virtualenv venv
source venv/bin/activate
```

and install the dependencies:

```sh
python3 setup.py install
pip3 install -r requirements.txt
```

##### Step 2. Create keys and `deposit_data-*.json`

Run one of the following command to enter the interactive CLI:

```sh
python3 ./staking_deposit/deposit.py new-mnemonic
```

or

```sh
python3 ./staking_deposit/deposit.py existing-mnemonic
```

You can also run the tool with optional arguments:

```sh
python3 ./staking_deposit/deposit.py new-mnemonic --num_validators=<NUM_VALIDATORS> --mnemonic_language=english --chain=mainnet --execution_address=<YOUR_WITHDRAW_ADDRESS>
```

```sh
python3 ./staking_deposit/deposit.py existing-mnemonic --num_validators=<NUM_VALIDATORS> --validator_start_index=<START_INDEX> --chain=mainnet --folder=<YOUR_FOLDER_PATH> --execution_address=<YOUR_WITHDRAW_ADDRESS>
```
