# Vite NFT Marketplace Contracts

## Project Requirements
> 2 independent contracts that can conduct the following auction types:

- [ ] English auction (highest bidder pays their bid). Can have a reserve price for if the highest bid is accepted or not
- [ ] Dutch auction (price descends until someone buys). Can have a reserve price for when the auction is canceled 
- [ ] The contracts should work with ERC-721 tokens

> An example user journey auctioning off an NFT could be:
 - [ ] A user approves an auction contract to transfer the NFT(s) they would like to sell
 - [ ] The user specifies which NFT to auction off and includes the auction parameters (e.g. starting price, reserve price, expiration date, minimum bid increase for English auctions, price decrease rate for Dutch auctions, date after which the seller can no longer cancel their auction, etc.)
 - [ ] The auction contract transfers that NFT to itself and hold it in escrow while the auction is ongoing
 - [ ] Other users bid on the auction. In the case of English auctions, new highest bids are held in escrow while the last highest bid is sent back to its bidder.
 - [ ] Once the auction has ended, the NFT and funds from the winning bid are transferred to their rightful owner

> Additional Requirements
 - [ ] Uses Solidity++ 0.8
 - [ ] Unit tests for all contract functionality using ViteJS and/or Vuilder and your unit testing library of choice.
 - [ ] Contracts should have functions for reading/paginating through all ongoing and ended auctions and reading auction info (e.g. NFT and auction parameters)