# Contract Info
[CryptoZombies](https://rinkeby.etherscan.io/address/0xB4fdb624Ba48d78Da8aA91E3E05A45358fE08BF0): 0xB4fdb624Ba48d78Da8aA91E3E05A45358fE08BF0

## To Set Up Dev Environment:
Within the root directory of this project, do the following:

1. Add a **.env** file with two values:
MNEMONIC="seed words go here"
INFURA_URL=https://rinkeby.infura.io/v3/ACCESS_TOKEN_GOES_HERE

MNEMONIC is equal to the 12 seed words that were generated when you generated a private key using a tool like Meta Mask.
INFURA_URL is equal to the https://rinkeby.infura.io/v3/ + your access token

2. Run `npm install truffle truffle-hdwallet-provider dotenv`

## To (Re)deploy Contract:

Use Truffle Console to deploy:

1. `truffle console --network rinkeby`
2. `migrate`

## To Interact with the Contract using Truffle Console:

1. `truffle console --network rinkeby`
2. Find deployed contracts and their addresses: `networks` (Note you will see the contract address listed next to 'CryptoZombies')
3. Access your deployed contract instance: `CryptoZombies.deployed();`
4. Make a new zombie `CryptoZombies.deployed().then(instance => instance.createRandomZombie("ZOMBIE NAME"));`