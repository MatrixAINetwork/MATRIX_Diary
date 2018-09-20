### [ANN][MN/PoW/PoS] ShardBit - the Social Gambling Blockchain

![](https://ip.bitcointalk.org/?u=https%3A%2F%2Fi.imgur.com%2FcpGwdsL.png&t=593&c=6rkIpHVIGQib9w)

#### The Social Gambling Blockchain - Introduction

The creation and subsequent release of Satoshi Nakamoto’s “Bitcoin: A Peer-to-Peer Electronic Cash System” was the world’s first major foray into the world of decentralization, cryptography,  and peer-to-peer networking. Not only did this new technology allow for an individual to safely and efficiently transfer a store of value across long distances without the need for a centralized institution as an intermediary, it finally allowed for one to become self-reliant in regards to managing their funds. In particular, though, the past few years have seen the value and benefits of these networks finally begun to be realized by the public. Ever since the world took notice of Bitcoin’s historic growth in December of 2017, the notion of the blockchain as a technological asset has been on everyone’s mind. As a result, the potential for its widespread adoption and usage is highly likely if not guaranteed. If this possibility comes to fruition, is highly likely that a large number of centralized institutions will be affected--even casinos. It is our goal with ShardBits to spearhead this decentralized revolution and put the power back in the hands of the individual.

The ShardBit project was created to facilitate the further development of the ShardBits cryptocurrency and the ShardBet platform as a whole. Although each individual piece of the ShardBit ecosystem works in sync with the rest, both the currency and the platform are inherently separate modules. The currency in itself is solely meant to be used as a medium of payment for the platform, and supplies the main bankroll for each DApp created, which in turn gives the currency a use case. To illustrate this, and the rest of our ideas for the development of the ShardBit project, we've launched a proof-of-concept DApp called ShardCrash, a BustaBit clone with quite a few improvements, and configured it to work with ShardBits. The core functionality of the game, however, is pretty much the same, and thus a seeding event a la Bustabit's initial seeding event is in order.

We have generated a chain of 10 million sha256 hashes, starting with a server secret that has been repeatedly fed the output of sha256 back into itself 10 million times. The sha256 of the final hash in the chain is mentioned below, by publicizing it here we are preventing any ability to pick an alternate sha256 chain. ShardBet will play through that chain of hashes, in reverse order, and use the hashes to determine the crash point in a probably fair manner. Also, to avoid criticism that the chain was carefully chosen to generate lots of "bad" crash points, each hash in the chain will be salted with a client seed, which we have no control of. The client seed will be the block hash of a ShardBit block that hasn't yet been mined: Block #500.


Final Hash: ccd9d795367ef7415e978e7fede17c31409f9b5d587608ae908559c801b562c1


#### ShardBit - Specifications

- Name: ShardBits (SHDB)
- Algorithm (PoW): C11
- Block Time (PoW/PoS): 90 seconds
- Total Supply: 2,240,300,000 SHDB
- Difficulty Retargeting: Every Block
- Premine: 17.8% (400,000,000 SHDB)
- P2P Port: 37451 | RPC Port: 37452 
- Masternode Collateral: 500,000 SHDB
- Coin Maturity: 24 hours[/size]

#### ShardBit - Features

- ASIC/NiceHash Resistant
- Nvidia & AMD GPU Mining
- Instamine Protection
- Masternode Reward Protection
- Friendly Masternode Setup
- Long-Term Development & Support
- Masternode Dividends from Casino Profit

#### ShardBit - Block Rewards

![](https://ip.bitcointalk.org/?u=https%3A%2F%2Fi.imgur.com%2FTNlsyBS.png&t=593&c=MubNL93w_jt-mw)

#### ShardBit - Masternode ROI

![](https://ip.bitcointalk.org/?u=https%3A%2F%2Fi.imgur.com%2Fd9rEviH.png&t=593&c=Wc-G_I5MgLHAVA)

#### ShardBit - Masternode Dividends

In order to further integrate Masternodes into the ShardBit ecosystem, we've 
developed a tool that automatically pays out a percentage of all profit earned by the 
casino to the current active Masternodes. The rate at which this payment occurs 
has not yet been decided upon, but we expect it to occur frequently enough to create
 an incentive to hosting an active node. 

#### ShardBit - Premine

Developing the coin, we realized that we’d require a substantial premine 
(calculated at 400,000,000 SHDB or 17.8%) to fund the bankroll of our initial 
DApps and in particular support future growth and development as necessary. 
Regarding the bankroll, we plan to set aside the majority of the coins taken for 
this purpose, to not be touched by the team throughout. Any coins not sold in 
the presale will be added to the bankroll. The overall breakdown of the 
premine’s projected use is as follows:

200,000,000 SHDB (50%) - Platform/DApp Bankroll

50,000,000 SHDB (12.5%) - Presale Distribution

80,000,000 SHDB (20%) - Marketing/Development Costs

50,000,000 SHDB (12.5%) - Developer/Founder Payments

20,000,000 SHDB (5%) - Bounty Program

#### ShardBit - Presale

As mentioned above in the premine breakdown, we've decided to set aside 
50,000,000 SHDB for the initial presale distribution. This will be broken down 
into a series of packages and Masternodes for purchase. Any coins set aside 
for the presale that are not bought will be added to the bankroll, for use with 
ShardBet DApps.

Masternode Phases

- Phase One (10 MNs) = 0.3 BTC
- Phase Two (20 MNs) = 0.4 BTC
- Phase Three (Inf MNs) = 0.5 BTC

Staking Packages

- Package #1 (10,000 SHDB) = 0.01 BTC
- Package #2 (50,000 SHDB) = 0.05 BTC
- Package #3 (100,000 SHDB) = 0.1 BTC

#### ShardBit - External Links

- Website: [ShardBit Website](http://info.shardbet.com/)
- Github: [ShardBit Github](https://github.com/shardbit-project)
- Guides/Wiki: [ShardBit Guides/Wiki](https://github.com/shardbit-project/shardbit/wiki)
- Whitepaper: [ShardBit Whitepaper](https://github.com/shardbit-project/shardbit-whitepaper/blob/master/shardbit-whitepaper.pdf)

- Bounty: [Bounty Campaign](https://bitcointalk.org/index.php?topic=5033173)
- ShardCrash: [ShardCrash Website](https://shardbet.com/)

- Daemon: [Daemon](https://github.com/shardbit-project/shardbit/releases/download/v1.0.0.0/shardbit-daemon-v1.0.0.0.zip)
- Linux Wallet: [Linux Wallet](https://github.com/shardbit-project/shardbit/releases/download/v1.0.0.0/shardbit-linux-v1.0.0.0.zip)
- Windows Wallet: [Windows Wallet](https://github.com/shardbit-project/shardbit/releases/download/v1.0.0.0/shardbit-windows-v1.0.0.0.zip)
- Mac Wallet: [Mac Wallet](https://github.com/shardbit-project/shardbit/releases/download/v1.0.0.0/shardbit-mac-v1.0.0.0.zip)

- Discord: [https://discord.gg/VXDsTpX](https://discord.gg/VXDsTpX)
- Twitter: [https://twitter.com/ShardBitEx](https://twitter.com/ShardBitEx)