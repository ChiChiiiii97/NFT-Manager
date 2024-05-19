# NFT Management System

Author: Cherrie Anne Sandrino, Student at NTC
Introduction
This project implements a simple JavaScript-based system for managing Non-Fungible Tokens (NFTs). The code includes functions for minting new NFTs, listing all NFTs, and retrieving the total supply of NFTs. This project serves as a basic introduction to NFT management and can be expanded for more complex applications.
 
## Code Explanation
Total Supply of NFTs
The getTotalSupply function returns the total number of NFTs in the collection.
function getTotalSupply() {
    return nftCollection.length;
}

Usage
Mint NFTs:
Call the mintNFT function with appropriate arguments to create new NFTs.
mintNFT("Art Piece 1", "Artist A", "A beautiful piece of digital art.");
mintNFT("Art Piece 2", "Artist B", "A stunning representation of modern art.");

List NFTs:
Call the listNFTs function to list all the NFTs in the collection.
listNFTs(); // Lists all NFTs

Get Total Supply:
Call the getTotalSupply function to get the total number of minted NFTs.
console.log(`Total NFTs minted: ${getTotalSupply()}`); // Prints total number of NFTs

In conclusion, this JavaScript code provides a basic implementation for managing NFTs. It allows users to mint new NFTs, list all existing NFTs, and retrieve the total supply of NFTs in the collection. This straightforward system serves as a foundation for more complex NFT management solutions.

Thank you for exploring this NFT management system with me.

This project is licensed under the MIT License.

### Minting NFTs

The `mintNFT` function creates a new NFT with the given name, creator, and description, and adds it to the NFT collection.

```javascript
function mintNFT(name, creator, description) {
    const nft = {
        name: name,
        creator: creator,
        description: description,
        timestamp: new Date().toISOString()
    };
    nftCollection.push(nft);
}

Listing NFTs
The listNFTs function displays the details of all NFTs in the collection.
function listNFTs() {
    nftCollection.forEach((nft, index) => {
        console.log(`NFT ${index + 1}:`);
        console.log(`  Name: ${nft.name}`);
        console.log(`  Creator: ${nft.creator}`);
        console.log(`  Description: ${nft.description}`);
        console.log(`  Timestamp: ${nft.timestamp}`);
    });
}

