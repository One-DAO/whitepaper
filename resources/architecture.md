# Architecture

![](<../.gitbook/assets/Tech Stack.png>)

## Components

Our token ecosystem is broken up into separate component areas. The marketplace for NFTs, and personalized arena hub and feed. The hub is an overview of the owner's arena including any custom NFTs, current and past contests and social feed, Discord integrations and filtered marketplace for reselling and trading by fans.

![](<../.gitbook/assets/Architecture Components.png>)

* Owners will mint their ASSETS using the custom NFT builder that's linked to the ERC-1155 token for the respective ARENA.
* The ASSETS are uploaded to IPFS via Pinata Cloud.
* Metamask is a Web3 provider which acts as the intermediary between the user and blockchain

### Front-End

Frontend is developed with React and Node.js.

Wallet integration is done via Metamask, Bitski, Wallet Connect, Trust Wallet, etc. These wallets are the primary asset storage tool and communication gateway to the blockchain API. Web3.js is used to connect to the wallet and smart contracts. Pinata cloud handles uploading and management of NFTs on IPFS.

### Back-End

Our backend handles the storing of user data and processes NFT data coming from IPFS.

### Blockchain

We utilize the Polygon frontend to interact with the blockchain, inspect blocks, execute transactions, and query state.

![](<../.gitbook/assets/Tech Stack Chart.png>)
