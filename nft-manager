let nftCollection = [];

function mintNFT(name, creator, description) {
    const nft = {
        name: name,
        creator: creator,
        description: description,
        timestamp: new Date().toISOString()
    };
    nftCollection.push(nft);
}

function listNFTs() {
    nftCollection.forEach((nft, index) => {
        console.log(NFT ${index + 1}:);
        console.log(  Name: ${nft.name});
        console.log(  Creator: ${nft.creator});
        console.log(  Description: ${nft.description});
        console.log(  Timestamp: ${nft.timestamp});
    });
}

function getTotalSupply() {
    return nftCollection.length;
}


mintNFT("Art Piece 1", "Artist A", "A beautiful piece of digital art.");
mintNFT("Art Piece 2", "Artist B", "A stunning representation of modern art.");

listNFTs(); // List all NFTs
console.log(Total NFTs minted: ${getTotalSupply()}); // Print total number of NFTs
