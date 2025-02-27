# Abachi Smart Contracts

## Table of Contents
- [Required Tools](#required-tools)
- [Getting Started](#getting-started)
- [Contracts](#contracts)
- [Contribution](#contribution)


## Required Tools
* Node v14
* Git

## Getting Started

#### Setup
```
git clone https://github.com/abachi-io/abachi-presale-contracts.git

cd abachi-presale-contracts

npm i

cp .env.example .env
```

* Edit `.env` file
* Edit scripts/deployAll.js and fill out `//required` addresses

#### Compile Contracts

`npx hardhat compile`

#### Deploy

`npx hardhat run scripts/deployAll.js --network [NETWORK]`

#### Verify Contracts on Etherscan/Polyscan (optional)

`npx hardhat verify --network [NETWORK] [CONTRACT ADDRESS] [CONSTRUCTOR PARAM 1] [CONSTRUCTOR PARAM 2]`

#### Test contracts
`npx hardhat test`

* To test using a local chain, add a comma separated list of private keys from the local rpc server
* Update default network in hardhat config file to `localhost`

## Contracts

#### Matic Mainnet (Polygon)

|       Contract    | Address |
|     ------------- | ------------- |
| aAbachi           | [0xcC649F54645f09751b3f3E7BeF57aBfD6A8885dc](https://polygonscan.com/address/0xcC649F54645f09751b3f3E7BeF57aBfD6A8885dc)   |
| presaleAbachi     | [0x860AB14370f3a99C6d7F834bdc99D5a117489f96](https://polygonscan.com/address/0x860AB14370f3a99C6d7F834bdc99D5a117489f96)  |
| DAI               | [0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063](https://polygonscan.com/address/0x8f3Cf7ad23Cd3CaDbD9735AFf958023239c6A063)  |

## Contribution

Thank you for considering to help out with the source code! We welcome contributions from anyone on the internet, and are grateful for even the smallest of fixes!

If you'd like to contribute to Abachi, please fork, fix, commit and send a pull request for the maintainers to review and merge into the main code base.

Please make sure your contributions adhere to our coding guidelines:

* Pull requests need to be based on and opened against the master branch.
* Pull request should have a detailed explanation about the enhancement or fix
* Commit messages should be prefixed with the file they modify.

Please see the [First Contributer's Guide](documentation/CONTRIBUTE.md) for more details on how to configure your git environment.
