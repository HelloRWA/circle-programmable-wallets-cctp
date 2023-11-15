# circle-programmable-wallets-cctp

## What it does

We build a blockchain base of X.com, all the new tweet require user to pay gas and ERC20 token to post.
User can login via X.com account and our system use the MPC wallet tech to create a new wallet for the user under the hood. So user do not need to import any private key on our platform but still have a wallet to interact with blockchain.

## What we do with Programmable Wallet and CCTP?

We use them in our *Random Lottery* module. 
User can create a new Lottery pool to attach to a new Tweet that other users can pay ERC20 token to buy the lottery and then get lucky then.
We use programmable wallet api to create a dev controlled programmable wallet to work as the vault of the lottery.
Also while the user lake of $BST and AVAX token, we use the *CCTP* to help user to use their *USDC on Georli* to buy *$BST and AVAX* on Fuji testnet.

* Create a new dev controled programmable wallet and attach to current login user
* While user try to post a new Tweet with *Random Lottery* attached
  * it require the user to fund enough $BST and also enough AVAX gas token in the programmable wallet
  * user can fund with their *USDC on Goerli* into *Fuji chain* via the CCTP tech
* We also use the *circle-mint in app-sanbox* that fund our wallet with 2000 USDC on Goerli
  * Which we will integrate the feature into our product that provide user to pay via credit card to buy USDC.

## Links

* [Demo Video](#)
* [Relative Source code about Programmable Wallet](./programmable-wallet)
  * [Programmable wallet we create](https://testnet.snowtrace.io/address/0xe3a4ee3674b7952d5f4457a94d3a3ab163e7679f)
* [Relative Source code about CCTP](./cctp)
* [Pitch](https://pitch.com/public/724fc677-e462-4ddc-bbb1-bb389d8ed886)

## What's next

* We still heavy build our product of RWA-Wallet.com, plan to launch it before 2023/12/01
* We also plan to use the [*Circle Mint*](https://www.circle.com/en/circle-mint) feature that we can provide our user to pay via their credit card which we need some time to setup a company in HongKong
