# ERC 721 Token DAPP for CryptoStar

This project is part of the Udacity Blockchain Nanodegree. In this project, a DAPP was created to create ERC 721 tokens associated with a Star name (CryptoStar). A user can mint a ERC 721 token with a given star name and tokenId. The DAPP smart contract inherits from the Openzeppelin ERC721.sol. The tokens are assigned a token name and a token symbol in the DAPP smart contract. The following functionality was added to the DAPP smart contract:
* Function createStar() - Creates a new Star using the provided star name and tokenID. This function calls the openZeppelin ERC721.sol _mint() function to create the token and assign the ownership to the msg.sender. 
* Function putStarUpForSale() - The owner of a token can use this function to put a star for sale by providing the tokenId and the sale price. 
* Function buyStar() - The function can be used to buy a star from an owner. The tokenId is transfered to the new owner.
* Function lookUptokenIdToStarInfo() - that looks up the stars using the Token ID, and then returns the name of the star.
* Function exchangeStars() - so 2 users can exchange their star tokens
* Function transferStar() - The function transfers a star from the address of the caller to a different address. The function    accepts 2 arguments, the address to transfer the star to, and the token ID of the star.

Truffle webpack was used to develop the code for this project. The functionality of the smart contract was tested using Mocha unit tests. The smart contract was then deployed to the Rinkeby test network using Metamask Wallet and Infura node. The front end of the DAPP was modified to create a new star and the corresponding ERC 721 tokenId. The front end was also modified so that a user can Lookup a star by ID using tokenIdToStarInfo() function.

## General Information
ERC-721 Token Name - Crypto Star

ERC-721 Token Symbol - CST

Version of the Truffle used - v5.0.18

Version of OpenZeppelin used - 2.1.2
