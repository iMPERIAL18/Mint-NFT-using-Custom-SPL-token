# Mint NFT using Custom SPL token

## Description
This project demonstrates the process of minting NFTs (Non-Fungible Tokens) using Solana. It covers the steps from creating wallets, configuring Solana, airdropping tokens, setting up the candy machine, and minting NFTs.

## Getting Started
To get started with the project, follow the instructions below:

### Prerequisites
- Make sure you have Node.js and npm installed on your machine.
- You need to have a Solana wallet set up. You can use the Solana CLI to create wallets.

### Executing Program
Follow the steps below to execute the program:

1. Go to mint-fungible-spl folder.
2. Create a Solana wallet using the command: `solana-keygen new --outfile wallet.json`
3. Set the Solana configuration to use the Devnet using the command: 
&nbsp;&nbsp;&nbsp;&nbsp;`solana config set --url https://rpc.ankr.com/solana_devnet`
&nbsp;&nbsp;&nbsp;&nbsp;`solana config set --keypair .\mint-fungible-spl\wallet.json`
4. Airdrop some funds to your wallet using the command: `solana airdrop 1`
5. Change the `MINT_CONFIG` and `MY_TOKEN_METADATA` data in the project.
6. Execute the minting script using: `ts-node mint.ts`
7. Copy the secret key and import the account to the Phantom wallet.
8. Take note of the token address.
9. Go to Folder mintNFT
10. Create two more Solana wallets for the owner and creator using the commands:
&nbsp;&nbsp;&nbsp;&nbsp;`solana-keygen new --outfile owner.json`
&nbsp;&nbsp;&nbsp;&nbsp;`solana-keygen new --outfile creator.json`
11. Set the Solana configuration to use these new wallets and airdrop some funds to both wallets.
12. Send some SPL (Solana SPL Token) to the owner's wallet.
13. After that, copy the token account address from the owner's wallet.

14. Run the command: `sugar launch` and follow the prompts to set up the candy machine. 
 - You will need to provide the number of NFTs you will have, the symbol, seller fee basis points, creator wallet address, and royalty percentage share.

15. Open the `config.json` file and add the required information.

16. Note down the candy machine id.

17. Clone the UMI-CMV3-UI Inofficial repository using: `git clone https://github.com/MarkSackerberg/umi-cmv3-ui-inofficial.git`

18. Follow the guide from the cloned repository to complete the minting process.

## Authors
- Hemin Patel
- GitHub: [https://github.com/iMPERIAL18](https://github.com/iMPERIAL18)
