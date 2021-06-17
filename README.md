# Ethereum Max
* **Current Objective** - To add 3% burn, 3% reflect, 3% transaction fee


## PreRequisites
* Install Chrome, Firefox, Opera
* Install MetaMask
* Create MetaMask Test Wallet
* Generate Currency From Faucet for Test Wallet
* Install NodeJS
* Install TruffleJS
* Install Ganache


## Deploying To Test Net
* **_Single line view_**
	* `git pull --all; npm install; truffle compile; npx truffle migrate --compile-all --network ropsten --reset`
* Execute the command below to pull in all the most recent changes
    * `git pull --all`
* Execute the command below to install all dependencies fo project
    * `npm install`
* Execute the command below to compile smart contracts
    * `truffle compile`
* Execute the command below to deploy to testnet
    * `npx truffle migrate --compile-all --network ropsten --reset`

## Other Notes
### commands
* to compile scripts
    * `npx truffle compile`
* to do a deployment, but get ganache running locally!  I got it working with the windows app, not on the linux subsystem btw.
    * `npx truffle migrate`
    * if you get the error:  `Error: Artifacts are from different compiler runs` do not believe their lies about `--all`, instead, run: 
        * `rm -r build && npx truffle compile` unless that doesn't work then use `--all` as recommeneded.
* to deploy to ropsten:
    * `npx truffle migrate --compile-all --network  ropsten --reset`
* to deploy to mainnet:
    * `npx truffle migrate --compile-all --network mainnet --reset`
* to run verification
    * `truffle run verify :COIN_NAME --network :NETWORK_NAME`

* to run tests
    1. launch ganache
    2. `npx truffle test`



Click [here](https://docs.openzeppelin.com/upgrades-plugins/1.x/proxies#transparent-proxies-and-function-clashes)  to explain the 4 contracts, 'TransparentUpgradeableProxy'
