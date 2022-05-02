# hacksmith-tokens

## delete for a fresh start

```
hacksmith-tokens/artifacts
hacksmith-tokens/cache
hacksmith-tokens/node_modules
hacksmith-tokens/package-lock.json
```

## example.env and .env

```
hacksmith-tokens/example.env
hacksmith-tokens/.env
```

Copy `example.env` to `.env`, and fill it in. For rinkeby:

```
ETHEREUM_NETWORK=rinkeby
WALLET_PRIVATE_KEY=InsertLettersAndNumbersHere
ALCHEMY_API_KEY=InsertLettersAndNumbersHere
ETHERSCAN_API_KEY=InsertLettersAndNumbersHere
DEPLOYED_CONTRACT_ADDRESS=FillInAfterDeploying
```

Change for mainnet:

```
ETHEREUM_NETWORK=mainnet
...
```

## compile, deploy, verify, and mint

```
$ npm install
$ npx hardhat check-balance
$ npx hardhat compile
$ npx hardhat deploy
(then paste the deployed contract address into .env)
$ npx hardhat verify 0xDeployedContractAddress
$ npx hardhat mint --address 0xDestinationWalletToReceiveNewlyMintedNFT
```
