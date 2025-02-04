# build-social-media-dapp-on-core

# Prerequisites

* Node.js and npm installed
* MetaMask extension installed
* A private key from your MetaMask account
* Core Testnet account funded with test tokens

## 1. Setting Up the Environment Variables

* Create a `.env` file in the root directory of the project.
* Copy and paste the following line into the `.env` file:
```
PRIVATE_KEY=""
```
* Inside the quotes, paste your MetaMask account's private key. Make sure to keep this file secure and do not share your private key.

## 2. Deploying the Contract on Core Testnet

* Deploy your smart contract on the Core Testnet.
* Note down the deployed contract address, as you will need it in the next steps.

## 3. Configuring the Frontend

* Navigate to the `interface` folder located in the root directory.
* Inside the `src` folder, create a new folder named `ABI`.

```
mkdir -p interface/src/ABI
```
* Copy the Metacircle.json file from artifacts/contracts/Metacircle.sol/ and paste it inside the newly created ABI folder.
* Open the Web3Context.js file located in the src/context/ folder inside the interface directory.
* Find the following line in Web3Context.js:
```
const CONTRACT_ADDRESS = "<Contract-Address>";
```
Replace <Contract-Address> with your deployed contract address.
```
const CONTRACT_ADDRESS = "YOUR_DEPLOYED_CONTRACT_ADDRESS";
```
## 4. Deploying the Contract on Core Testnet
* Navigate to the interface directory.
* Install the required dependencies:
```
npm install
```
* Start the frontend dApp:
```
npm start
```
* Open your browser and navigate to http://localhost:3000 to view the dApp.

## Conclusion

Your frontend dApp should now be connected to your deployed contract on the Core Testnet and ready to use. If you encounter any issues, ensure that all steps have been followed correctly and that the .env file is properly configured.

