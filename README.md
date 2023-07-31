# polyproof-mod1
deploy an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge

* Generate a 5-item collection using DALLE 2 or Midjourney
* Store items on IPFS using pinata.cloud
* Deploy an ERC721 or ERC1155 to the Goerli Ethereum Testnet
  You should have a promptDescription function on the contract that returns the prompt you used to generate the images
* Map Your NFT Collection using Polygon network token mapper. Note: this isn’t necessary but helpful for visualization.
* Write a hardhat script to batch mint all NFTs. Hint: ERC721A is optimal here.
* Write a hardhat script to batch transfer all NFTs from Ethereum to Polygon Mumbai using the FxPortal Bridge
   Approve the NFTs to be transferred
   Deposit the NFTs to the Bridge
   Test balanceOf on Mumbai


  for terminal:- 
```npm i```

to deploy:-
```npx hardhat run scripts/deploy.js```


to deploy to georli network :-
```npx hardhat run scripts/deploy.js --network goerli ```

to mint :-
```npx hardhat run scripts/batchMint.js --network goerli```

to verify and deposit :-
```npx hardhat run scripts/approvedDeposit.js --network goerli ```

copy the address and check the balace of the wallet and verify the transaction.



