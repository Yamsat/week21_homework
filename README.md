# Week 21 Homework
## Crowdsale
I created smart contracts to crowdsale a ERC20 token, PupperCoin to help fund the network development. The goal is to raise 300 ETH in 24 weeks.

To perfom this crowdsale, three contracts were created.
- PupperCoin
- PupperCoinSale
- PupperCoinSaleDeployer

### PupperCoin
This contract creates ECR20Mintable token, PupperCoin.  I imported ERC20Mintable and ERC20Detailed contracts from OpenZeppelin library.

![PupperCoin](/screenshots/code_3.png)

### PupperCoinSale
This contract performs a crowdsale.  We use the following contracts from OpenZeppelin library.
- Crowdsale
- MintedCrowdsale
- CappedCrowdsale
- TimeCrowdsale
- RefundablePostDeliveryCrowdsale

![PupperCoinSale](/screenshots/code_1.png)

### PupperCoinDeployer

This contact is to deploy PupperCoin and PupperCoinSale contracts.

![PupperCoinDeployer](/screenshots/code_2.png)

## Test 
For testing purpose I modified the parameters as follows;
Goal: 300 ETH to 3000000 Wei
Duration: 24 weeks to 60 minutes

![parameters modified](/screenshots/parameters_modified.png)

### Deployment

Deploy PupperCoinSaleDeployer.

![PupperCoinSaleDeployer deploy](screenshots/PupperCoinSaleDeployer_deploy.png)

PupperCoinSaleDeployer was successfuly deployed.

![PupperCoinSaleDeployer success](screenshots/contract_deploy_success.png)

Deploy PupperCoin.

![PupperCoin deploy](screenshots/PupperCoin_deploy.png)

PupperCoin is deployed.

![PupperCoin deployed](screenshots/PupperCoin_deployed.png)

Deploy PupperCoinSale.

![PupperCoinSale deploy](screenshots/PupperCoinSale_deploy.png)

PupperCoinSale is deployed.

![PupperCoinSale deployed](screenshots/PupperCoinSale_deployed.png)

Check parameters.

![parameters](screenshots/parameters.png)

### Transactions

The first investor invests 1000000 Wei.

![first buy](screenshots/buy_token_1.png)

The transction was successful.

![first buy success](screenshots/buy_token_1_success.png)

Check how much Wei has been raised.

![raised 1](screenshots/raised_1.png)

The second investor invests 1000000 Wei.

![Second buy](screenshots/buy_token_2.png)

The transction was successful.

![Second buy success](screenshots/buy_token_2_success.png)

Check how much Wei has been raised.

![raised 2](screenshots/raised_2.png)

The third investor invests 1000000 Wei.

![third buy](screenshots/buy_token_3.png)

The transction was successful.

![third buy success](screenshots/buy_token_3_success.png)

Check how much Wei has been raised. Yes, we have acheived the goal!

![raised 1](screenshots/raised_3.png)

The cap has also been reached. But someone tries to buy PupeerCoin.

![raise 4](screenshots/buy_token_4.png)

Error message pops up.

![error](screenshots/error.png)

60 minutes has been passed... Let's finalize.

![finalize](screenshots/finalize.png)

Successfully finalized!

![finalized successfully](screenshots/finalize_success.png)

Let's see if the parmeters have changed.

![after finalized](screenshots/after_finalized.png)

Lets's check token balance for each investor.

![token balance 1](screenshots/token_balance_1.png)

![token balance 2](screenshots/token_balance_2.png)

![token balance 3](screenshots/token_balance_3.png)

### Adding PupperCoin to Metamask

Let's export PUP token to Metamask.
Click "Assets" tab and navigate to "Import tokens."

![token import 1](screenshots/import_1.png)

Populate "Token Contact Address" with PupperCoin contract address.  Symbol and decimal automatically show up. Then click "Add Custom Token."

![token import 2](screenshots/import_2.png)

You see PupperCoin and its balance. Click "Import Tokens."

![token imported](screenshots/token_imported.png)



