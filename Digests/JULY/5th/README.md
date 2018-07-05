### [ANN] [CryptoNightV7] ⚡ Electroneum Classic ⚡ 

![](https://i.imgur.com/96ikvTjg.png)


### ⚡ Electroneum Classic ⚡

### ETNC

Electroneum without the BS

Website: https://electroneum-classic.com

#### Features:

 - CryptonightV7
 - 60 second block time
 - 21,000,000,000 total supply
 - Zawy LWMA diff algo
 - No 60% premine
 - No simulation miner


#### Roadmap:

 - Bulletproofs
 - Mobile Wallet
 - Possible cryptonight-etnc variant?


#### Why Electroneum Classic:
Electroneum Classic takes Electroneum v2.0.0.0, which is pre-hardfork back to ASICS, and improves it.  
We added Zawy LWMA difficulty algo to prevent hashrate fluctuations and make 51% attacks much harder. 
We are sticking to CryptonightV7, with a custom variant of cryptonight a future possibility if new threats arise.

Instead of a hardfork we decided to restart the blockchain from genesis. 
This is because Electroneum had a 60% premine of 12.6 Billion coins, with a total supply of 21 Billion. 
This is clear dishonesty and there is about ~7 billion unaccounted coins (mined to an untraceable wallet in block 1) from what was stated in their ICO.
The current circulating supply is not 7,309,891,787 ETN as coinmarketcap states but it is ~14.9 billion


#### Code:

     print_coinbase_tx_sum 0 324157
    Sum of coinbase transactions between block heights [0, 324157) is 14912359342.20 consisting of 14911859354.20 in emissions, and 499988.00 in fees



If we hardfork, these 7 billion coins could easily be dumped by the wallet controller.

#### Why no mobile miner:
The moblle miner is just a simulation that does not have emissions to warrant anywhere near the rumoured 7 billion coins allocated to it.
There are 7 billion coins rumoured to be allocated to the mobile mining simulation, this is 105 million dollars worth of Electroneum at todays price of ~$0.015.
The mobile mining simulation pays out 0.36 ETN per hour at 50 h/s at 120k users, and 0.26 at 50 h/s at 180k users.
If the emissions stay the same, that's (7,000,000,000 / (0.36 * 24 * 120000)) / 365 = 18.5 years.
Basically there is way too much allocated to that pool, as we cannot expect emissions to stay the same as they are,
unless we speculate that Electroneum will not go up in price.
Also this is assuming every mobile miner mines at the maximum allowed speed of 50 h/s.

#### Premine:
- 5% of total coins (1.05 billion) have been premined in block 1.
- 3% is for operations encompassing everything from developer salaries to team equity.
- 1% is for exchange listings.
- 1% is for airdrops, marketing, PR, and social media.

#### Use cases:
We want Electroneum Classic to become the go to for private and fast transactions.  
Paying for a coffee, transferring a large balance or even paying for a VPN should be possible within minutes with full privacy.

#### Road Map:
We are looking to implement bulletproofs as this would reduce the blockchain size and as well as reduce wallet load, exchanges will be happy!

We also want to push out a mobile wallet to allow easy payments.
Of course threat protection and security is our top priority as well.


#### Community:
- Discord: https://discord.gg/h86vs4g
- Reddit: https://www.reddit.com/r/ElectroneumClassic/
- Telegram: https://t.me/electroneumclassic

#### Source:
Github: https://github.com/vans163/electroneum-classic

Currently only Ubuntu binary release are available with the cli wallet.