Following below procedure to run the NFT-portal.


Prerequisites:

  1.Node.js installed on the local machine.
  
  2.Ganache installed on the local machine.
  
  3.Truffle installed on the local machine
  
  4.A code editor


Steps:

1.Unzip NFT-Portal project.

2.Signup and Create Infura Web3 API project and copy API key and and configure in .env file under INFURA_API_KEY key.

3.Start Ganache UI and name the MNEMONIC and then restart the blockchain network, copy MNEMONIC name and configure in .env file under MNEMONIC key.

4.Create Metamask Wallet account and create "Goerli Test network and lead test ether".

5.Smart contract present in nft-portal/contracts/NFT.sol.

6.Deploy script present in nft-portal/migrations/2_deploy_contracts.js, compile and deploy the smart contract to Ganache using truffle command "truffle migrate --reset --network development".

7.Copy deployed smart contract address and configure in .env under REACT_APP_NFT_ADDRESS key, file present inside ./client folder.

8.Copy NFT.json from /build/contract to /client/src folder.

9.Prepare Web application run "npm install" from /client path

10.Start the application by running "npm start".

11.Once React application starts, it's will ask permision to connect to Metamask wallet account,(approve and wallet will connect successfully with app).

12.Mint NFT by providing name, destribtion and image path.
