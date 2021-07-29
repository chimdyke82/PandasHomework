### Test Transactions

### Wallet 

## Description
-   This wallet is a tool that has been built to manage multiple crypto assets to serve numerous customers. For this test case, the wallet particularly manages the following crypto assets:

        -   ETH 
        -   BTCTEST

This wallet is built such that all the customer needs to have is a single mnemonic phrase and s/he is able to unlock and access all crypto asset in the portfolio. It is important that the mnemonic phrase is kept secret as it could lead to serious asset losses if it falls into the wrong hands.
## How to Use it
## What it is built with
-   This wallet was programmed using python language and built in the .php environment. This wallet was built using a `hd-wallet-derive` tool that supports not only BIP32, BIP39 and BIP44 but also supports other non-standard derivation paths for most wallets available today, making it the ideal 'universal wallet' that may be used to manage billions of addresses across a large proportion (300+) of cryptocurrencies. It is built in the .php environment and backend integrated with Python. 


## Installing HD-Wallet-Derive
### Step 1 - Setup Environment
The `hd-wallet-derive` tool is built using the PHP language. Your machine would therefore have to have the PHP environment needed for the tool to function.

### Step 2 - Installing the `HD-WALLET-DERIVE` Tool
> 1.    Open a fresh terminal. Windows users **must** open the terminal as administrator as shown below. If this is not done, the installation will not be successful!



> 2.    With the terminal open, navigate into the wallet folder and run the code below:

        git clone https://github.com/dan-da/hd-wallet-derive
        cd hd-wallet-derive
        curl https://getcomposer.org/installer -o installer.php
        php installer.php
        php composer.phar install

> 3.    A folder called `hd-wallet-derive` sontaining the .php library should now be created. 



### 