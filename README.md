# NFT Marketplace

An NFT elaborates the idea behind blockchain and introduces digital ownership of specific assets. It has become possible thanks to the non-interchangeable (aka non-fungible) nature of a token, which allows the right to possess digital art property to be established. In other words, NFTs represent an abstract means to secure the possession of a specific item by a specific blockchain wallet. An NFT can be sold and traded with the help of smart contracts. Different types of NFT data units can be used to connect digital media such as pictures, videos, and music. Nonfungible tokens can be used to digitally represent any item, such as online-only assets like digital artwork as well as real-world assets like real estate.

My project, the NFT marketplace, creates a much-needed arena for such commercial transactions. It is a virtual shopping centre that offers collectors and artists boundless tokenization and purchase of programmable digital goods, such as:

- Digital art
- Gaming items
- Collectibles

![Home Page](https://github.com/conan1005/NFT-marketplace/blob/master/images/home_page.png)

## Project Features

- `Wallet Connect`: Individuals need crypto wallets to perform any transaction on the marketplace. Different kinds of wallets can be connected to the marketplace giving more choice to the user.
- `Creating NFTs`: Creation of NFTs is the most important feature in the whole Non-Fungible token ecosystem. If an individual needs to create some NFT, they might need to code the smart contract, deploy it on the mainnet of some Blockchain network all by themselves, incurring a huge loss because of the fees. NFT Marketplaces allow everyone to create the tokens on their platform without having the need to code anything. Deployment cost for the task is negligible as well.
- `Auctions - Buying, Selling, Reselling:`: Our NFT Marketplace features a frontend which is where all the items are presented. They are divided into many categories and listed on the platform. The owner of NFTs has the ability to list them on marketplaces, while all other users can buy or sell them. All the transactions are saved onto the blockchain instead of a traditional database.

## Tech Stack

| Framework / Library                                       | Usage                            |
| --------------------------------------------------------- | -------------------------------- |
| [Next.js](https://nextjs.org/docs/getting-started)        | For frontend                     |
| [solidity](https://docs.soliditylang.org/en/v0.8.13/)     | For writting smart contracts     |
| [tailwind css](https://tailwindcss.com/docs/installation) | For designing UI                 |
| [ether.js](https://docs.ethers.io/v5/)                    | Web3 client (contract testing)   |
| [web3.js](https://www.npmjs.com/package/web3)             | Web3 client (Frontend Next.js)   |
| [Chai](https://www.npmjs.com/package/chai)                | Javascript testing framework     |
| [hardhat](https://www.npmjs.com/package/hardhat)          | Ethereum development environment |
| [Polygon](https://polygon.technology/)                    | For better scaling. (Uses POS)   |
| [IPFS](https://www.infura.io/product/ipfs)                | For distributed file system.     |

---

## Running the Application:

- Configure Metamask Settings

  ```
  Network Name: Localhost 8545
  New RPC URL: http://localhost:8545
  Chain ID: 1337
  Currency Symbol: ETH
  ```

  ![settings](https://github.com/conan1005/NFT-marketplace/blob/master/images/metamask_settings.png)

- Run hardhat node
  ```
  npx hardhat node
  ```
- Deploy contract in local hardhat node
  ```
  npx hardhat run scripts/deploy.js --network localhost
  ```
- Login to Metamask and import some hardhat accounts to Metamask by using Private Keys
  ![hardhatnode](https://github.com/conan1005/NFT-marketplace/blob/master/images/hardhat_node.png)

  ![hardhatnode](https://github.com/conan1005/NFT-marketplace/blob/master/images/import.png)

- Run Next.js frontend
  ```
  npm run dev
  ```
