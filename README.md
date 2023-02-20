Following below procedure to run the NFT-portal.
Prerequisites:
  Node.js installed on the local machine
  Ganache installed on the local machine
  Truffle installed on the local machine
  A code editor
Steps:
Unzip NFT-Portal project
Signup and Create Infura Web3 API project and copy API key and and configure in .env file under INFURA_API_KEY key.
Start Ganache UI and name the MNEMONIC and then restart the blockchain network, copy MNEMONIC name and configure in .env file under MNEMONIC key.
Create Metamask Wallet account and create "Goerli Test network and lead test ether".
Smart contract present in nft-portal/contracts/NFT.sol 
Deploy script present in nft-portal/migrations/2_deploy_contracts.js, compile and deploy the smart contract to Ganache using truffle command "truffle migrate --reset --network development"
Copy deployed smart contract address and configure in .env under REACT_APP_NFT_ADDRESS key, file present inside ./client folder.
Copy NFT.json from /build/contract to /client/src folder
Prepare Web application run "npm install" from /client path
Start the application by running "npm start"
Once React application starts, it's will ask permision to connect to Metamask wallet account,(approve and wallet will connect successfully with app)
Mint NFT by providing name, destribtion and image path.
