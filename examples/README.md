This directory contains a series of small examples apps that illustrate how to
code up common use cases for a Bitcoin Cash application.

The `low-level` directory
contains low-level applications exercising a single feature of BITBOX. Think of
these examples like lego blocks that can be used to build a bigger app.

The `applications` directory contains example applications like wallets, voting,
and other ideas.

## Installation
Prior to running these examples, you need to setup this code repository. In the
root directory run these commands:
```
npm install
npm build
npm postbuild
```

## Running Examples
You can run each example script by entering its directory and executing `npm start`

## Basic BCH Wallet Functions
These basic examples in the `applications/wallet` directory are used to bootstrap
a BCH testnet wallet for use with the other examples. Recommended path:
Create a wallet, fund it with a faucet, check the balance, then send some tBCH
back to faucet. Once those objectives are achieved, you're ready explore some of
the other examples.

* `create-wallet` Create a BCH compatible HD Node wallet on the BCH testnet.
Send test BCH using a testnet faucet (like
[this one](https://testnet.manu.backend.hamburg/bitcoin-cash-faucet) or
[this one](http://www.wormhole.cash/test/)) to the address saved in the
wallet.json file generated by this app.

* `check-balance` Check the balance of your BCH wallet. This displays both BCH
information as well as Wormhole token information.

* `send-bch` Send BCH to another address. (Great for sending balances back to
the testnet faucet.)
