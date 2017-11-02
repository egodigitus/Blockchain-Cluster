# Blockchain-Cluster

The idea of this categorization is to make different blockchain protocols comparable and to identify protocol attack vectors.
This categorization shall be seen as a first step towards a mature security blockchain research.
Further details can be found in the associated thesis "Clustering Blockchain Protocols with Regards to Security Testing" from Tim Menapace. https://www.academia.edu/34955919/Clustering_Blockchain_Protocols_With_Regards_To_Security_Testing 

Feel free to add new blockchain protocols or to enhance the categorization scheme by itself.
//tim
# Categories of Blockchain Design
A blockchain design is defined as the compound of the three design primitives transaction design, consensus design & block design.
![](images/Blockchain_Design.png?raw=true)

Each Design primitive has several subcategories, described in the following tables:

## Transaction Design
| Category                  | Description of the category. For each blockchain protocol a category can have different values. |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Chaincode                  | Code that is deployed into the blockchain inside a transaction and  processed by every node in the network. Especially non-standard  transaction code that is capable to enforce some kind of business logic. |
| Transaction Cryptography   | How does the protocol ensure confidentiality, integrity,  non-repudiation and authentication of transactions?                                                                                                 |
| --Key Generation           | The cryptographic algorithm that generates the public/private key pair.                                                                                                                                       |
| --Address    Generation    | The algorithm that generates the wallet address from the public key.                                                                                                                                          |
| --Transaction    Signature | The algorithm that uses the public/private key pair to sign a transaction  broadcasted to the network.                                                                                                        |

## Consensus Design
| Category                  | Description of the category. For each blockchain protocol a category can have different values. |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Consensus Algorithm        | The algorithm that lets the nodes in the network eventually come to  one state. Depending on the number of malicious processes  consensus is possible, see section \ref{BFT}.                                 |
| Node Authentication        | How does a node authenticate itself to its peers in the network?                                                                                                                                              |
| Governance                 | How is the codebase of the Reference Implementation developed  and who is leading this development?                                                                                                           |
| Transparency               | Who got what kind of permissions on the network? 
| |public: Everybody can read  
| |private: Selected nodes can read  
| |permissionless: Everybody can write     
| |permissioned: Selected nodes can write                              
                                                                                                      

## Data structure & Block Design
| Category                  | Description of the category. For each blockchain protocol a category can have different values. |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Data structure             | How is the data of the blockchain stored in the nodes?                                                                                                                                                        |
| Blocktime                  | The average time between two blocks.                                                                                                                                                                          |
| Tokens                     | Can users generate their own coin-like tokens?                                                                                                                                                                |
| Coin supply                | Is there a generic coin in the system? How is it supplied?  Incentive to generatenew blocks?                                                                                                                  |

# Characteristics of Blockchain Protocols

Each subcategory can have different values.
The following table is an ongoing collection of different values / characteristics for blockchain design.


| Consensus Algorithm        | Node  Authentification | Governance    | Transparency  | Data structure         | Blocktime  | Coinsupply      | Tokens        | Key  Generation | Address Generation | Transaction Signature     |   | Usage                          |   |
|----------------------------|------------------------|---------------|---------------|------------------------|------------|-----------------|---------------|-----------------|--------------------|---------------------------|---|--------------------------------|---|
| Proof of work              | No                     | decentralized | public        | UTXO                   | fixed time | fixed amount    | Via chaincode | ECC             | RIPEM160 & SHA256  | ECDSA -ed25519 -secp256k1 |   | computation                    |   |
| Proof of stake             | RLPx                   | Foundation    | permissonless | Merkle Patricia Tree   | adjustable | unlimited       | No Tokens     | PKI X.509       | SHA3               | PKI X.509                 |   | file storage                   |   |
| Proof of burn              | X.509                  | incorporated  | private       | NoSQL DB               | No blocks  | no generic coin |               | Kerl            | PKI X.509          | Hash-based OTS            |   | external data                  |   |
| Proof of activity          | Mutual tethering       |               | permissioned  | Directed Acyclic Graph |            |                 |               |                 | Kerl               | ring                      |   | monetization                   |   |
| Proof of capacity          |                        |               |               | Treestate              |            |                 |               |                 |                    |                           |   | payments                       |   |
| Proof of elapsed time      |                        |               |               |                        |            |                 |               |                 |                    |                           |   | cross-blockchain communication |   |
| pBFT                       |                        |               |               |                        |            |                 |               |                 |                    |                           |   | media                          |   |
| Stellar Consensus Protocol |                        |               |               |                        |            |                 |               |                 |                    |                           |   | supply chain                   |   |
| RAFT                       |                        |               |               |                        |            |                 |               |                 |                    |                           |   | securitization                 |   |
| Federated                  |                        |               |               |                        |            |                 |               |                 |                    |                           |   | settlement                     |   |
|                            |                        |               |               |                        |            |                 |               |                 |                    |                           |   | assets                         |   |
|                            |                        |               |               |                        |            |                 |               |                 |                    |                           |   | governance                     |   |

