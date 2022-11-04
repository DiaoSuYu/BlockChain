<h1 align="center">Crowfunding</h1>

## This is a smart contract of crow funding, it can implement basic crowdfunding functions.

*  Code Version: 1.0
1. This code version can support the start and end of multiple crowdfunding projects at the same time, can trace the real-time status of each crowdfunding project at any time, can also call the investors of each crowdfunding project at the same time, and finally transfer escrow funds to the crowdfunding initiator after the crowdfunding project completes the fundraising.  
2. The contract has deployed to the goerli testnet: 
```
https://goerli.etherscan.io/address/0x8c0A0EB5b7928F87d2CA38bf5c4d16019f1bf563#code
```

* Bug List  
`Bug1`: The transfer unit is only support 'WEI', if someone uses other units of calculation for ETH to make a transfer, the amount of ETH will not record in contract, but it has transfered to contract.  
`Bug2`: When transferring funds to a crowdfunding project that has already been completed, no consideration is given to who is entitled to the funding rights of the contract.  