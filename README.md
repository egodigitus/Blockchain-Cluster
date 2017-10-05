# Blockchain-Cluster
# Characteristics of Blockchain Protocols

Governance 					| Consensus 					| Hash 			| Signatures 	| Data structure 	| Tokensupply 	| Programmable Transactions | Usage
------------ 				| ------------- 				| ------------- | ------------- | ------------- 	| ------------- | ------------- 			| -------------
Private / Permissionless 	| Proof of work 				| SHA-256 		| ed25519 		| Merkle tree 		| finite (int)	| simple conditions 		| computation
Public / Permissioned 		| Proof of stake 				| SHA-512 		| ring 			| UTXO database 	| infinte 		| smart contracts 			| file storage
Hybrid 						| Proof of burn 				| SHA3-256		| secp256k1 	| ... 				| ICO			| ...						| external data
Foundation 					| Proof of acticity 			| zk-SNARKs		| ... 			| ... 				| pre mining	| ...						| monetization
Linux 						| Proof of capacity 			| blake2b  		| ... 			| ... 				| open mining	| ...						| payments
incorporated 				| Proof of elapsed time (PoET) 	| Keccak-256 	| ... 			| ... 				| ... 			| ... 						| cross-blockchain communication
...							| Byzantine Consensus Algorithm	| RIPEMD160		| ...			| ...				| ...			| ...						| media
distributed					| bPFT							| ...			| ...			| ...				| ...			| ...						| supply chain
...							| Stellar Consensus Protocol	| ...			| ...			| ...				| ...			| ...						| securitization
...							| RAFT							| ...			| ...			| ...				| ...			| ...						| settlement
...							| Federated						| ...			| ...			| ...				| ...			| ...						| assets
...							| ...							| ...			| ...			| ...				| ...			| ...						| governance
...							| ...							| ...			| ...			| ...				| ...			| ...						| identity

# Categorization of Blockchain Protocols

|                        | Bitcoin                  | Ethereum                | Hyperledger Fabric     | IOTA                          | Monero                    | Zcash                   | Stellar                 | Tendermint             | Chain | Tezos | Sia     | BigchainDB      | Mediachain |
|------------------------|--------------------------|-------------------------|------------------------|-------------------------------|---------------------------|-------------------------|-------------------------|------------------------|-------|-------|---------|-----------------|------------|
| Consensus Algorithm    | Proof-of-work SHA-256    | Proof-of-work ethhash   | Ordering  Service      | Tip selection MCMC            | Proof-of-work CryptoNight | Proof-of-work equihash  | Stellar Consensus       | BFT                    |       |       | PoW     | PoS             |            |
| Node  Authentification | No BIP 150 & 151         | Yes RLPx                | X.509                  | Mutual tethering              |                           |                         |                         |                        |       |       |         |                 |            |
| Governance             | decentralized            | Ethreum Foundation      | IBM & Linux Foundation | IOTA Foundation               | decentralized             | Zcash Foundation        | Foundation              |                        |       |       |         |                 |            |
| Transparency           | public &  permissionless | public & permissionless | private & permissioned | public & permissionless       | public & permissionless   | public & permissionless | public & permissionless | private & permissioned |       |       |         |                 |            |
| Data structure         | UTXO                     | Merkle Patricia Tree    | NoSQL DB               | Directed  Acyclic Graph       | UTXO LMDB                 | Treestate               |                         |                        |       |       |         |                 |            |
| Blocktime              | 10 min                   | ~ 30 sec                | adjustable             | No blocks                     | 2 min                     | 150 sec                 |                         |                        |       |       |         |                 |            |
| Coinsupply             | 21 mio BTC               | Unlimited ETH           | No generic coin        | ((3^33-1)/2) IOTA             | Unlimited XMR             | 21 mio                  | 100 bil lumen           |                        |       |       |         | No generic coin |            |
| Tokens                 | Via script               | Via smart contract      | Via chaincode          | No                            |                           |                         | Yes                     |                        |       |       |         |                 |            |
| Chaincode              | Bitcoin script           | Ethereum bytecode       | Chaincode              | No                            |                           |                         |                         |                        |       |       |         |                 |            |
| Key Generation         | secp256k1                | secp256k1               | PKI X.509              | Kerl Ternary Keccak384        | ed25519                   |                         | secp256k1               |                        |       |       |         |                 |            |
| Address  Generation    | RIPEMD160 & SHA-256      | SHA3                    | PKI X.509              |                               | Keccak256                 | zk-SNARKs black         | SHA-256                 | SHA-256                |       |       | blake2b | SHA3-256        |            |
| Transaction Signature  | ECDSA                    | ECDSA                   | PKI X.509              | Hash-based One-time Signature | ring signature            | BLAKE2b-256             | ed25519                 | ed25519                |       |       | ed25519 | ed25519         |            |


# Categorization of Blockchain Applications
Augur, Gnosis, Steemit, Counterparty

## uncategorized
private blockchain, public blockchain, bft, blockless, decentralized, mining, nodes, Hash, Mempool, Merkle root, Seed,

### properties
persistence, data exchange/data synchronization, immutability, availability, throughput, anonymity/pseudonymity, trustlessness, node operator, intregrated payment processes, currency, (near) real time
