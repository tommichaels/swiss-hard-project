# LearnWeb3DAO <> Swisstronik Challenge

This project demonstrates a simple Hardhat x Swisstronik use case. It consists of a simple solidity smart contract which sets and gets a message (string) and three scripts that deploys the "contract", sets and gets a message(i.e the message that was set).

## Task 
Deploy a smart contract using Hardhat on the Swisstronik network.

## Overall Usage
```
npm install --save-dev hardhat
npx hardhat
npm install --save-dev @nomicfoundation/hardhat-toolbox
npm i @swisstronik/swisstronik.js
npx hardhat compile
npx hardhat run scripts/deploy.js --network swisstronik
npx hardhat run scripts/setMessage.js --network swisstronik
npx hardhat run scripts/getMessage.js --network swisstronik
```

## 1. Smart Contract Deployed
```
EVM : 0xf84Df872D385997aBc28E3f07A2E3cd707c9698a
```

### TX Deploy Smart Contract
```
https://explorer-evm.testnet.swisstronik.com/tx/0x095888ada3ed4986dbebb701965e37ac234897e5938533496e71c38b418177b6
```

## 2. Deploy code in scripts/deploy.js
```
npx hardhat run scripts/deploy.js --network swisstronik 
```

## 3. Interact with the contract - Transaction
```
npm i @swisstronik/swisstronik.js
```
Create File setMessage.js in folder Scripts

```
npx hardhat run scripts/setMessage.js --network swisstronik
```

### TX interact - Transaction
```
https://explorer-evm.testnet.swisstronik.com/tx/0x7238ecf7885503a8c9df462997933a88910e234efab4454a5f0d721873cf0f9e
```

## 4. Interact with the contract - Call

Create File getMessage.js in folder Scripts

```
npx hardhat run scripts/getMessage.js --network swisstronik
```

> Decoded response: Hello Swisstronik!!
