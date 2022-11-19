Homework 17
1. Create a fork of mainnet (details below)
2. On the command line check the current block height, is this what you expected ?
3. Can you transfer ETH from one of Vitalik's accounts to your own account ?
Creating a fork of mainnet
See also lesson 9
See hardhat documentation
You first need to have an account on Infura or Alchemy
This will give you a key so that you can use their RPC nodes.
Forking using ganache
npx ganache-cli --f https://mainnet.infura.io/v3/<your key> -m
“your 12 word mnemonic” --unlock <address> -i <chain ID>
Fork from hardhat
npx hardhat node --fork https://eth-
mainnet.alchemyapi.io/v2/<your key>
In hardhat you can also specify this in the config file
networks: {
hardhat: {
forking: {
url: "https://eth-mainnet.alchemyapi.io/v2/<key>",
}
}
}
