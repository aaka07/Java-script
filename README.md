NFT Metadata Manager - README
This README provides an overview of the JavaScript program for managing NFTs (Non-Fungible Tokens) using a simple data structure. The program enables minting new NFTs, listing their metadata, and tracking the total number of minted NFTs.

Overview
The NFT Metadata Manager program includes:

A variable to store NFTs.
A function to mint new NFTs by adding their metadata to the collection.
A function to list all NFTs with their details.
A function to display the total number of minted NFTs.
Features
1. Variable to Store NFTs
nfts: An array to hold the metadata of all minted NFTs.
2. Functions
a. mintNFT(name, artist, date, description)
Purpose: Creates a new NFT object and adds it to the nfts array.
Parameters:
name: Name of the NFT.
artist: Name of the artist who created the NFT.
date: The creation date of the NFT.
description: A brief description of the NFT.
Logic:
Constructs an NFT object using the provided parameters.
Appends the NFT object to the nfts array.
b. listNFTs()
Purpose: Iterates through the nfts array and prints the metadata of each NFT to the console.
Logic:
Loops through the nfts array using a for loop.
Logs the name, artist, date, and description of each NFT, along with a separator line for readability.
c. getTotalSupply()
Purpose: Returns the total number of NFTs in the nfts array.
Logic:
Uses the length property of the nfts array to determine the total supply.
Example Usage
Minting NFTs
The mintNFT function is used to create new NFTs. Example:

javascript
Copy code
mintNFT("Sunset Bliss", "Alice", "2023-01-01", "A beautiful sunset over the mountains.");
mintNFT("Ocean Waves", "Bob", "2023-02-14", "Waves crashing onto the shore.");
mintNFT("City Lights", "Charlie", "2023-03-30", "The city skyline at night.");
Listing NFTs
The listNFTs function displays all minted NFTs with their metadata:

javascript
Copy code
listNFTs();
Output:

yaml
Copy code
Name: Sunset Bliss
Artist: Alice
Date: 2023-01-01
Description: A beautiful sunset over the mountains.
---------------------------
Name: Ocean Waves
Artist: Bob
Date: 2023-02-14
Description: Waves crashing onto the shore.
---------------------------
Name: City Lights
Artist: Charlie
Date: 2023-03-30
Description: The city skyline at night.
---------------------------
Total Supply
The getTotalSupply function returns the total number of NFTs:

javascript
Copy code
console.log("Total Supply: " + getTotalSupply());
Output:

mathematica
Copy code
Total Supply: 3
How It Works
Minting NFTs:

Call the mintNFT function with the required metadata (name, artist, date, description).
The function adds a new NFT object to the nfts array.
Listing NFTs:

The listNFTs function iterates over the nfts array and logs each NFT's metadata to the console.
Tracking Total Supply:

The getTotalSupply function calculates the total supply by returning the length of the nfts array.
Enhancements
Add functionality to search for NFTs by name or artist.
Implement editing or deleting NFT metadata.
Integrate with blockchain technologies to mint NFTs on-chain.
Add UI to display NFTs and their metadata visually.
Conclusion
This program provides a basic framework for managing NFTs with JavaScript. It serves as a foundation for more advanced NFT-related projects and can be extended to include additional features.
