---
description: DROP - the gate between web3 and real life
---

# The future of NFTs

DROP is an ERC-1155 NFT system designed as Redeemable**,** Tradable, Scalable and Trustless.\
Each ID of DROPs can redeem different gifts and represent different pre-set value (in usdt) to vendors.\


**REDEEMABLE -** The main feature of DROP is for redemption of online/offline products for exclusive members. This feature can also be used by 3rd parties (e.g. vendors that provide products and accept DROPs for redemption). Once the vendors/3rd parties collect DROP from customers (airdrop holders), they will be able to execute "SETTLEMENT" function from DROP smart contract  to burn DROPs and receive pre-set amount of ERC-20 tokens (USDT) from each burnt DROPs.

**TRADABLE** - Any airdrop holders who (for any reasons) don't want to redeem DROPs can trade them on secondary markets such as OPENSEA.

**SCALABLE** - DROPs will be deployed on POLYGON Chain: an Ethereum 2nd layer chain with up to 65000 transaction per second. Which means, it can support large events (e.g. music festivals) with minimum gas fee impacts. Also, since web3 transactions has no boundaries, event hosts can create campaigns to benefit oversea members.

**TRUSTLESS** - Whenever event hosts want to create (mint) new DROPs, they have to decide:\
1\) How many DROPs they want to mint to issue to their customers.\
2\) How much is it worth per DROP. (in USDT)\
After that the DROP contract will require event hosts to deposit the total amount (plus fees) of ERC-20 token to ensure every DROPs can be paid to vendors' "SETTLEMENT" calls.



## WORKFLOW

![Comlplete workflow of DROP system](../../.gitbook/assets/DROP\_workflow.drawio.png)

## Roles explaination

There are 4 different roles in DROP system:

### 1) Event creators

Those who want to airdrop to their NFT members or list of address to provide exclusive benefits. Any wallet address that holds AMDC NFTs are eligible to be event creators to create their own airdrops.&#x20;

Available functions:\
_Mint_ - input quanity, unit price and USDT to mint new DROPs.\
_Assign Vendors_ - input address, quantity. Setting specific address to be able to accept 'Redeem' function and use 'Settlement' function. Quantity is set for how many DROPs are needed to redeem per gift.\
_Revoke Vendors_ - input address , id (of DROP)\
_Settlement_ - Burn unused / unissued DROPs and withdraw USDT.

### 2) Members

Members receive DROPs can redeem gifts online or offline. (Depend on situation decided by Event creators) If, for any reasons, members don't want to redeem the gifts. They can give, or sell the DROP nfts on OPENSEA.

Available function:\
_Redeem_ - A special function to send DROP to event creators assigned Vendor address. Once triggered, Drops will be transfered to vendor's address and mint the same amount of 'memorial' / 'used' NFT back to the caller.

### 3) Non members

Anyone can own DROPs. If one wants to redeem the airdrop gifts, they can purchase them on secondary markets (e.g. Opensea)

Available function:\
Same as Members

### 4) Vendors

Vendors are a list of address (limited number) assigned by event creators. They are the endpoint for DROP holders to redeem gifts. In real life events, DROP holders send DROPs to vendors with 'redeem' function, once vendors validate the transactions they will issue the gifts to DROP holders.\
After vendors collected DROPs they can initiate '_Settlement_' functions to burn DROPs and collect USDT in return

Available function:\
_Settlement_ - inputs amount of DROPs to burn and receive corresponding amount of USDT

## Use case examples simulation

**Borderless** - Alkiemonkdrinking.club (event host) issue airdrops to 1000 holders(members) to redeem free beer in a list of bars **globally**. Those Bar owners(vendor) will receive $5 USDT on each collected DROPs with 'Settlement' function.

**Collectible -** Alkiemonkdrinking.club (event host) issue airdrops to 1000 holders(members) for Monk's choice Whisky. It's a single cask whisky and its very limited. So members have to spend 3 DROPs to redeem one bottle. Hence, members who want this limited single cask whicky has 2 choices : \
1\) Own 3 AMDC nft so they can have 3 DROPs at once. \
2\) Buy the 2 more DROPs from secondary market (OPENSEA)