# Categorization of Blockchain Protocols

|                        | Bitcoin                  | Ethereum                | Hyperledger Fabric     | IOTA                          | Monero                    | Zcash                   | Stellar                 | Tendermint             | Chain | Tezos | Sia     | BigchainDB      | Mediachain |
|------------------------|--------------------------|-------------------------|------------------------|-------------------------------|---------------------------|-------------------------|-------------------------|------------------------|-------|-------|---------|-----------------|------------|
| **Consensus Algorithm**    | Proof-of-work SHA-256    | Proof-of-work ethhash   | Ordering  Service      | Tip selection MCMC            | Proof-of-work CryptoNight | Proof-of-work equihash  | Stellar Consensus       | BFT                    |       |       | PoW     | PoS             |            |
| **Node  Authentification** | No BIP 150 & 151         | Yes RLPx                | X.509                  | Mutual tethering              |                           |                         |                         |                        |       |       |         |                 |            |
| **Governance**             | decentralized            | Ethreum Foundation      | IBM & Linux Foundation | IOTA Foundation               | decentralized             | Zcash Foundation        | Foundation              |                        |       |       |         |                 |            |
| **Transparency**           | public &  permissionless | public & permissionless | private & permissioned | public & permissionless       | public & permissionless   | public & permissionless | public & permissionless | private & permissioned |       |       |         |                 |            |
| **Data structure**         | UTXO                     | Merkle Patricia Tree    | NoSQL DB               | Directed  Acyclic Graph       | UTXO LMDB                 | Treestate               |                         |                        |       |       |         |                 |            |
| **Blocktime**              | 10 min                   | ~ 30 sec                | adjustable             | No blocks                     | 2 min                     | 150 sec                 |                         |                        |       |       |         |                 |            |
| **Coinsupply**             | 21 mio BTC               | Unlimited ETH           | No generic coin        | ((3^33-1)/2) IOTA             | Unlimited XMR             | 21 mio                  | 100 bil lumen           |                        |       |       |         | No generic coin |            |
| **Tokens**                 | Via script               | Via smart contract      | Via chaincode          | No                            |                           |                         | Yes                     |                        |       |       |         |                 |            |
| **Chaincode**              | Bitcoin script           | Ethereum bytecode       | Chaincode              | No                            |                           |                         |                         |                        |       |       |         |                 |            |
| **Key Generation**         | secp256k1                | secp256k1               | PKI X.509              | Kerl Ternary Keccak384        | ed25519                   |                         | secp256k1               |                        |       |       |         |                 |            |
| **Address  Generation**    | RIPEMD160 & SHA-256      | SHA3                    | PKI X.509              |                               | Keccak256                 | zk-SNARKs black         | SHA-256                 | SHA-256                |       |       | blake2b | SHA3-256        |            |
| **Transaction Signature**  | ECDSA                    | ECDSA                   | PKI X.509              | Hash-based One-time Signature | ring signature            | BLAKE2b-256             | ed25519                 | ed25519                |       |       | ed25519 | ed25519         |            |


# Categorization of Blockchain Applications
Augur, Gnosis, Steemit, Counterparty <- To Do

## uncategorized
bft, mining, nodes, Hash, Mempool, Merkle root, Seed,

### properties
persistence, data exchange/data synchronization, immutability, availability, throughput, anonymity/pseudonymity, trustlessness, node operator, intregrated payment processes, currency, (near) real time
