### [ANN][MN/PoW/PoS] ShardBit - the Social Gambling Blockchain

![](https://ip.bitcointalk.org/?u=https%3A%2F%2Fi.imgur.com%2FcpGwdsL.png&t=593&c=6rkIpHVIGQib9w)

#### The Social Gambling Blockchain - Introduction

The creation and subsequent release of Satoshi Nakamoto’s “Bitcoin: A Peer-to-Peer Electronic Cash System” was the world’s first major foray into the world of decentralization, cryptography,  and peer-to-peer networking. Not only did this new technology allow for an individual to safely and efficiently transfer a store of value across long distances without the need for a centralized institution as an intermediary, it finally allowed for one to become self-reliant in regards to managing their funds. In particular, though, the past few years have seen the value and benefits of these networks finally begun to be realized by the public. Ever since the world took notice of Bitcoin’s historic growth in December of 2017, the notion of the blockchain as a technological asset has been on everyone’s mind. As a result, the potential for its widespread adoption and usage is highly likely if not guaranteed. If this possibility comes to fruition, is highly likely that a large number of centralized institutions will be affected--even casinos. It is our goal with ShardBits to spearhead this decentralized revolution and put the power back in the hands of the individual.

The ShardBit project was created to facilitate the further development of the ShardBits cryptocurrency and the ShardBet platform as a whole. Although each individual piece of the ShardBit ecosystem works in sync with the rest, both the currency and the platform are inherently separate modules. The currency in itself is solely meant to be used as a medium of payment for the platform, and supplies the main bankroll for each DApp created, which in turn gives the currency a use case. To illustrate this, and the rest of our ideas for the development of the ShardBit project, we've launched a proof-of-concept DApp called ShardCrash, a BustaBit clone with quite a few improvements, and configured it to work with ShardBits. The core functionality of the game, however, is pretty much the same, and thus a seeding event a la Bustabit's initial seeding event is in order.

We have generated a chain of 10 million sha256 hashes, starting with a server secret that has been repeatedly fed the output of sha256 back into itself 10 million times. The sha256 of the final hash in the chain is mentioned below, by publicizing it here we are preventing any ability to pick an alternate sha256 chain. ShardBet will play through that chain of hashes, in reverse order, and use the hashes to determine the crash point in a probably fair manner. Also, to avoid criticism that the chain was carefully chosen to generate lots of "bad" crash points, each hash in the chain will be salted with a client seed, which we have no control of. The client seed will be the block hash of a ShardBit block that hasn't yet been mined: Block #500.


Final Hash: ccd9d795367ef7415e978e7fede17c31409f9b5d587608ae908559c801b562c1


