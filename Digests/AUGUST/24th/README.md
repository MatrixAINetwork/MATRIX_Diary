### [ANN] QRL - Announcing the Quantum Resistant Ledger

Quantum Resistant Ledger (QRL) has the launch window: mid-Q1 2018!

The QRL will be the first decentralized cryptocurrency which is implemented from the outset to be resistant to both classical and quantum computing attack. It uses a different system of cryptography to bitcoin (and all other altcoins) known as XMSS, which is a hash-based digital signature scheme, and provably quantum-resistant.  The ledger will be the first to use quantum-resistant signatures on a blockchain, which provides an ultra secure store of value in the event of a sudden advance in quantum computing (rendering bitcoin, ethereum etc vulnerable to attack). The initial aim of the project is to establish a functional and secure blockchain on which more technology can be built, such as the Ephemeral post-quantum secure data channels.

The project has grown significantly over the course of 2017, led by myself, a core dev team, ancillary devs and a post-quantum cryptographer. We have added to that a marketing manager and small communications team.

We will ship with the following featureset in Q1 2018.


1. multi-platform qrlcore node release.
2. 100% PQ-secure address space for the QRL (XMSS)
3. cryptonight POW algorithm, 1 minute block-time interval, ability to mine in existing pools, using existing mining software.
4. ephemeral messaging layer capability (PQ-secure end-end data channel functionality utilising Kyber and Dilithium).
5. completely separated wallet and node functionality with all wallet-based requests passing through the node by our universal grpc api.
6. Use of slave XMSS tree signing capability to allow secure mining (and later in the year staking) keeping private keys offline.
7. GUI-based webwallet and full block explorer functionality
8. PQ-token capability out of the box — creating tokens on the QRL chain is now functional.
9. PQ-secure data stamping functionality out of the box.