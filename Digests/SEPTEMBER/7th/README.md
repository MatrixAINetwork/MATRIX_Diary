### [ANN] [TERA Smart money] [PoW, CPU, 1000 TPS]


#### Introducing TERA | Smart money 


![](https://ip.bitcointalk.org/?u=https%3A%2F%2Fraw.githubusercontent.com%2Fterafoundation%2Fwallet%2Fmaster%2FPic%2FTera.png&t=592&c=-AjXIgqy8s7IVw)

    We sent two important updates to the network, after which the network began to work stably. Now we will deal with smart contracts ...
    Last update 450: https://github.com/terafoundation/wallet 



#### Specification

Name: TERA

Consensus: PoW

Algorithm:  sha3 + meshhash (ASIC resistent hashing)

Max emission: 1 Bln (TERA)

Reward for block: 1-20 coins, depends on network power (one billionth of the remainder of undistributed amount of coins and multiplied by the hundredth part of the square of the logarithm of the network power)

Block size 120 KB

Premine: 5%

Development fund: 1% of the mining amount

Block generation time: 1 second

Block confirmation time: 8 seconds

Speed: from 1000 transactions per second

Commission: free of charge 


#### Additional data:

- Cryptography: sha3, secp256k1
- Protection against DDoS: PoW (hash calculation)
- Platform: Node.JS
- Wallets (src only): Windows, MacOS, Linux
- Network launch: 01.07.2018 12:0:0 (UTC)
- Mining launch: UTC "2018-07-24T15:33:20"
- Type mining: CPU only

#### Links and Resources

- GitHub: https://github.com/terafoundation/wallet  RUS description
- Twitter: https://twitter.com/terafoundation
- Telegram: https://web.telegram.org/#/im?p=@terafoundation
- Discord: Common: https://discord.gg/CvwrbeG RUS: https://discord.gg/dzSGKyR

#### Road map

- Smart-contracts – July (?), 2018
- Internal voting system for adding new functions – August, 2018
- Decentralized messenger – September, 2018
- Decentralized stock exchange – Q4 2018
- Android/iOS Wallets – Q1 2019
- Sharding and increase in transaction speed to 1 million per second – Q2 2019

#### Referral mining program

In the first year of the network work (when the number of the block is in the range from 2 mln to 30 mln), the referral program of mining works. If the miner indicated an adviser in his wallet, then he gets about twice the size of the reward, and his adviser receives a one-time reward. Thus, at the beginning of the action of the referral program, the emission is roughly tripled.

Technically, an adviser is an account number. Any account can become an adviser, provided that it was created more than 1 mln blocks ago (i.e. approximately 12 days).
In order to smooth out the emission curve, the award for referral mining is multiplied by a factor that assumes a value from 1 to 0. The factor takes the value equal to 1 at the beginning of the program and smoothly changes to 0 at the end of the program (up to 30 millionth block).

An example of calculating coins emission:
Let's assume that now the capacity of the network equals to 30 bits in the hash of the block, and it is 1 billion of unallocated coins in total, and we are at the very beginning of the mining program, then one award equals to 900/100 = 9 coins.

Coins will be distributed as follows: 2 awards to the miner, 1 reward to the adviser, and in total there will be deducted 27 coins from the system account (3*9 = 27).

In case if we are in the middle of the referral mining program, when the factor is 0.5, the emission takes the following values ​​in the example above: 1.5 of reward to the miner, 0.5 of reward to the adviser, and in total there will be deducted 18 coins from the system account (2*9 = 18) .

Description of the coins storage rule

The coins are kept in accounts by analogy with bank accounts. The accounts are numbered from 0 sequentially. The zero account number is for system account, to which initially 1 bln coins were issued. To create new account you need to send to the network special transaction ACCOUNT_CREATE where you need to specify a public key of the account owner and unnecessary characteristic “name of account” (a line with length up to 40 bytes). It is advisable to specify the name to check the correctness of the account number input when sending the payment.


#### Transactions

Minimal transaction size of coins transfer from account to account is 114 bytes. 

Minimal size can be obtained if there is one recipient and no description of the payment details. 

Transaction in text format JSON looks as follows:

Code:

    {
       "Type": 110,
      "Version": 0,
      "Currency": 0,
      "FromID": 1,
      "OperationID": 40167,
      "To":
       [
           {
               "ID": 2,
               "SumTER": 100,
               "SumCENT": 0
           }
       ],
      "Description": "test",
      "Sign": "B39C39D91136E92C5B9530ABC683D9A1AF51E27382AFC69EA3B1F14AD7C4CDBE46D36BD743F2B4AE7760F8DDE706D81FB8201ABBF27DABF6F1EC658FE432C141"
    }

Note: transaction in the example above has a length of 118 bytes.

Text representation is packed in binary format + 12 bytes POW are added (for protection against DDoS).
Payment details should be not more than 200 bytes. Actually the size is limited to a maximum of 65535 bytes, but 200 bytes is the size which can be seen by users’ wallets, if the length is more, they cut it.
The longer the transaction length, the more calculation POW must be done to receive competitive transaction and its inclusion in block.

Important change in update 11.07.2018:

Added hash of accounts table in blockchain. This is implemented through a special transaction type 117

Code:

    {
      "Type": 117,
     "BlockNum": 956290,
     "Hash": "75455839E961080C73F1883B7758D27FC0FA63C5F599D37CD63BFC08AED1943A"
    }
 