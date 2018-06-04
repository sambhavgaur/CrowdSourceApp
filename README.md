# CrowdSource-App
MacOX —
brew update
brew upgrade

brew tap ethereum/ethereum
brew install ethereum

git clone https://github.com/enterprise-blockchain-book/first-edition

Navigate to /crowdsource-app/ethereum/setup/start.json

geth --datadir=./data init start.json


geth --networkid 999 --ipcpath ~/Library/Ethereum/geth.ipc --rpc --rpcaddr "127.0.0.1" --rpcapi="db,eth,net,web3,personal,web3" --rpcport "8545" --datadir=./data --rpccorsdomain "*" console

>web3.personal.newAccount(“password”);
>web3.personal.listAccounts
> web3.fromWei(eth.getBalance(eth.coinbase));

Open New Terminal 
geth attach ~/Library/Ethereum/geth.ipc

miner.start(2)

main account should have around 1500 ethers
miner.stop()

Install Ethereum Wallet ——

Add Wallet.
Initiate transaction(password should be of main wallet which was created on console earlier)

After creating few accounts, deploy contract.

Copy Crowdsource contract from contract directory and deploy. it should work and you may use its methods.
.

