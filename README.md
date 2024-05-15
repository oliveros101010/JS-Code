const NFTs = [];

// Function to mint NFTs
function mintNFT(_name, _colorType, _vehiclesType,_placeType,_accessories) {
    const NFT = {
        "name": _name,
        "colorType": _colorType,
    "vehiclesType":_vehiclesType,
        "placeType": _placeType,
        "accessories":_accessories
    };

    NFTs.push(NFT);
    console.log("Minted: " + _name);
    console.log("---------------------------")
}

// Function to list NFTs
function listNFTs() {
    console.log(">> List of NFTs <<");
    for (let i = 0; i < NFTs.length; i++) {
        const NFT = NFTs[i]; 
        // Fetching each NFT object
        console.log("Name: " + NFT.name);
        console.log("color: " + NFT.colorType);
        console.log("vehicles: " + NFT.vehiclesType);
        console.log("placeType: " + NFT.placeType);
        console.log("accessories: " + NFT.accessories);
        console.log("---------------------------");
    };
}

// Function to get total supply of NFTs
function getTotalSupply() {
    console.log("Total Supply: " + NFTs.length);
}

// Minting at least three NFTs

// call your functions below this line
mintNFT("NFT 1", "Red", "Truck ", "School", "Hats");
mintNFT("NFT 2", "Blue", "Car", "Church", "Watches");
mintNFT("NFT 3", "Pink", "Bus", "Bank", "Belts");

// Listing NFTs and getting total supply
listNFTs();
getTotalSupply();
