# Multi-Asset Crypto Wallet Project

## Description
-   This wallet is a tool that has been built to manage multiple crypto assets to serve numerous customers. For this test case, the wallet particularly manages the following crypto assets:

        -   ETH 
        -   BTCTEST

This wallet is built such that all the customer needs to have is a single mnemonic phrase and s/he is able to unlock and access all crypto asset in the portfolio. It is important that the mnemonic phrase is kept secret as it could lead to serious asset losses if it falls into the wrong hands.

## What it is built with
-   This wallet was programmed using python language and built in the .php environment. This wallet was built using a `hd-wallet-derive` tool that supports not only BIP32, BIP39 and BIP44 but also supports other non-standard derivation paths for most wallets available today, making it the ideal 'universal wallet' that may be used to manage billions of addresses across a large proportion (300+) of cryptocurrencies. It is built in the .php environment and backend integrated with Python. 

## How to Use it



## **Installing HD-Wallet-Derive**
### Step 1 - Setup Environment
The `hd-wallet-derive` tool is built using the PHP language. Your machine would therefore have to have the PHP environment needed for the tool to function.

### Step 2 - Installing the `HD-WALLET-DERIVE` Tool
> 1.    Open a fresh terminal. Windows users **must** open the terminal as administrator as shown below. If this is not done, the installation will not be successful!

![Admin-terminal](Images/administrator.jpg)

> 2.    With the terminal open, navigate into the wallet folder and run the code below:

        git clone https://github.com/dan-da/hd-wallet-derive
        cd hd-wallet-derive
        curl https://getcomposer.org/installer -o installer.php
        php installer.php
        php composer.phar install

> 3.    A folder called `hd-wallet-derive` sontaining the .php library should now be created. 

## Using The Wallet
### Setup Constants
-   Update the `constants.py` file to reflect the cyrptocurrencies of interest. 

### Setup the `MNEMONIC` and Derive Wallet keys
-   Open the `.env` file located in the folder and update the mnemonic and importing into the wallet.py.



## **Transacting**
1. Confirm the `priv_key_to_account` function details. Update the `priv_key_to_account` function with the coin (either ETH or BTCTEST) and private key details of the sending or originating account. This function converts a ~priv_key~ (private key) to the `account` variable that is an input to the actual `send_tx` function.
![Private_Key](Images/privkey_code.jpg)


2. The `send_tx` code is a function that requires four parameters:
![Send_code](Images/send_code.jpg)
    
 
- **coin**: The crypto asset to be transacted, either ETH or BTCTEST.
- **account**: The originating account.
- **to**: The receiving account.
- **amount**: The amount to be transacted (sent).

These parameters have to be inputted for the transaction to be successful. An example is shown:

![Send_example](Images/send_examp.jpg)


![Successful_Txn](Images/txn.jpg)

### Test Transactions
The Private Key of the sender account was inputted into MyCrypto to unlock the account as shown below:
![Unlock Account](Images/Unlock.jpg)
Click the unlock button and it reveals the funded account.
![Unlock Account](Images/Unlocked_Account.jpg)

Insert the transfer details - receipt account and amount. Click on the Tx Status on left menu list to see the status of the transaction.
![Successful_Txn](Images/Txn_Pending.jpg)
When completed, the Transaction status should change to **SUCCESSFUL**.
![Successful_Txn](Images/Eth_Txn_Confirmed.jpg)