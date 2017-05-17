# Blockchain-Cluster
# Characteristics of Blockchain Frameworks

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

# Categorization of Blockchain Frameworks

Characteristics / Frameworks 	| Usage 									| Governance 			| Consensus 													| Hash 							| Signature 		| Structure 		| Tokensupply 		| Transaction 		| Blocktime
------------ 					| ------------								| ------------ 			| ------------ 													| ------------ 					| ------------ 		| ------------ 		| ------------ 		| ------------ 		| ------------ 
Bitcoin Core 					| payment 									| distributed 			| PoW 															| SHA2-256 and RIPEMD160 		| ... 				| UTXO database 	| 21 mio 			| simple conditions | 10 min
Stellar 						| payment 									| Foundation 			| Stellar Consensus Protocol (federated Byzantine agreement) 	| SHA256 						| ed25519 			| ... 				| 100 bil lumens 	| ... 				| ...
Monero 							| payment 									| ... 					| PoW 															| ZK 							| ring (CryptoNote) | ... 				| ... 				| ... 				| 1 min
Zcash 							| payment 									| Foundation 			| PoW (equihash) 												| zk-SNARKs black 				| ... 				| ... 				| 21 mil 			| ... 				| 150 sec
Ethereum 						| computation 								| Foundation / Classic 	| PoW -> PoS (Casper) 											| ? / Keccak-256 				| ... 				| smart contracts 	| ... 				| ... 				| 20 sec
Sia 							| file storage 								| ... 					| PoW 															| blake2b 						| ed25519, entropy 	| ... 				| ... 				| ... 				| 10 min
BigchainDB 						| file storage 								| ... 					| PoS															| SHA3-256 						| ed25519 			| ... 				| ... 				| ... 				| ...
Tendermint 						| cross-blockchain communication 			| ... 					| Byzantine Consensus Algorithm 								| SHA256 						| ed25519 			| ... 				| ... 				| ... 				| ...
Mediachain 						| media 									| open-source (Spotify) | RAFT (federated) 												| ... 							| ... 				| ... 				| ... 				| ... 				| ...
Hyperledger Fabric 				| ... 										| Linux 				| Batch Practical Byzantine Fault Tolerance (bPBFT) 			| SHA256 						| ... 				| ... 				| ... 				| ... 				| ...
Hyperledger Sawtooth Lake 		| supply chain, securitization, settlement 	| Linux 				| Proof-of-Elapsed-Time (PoET) 									| SHA512 						| secp256k1 		| ... 				| ... 				| ... 				| ...
Chain 							| assets 									| incorporated 			| Federated 													| ... 							| ... 				| ... 				| ... 				| ... 				| ...
ꜩ (Tezos) 						| governance 								| ... 					| PoS 															| ... 							| ... 				| ... 				| ... 				| ... 				| ...
Blockstack 						| identity 									| ... 					| ... 															| ... 							| ... 				| ... 				| ... 				| ... 				| ...
Monax 							| ... 										| ... 					| ... 															| ... 							| ... 				| ... 				| ... 				| ... 				| ...


# Categorization of Blockchain Applications
Augur, Gnosis, Steemit, Counterparty

## uncategorized
private blockchain, public blockchain, bft, blockless, decentralized, mining, nodes, Hash, Mempool, Merkle root, Seed,

### properties
persistence, data exchange/data synchronization, immutability, availability, throughput, anonymity/pseudonymity, trustlessness, node operator, intregrated payment processes, currency, (near) real time
