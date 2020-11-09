# Advanced Solidity Contracts 
## Sell to the crowd!

![coin](Images/pexels_coin.jpg)


## Background

A company has decided to crowdsale their PupperCoin token in order to help fund the network development.
This network will be used to track dog breeding activity across the globe in a decentralized way, and allow humans to track the genetic trail of their pets. It has already worked with the necessary legal bodies and obtained the green light on creating a crowdsale open to the public. However, it is required to enable refunds if the crowdsale is successful and the goal is met, and it is only allowed to raise a maximum of 300 ether. The crowdsale will run for 24 weeks.

It is required to create an ERC20 token that will be minted through a `Crowdsale` contract that can be leveraged from the OpenZeppelin Solidity library.

This crowdsale contract will manage the entire process, allowing users to send ETH and get back PUP (PupperCoin).
This contract will mint the tokens automatically and distribute them to buyers in one transaction.

It will need to inherit `Crowdsale`, `CappedCrowdsale`, `TimedCrowdsale`, `RefundableCrowdsale`, and `MintedCrowdsale`.

For demonstration, the crowdsale will be conducted on the Kovan or Ropsten testnet in order to get a real-world pre-production test in.


## Detailed Steps:
### Launch Ganache
Step-1: Launch Ganache and check the tabs- Accounts and Blocks

Step-2: Launch Chrome and open Remix, check the Metamask and select the Localhost 8545 and login to the account.


### Designing the contracts
Step-3: Complete coding in a) PupperCoin.sol and b) Crowdsale.sol

The contract was bootstrapped by inheriting the following OpenZeppelin contracts:

* `Crowdsale`

* `MintedCrowdsale`

* `CappedCrowdsale`

* `TimedCrowdsale`

* `RefundablePostDeliveryCrowdsale`

The parameters were provided for all of the features of the crowdsale, such as the `name`, `symbol`, `wallet` for fundraising, `goal`, etc. 

Step-4: Complile the above 2 programs

Step-5: Deploy PupperCoin amd check deployment status and variables on Remix. Then check  Ganache for confirmation.

Step-6: Deploy PupperCoinCrowdsaleDeployer

Step-7: Deploy PupperCoinCrowdsale

Step-8: Test Contract






