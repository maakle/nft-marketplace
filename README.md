# NFT marketplace

To get this project running locally you need Node as well as Metamask in your browser.

## Install dependencies

Please run the following inside the project directory.

```shell
yarn
```

## Run

### Deploy smart contracts

In a new terminal window inside the project, run the following command:

```shell
npx hardhat node
```

This will create a few test accounts with 10.000 ETH. Copy 2-3 and add them to Metamask to interact later with the App.

Also, create a file `.secret` in your project's root directory and add one of the account's private keys in there.

In a separate terminal window inside the project, run the following command:

```shell
npx hardhat run scripts/deploy.js --network localhost
```

This will deploy the smart contracts to a local testnet. It should print something like this in your console:

```shell
nftMarket deployed to: 0x5FbDB2315678afecb367f032d93F642f64180aa3
nft deployed to: 0xe7f1725E7734CE288F8367e1Bb143E90bb3F0512
```

Copy those addresses into the file `config.js` in the project root directory.

### Run App

Run the following command to start the app on `http://localhost:3000`

```shell
yarn dev
```
