# BlockChain-Tutorial-Notes

Blockchain A-Z™: Learn How To Build Your First Blockchain

Course content list is here, https://www.superdatascience.com/pages/blockchain

Podcast: 14 March 2018: The Rise of Blockchain: A Disruptive Super-Technology Much More Than Bitcoin https://www.superdatascience.com/podcast/podcast-rise-of-blockchain

FAQ Bot: MangoBot: June 2019: https://www.superdatascience.com/pages/welcome-to-faqbot

Original White-paper: https://anf.es/pdf/Haber_Stornetta.pdf

Important Concepts of block chain
- Hash Cryptography
- Immutable Ledger
- Distributed P2P Network
- Mining
- Consensus Protocol

--------------------- --------------------- --------------------- --------------------- 

## Hash Cryptography
- Fingerprints are 1 in 60M

## Requirements of Hash Also
- one way
- Deterministic
- Fast Computation
- The Avalanche Effect: small change in input should reflect change in hash value
- Must withstand collisions: collisions will happen but must be rare, it should not be possible to intentionaaly create the input to create a desired hash value

## SHA256 by NSA
- Secure Hash Algo using 256 bits
- Hexadecimal hash
- 64 Chars string is generated
- Create SHA256 hash here , https://tools.superdatascience.com/blockchain/hash

--------------------- --------------------- --------------------- --------------------- 

## Immutable Ledger
- a ledger that can not be modified by un-authorized person
- Read: The Blockchain Economy: A beginner’s guide to institutional cryptoeconomics https://medium.com/cryptoeconomics-australia/the-blockchain-economy-a-beginners-guide-to-institutional-cryptoeconomics-64bf2f2beec4

--------------------- --------------------- --------------------- --------------------- 

## Distributed P2P Network
- If chain is kept only at one place then it can be still modified 
- Keep the chain data in distributed peer to peer n/w , copied at multiple nodes
- Peers constatntly update/verify the data copies with each other, 
- majority wins; data consistency with most-nodes is valued more
- if one node is hacked, its data is considered in-consistent
- For a successful hack ine will need to hack more than half of the nodes simultaneously
- Read: The Meaning of Decentralization : https://medium.com/@VitalikButerin/the-meaning-of-decentralization-a0c92b76a274
- Decentralized vs Distributed?

--------------------- --------------------- --------------------- --------------------- 

## Mining
- A block may store Data of multiple transactions
- Block has: Block number, Data, Prev block hash, current block hash and NONCE
- Apart from Hash used in a block, there is also a "Nonce" in each block, Number used only once!
- Hash is generated of ( Data, Block number, Nonce, Previous hash ), changing any one value will change hash due to avalanche effect of SHA256

## How mining works? The Cryptographic Puzzle
- A hash is a number
- while mining a target (max) hash value is set
- any hash generated gretaer than the target doesn't count
- its a challenge / hurdle created to increase complexity 
- you get to mine a block only if you create a hash smaller than the target
- to create a controlled hash you can keep changing Nonce of the block you want to add
- so miners keep finding Nonce that will create the hash under below the target hence allowing to add the block

--------------------- --------------------- --------------------- --------------------- 

## Consensus Protocol
- it follows Byzantine Generals Problem protocol
- if traitors aquire more than half network (peers) then the newtork can be hacked 
- Read: Understanding Blockchain Fundamentals, Part 1: Byzantine Fault Tolerance:  https://medium.com/loom-network/understanding-blockchain-fundamentals-part-1-byzantine-fault-tolerance-245f46fe8419

## Byzantine Fault Tolerance
- there are 4 generals, they have to aquire a castle
- one of the general is the lead and one of them is (or may be) a traitor, the lead may be the traitor 
- they can attack or retreat
- once the leader sends a message the remaing generals will cross check the message received (attack/retreat) among them
- based on the majority (not equal votes,  majority is required) what the order is received they will act, they are reaching the Consensus here
- 




