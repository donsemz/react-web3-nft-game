# A React Vite App NFT client using Avalanche and Core Wallet intergration

### Live Site Available Here: https://adorable-brioche-fba06c.netlify.app/

## The app is built using:
1. HTML, CSS, JS, React
2. Avalanche
3. Hardhat
4. Sollidity
5. Tailwindcss

## Functionalities Implemented:
1. Users can Play with their friends online using Game NFTs and Smart Wallets
2. Users can Attack and defend in the game
3. Users can also generate Health points (HP)
4. Users can create a room and play against their friends in them.

## The App demonstrates:
1. Hardhat and solidity to define and deploy smart contracts
2. The ability to deploy smart contacts on Web3 and utilize its implementations.
3. Responsiveness with pure CSS tailwind
4. Make API requests
7. Error Handling
8. Clean SOLID Principles in coding
9. Data Management and Display

## App Screenshots

### Landing page:
<img width="1386" alt="Screen Shot 2023-02-01 at 17 00 08" src="https://user-images.githubusercontent.com/20219448/216390519-f0ce07fd-c907-4a67-a683-f347e51fc8fd.png">

### Battlegrounds
<img width="954" alt="Screen Shot 2023-02-01 at 17 00 23" src="https://user-images.githubusercontent.com/20219448/216390673-2c37e621-8a4b-45a6-bf92-632831c67ac1.png">

### Battles
<img width="624" alt="Screen Shot 2023-02-01 at 17 03 07" src="https://user-images.githubusercontent.com/20219448/216390766-f6716a65-bdef-4962-aa6b-848391f6691d.png">


## Instructions on setting up the Web3 part of the project
0. `cd web3`
1. `npx hardhat` -> y → typescript → enter → enter
2. `npm install @openzeppelin/contracts dotenv @nomiclabs/hardhat-ethers` + Hardhat packages `npm install --save-dev "hardhat@^2.12.0" "@nomicfoundation/hardhat-toolbox@^2.0.0"`
3. Install [Core](https://chrome.google.com/webstore/detail/core/agoakfejjabomempkjlepdflaleeobhb), a Metamask smart wallet alternative built for Avalanche dApps
  1. Turn on the testnet mode by: opening up the Core extension -> click the hamburger menu on the top left -> go to advanced -> turn on the testnet mode
4. Fund your wallet from the [Avax Faucet](https://faucet.avax.network/)
5. Create a `.env` file and specify a PRIVATE_KEY variable.
6. To get to the private key, do the following steps:
  1. Open up the Core extension -> click the hamburger menu on the top left -> go to security and privacy -> click show recovery phase -> enter your password -> copy the phrase -> go to [wallet.avax.network](https://wallet.avax.network/) -> click access wallet -> choose mnemonic key phrase -> paste what the words we’ve copied from Core -> on the sidebar click manage keys -> view c-chain private key -> copy -> paste it in the .env file
7. Copy the `hardhat.config.ts` file from the GitHub gist down in the description
8. Copy the `deploy.ts` script from the GitHub gist down in the description
9. Copy the `AvaxGods.sol` smart contract code from the GitHub gist down in the description
10. Compile the contract by running the `npx hardhat compile` command
11. Deploy the smart contract on the Fuji test network by running the `npx hardhat run scripts/deploy.ts --network fuji` command
  Move the `/artifacts/contracts/AVAXGods.json` file to the `/contract` folder on the frontend
  Copy the address of the deployed contract from the terminal and paste it into the `/contract/index.js` file of the frontend application
  
