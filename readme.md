#Contract Info#
[CryptoZombies](https://rinkeby.etherscan.io/address/0xB4fdb624Ba48d78Da8aA91E3E05A45358fE08BF0): 0xB4fdb624Ba48d78Da8aA91E3E05A45358fE08BF0

##To (Re)deploy:##

Use Truffle Console to deploy:

1. `truffle console --network rinkeby`
2. `migrate`

To Interact with the contract using Truffle console:

1. `truffle console --network rinkeby`
2. Find contract address: `networks` (Note you will see the contract address listed next to 'CryptoZombies')
3. Access your deployed contract instance via: `CryptoZombies.deployed();`
4. Make a new zombie `CryptoZombies.deployed().then(instance => instance.createRandomZombie("ZOMBIE NAME"));`