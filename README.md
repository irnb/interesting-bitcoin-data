# interesting-bitcoin-data

Interesting data artifacts from the Bitcoin blockchain, useful to QA/security testers, developers, and researchers.

## Transactions

### BIP 30

Prior to the BIP 30 fix, transactions could have duplicate hashes/IDs. There are 2 pairs:

* https://blockchain.info/tx/d5d27987d2a3dfc724e359870c6644b40e497bdc0589a033220fe15429d88599 (appears in blocks at height 91812 and 91842)
* https://blockchain.info/tx/e3bf3d07d4b0375638d5f1db5255fe07ba2c4cb067cd81b84ee974b6585fb468 (appears in blocks at height 91722 and 91880)

### The Megatransaction

* https://blockchain.info/tx/bb41a757f405890fb0f5856228e23b715702d714d59bf2b1feb70d8b2b4e3e08 (contains 5569 inputs)

### Sample Coinbase tx

* https://blockchain.info/tx/a8d0c0184dde994a09ec054286f1ce581bebf46446a512166eae7628734ea0a5

### Sample BIP47 tx

* https://blockchain.info/tx/9414f1681fb1255bd168a806254321a837008dd4480c02226063183deb100204

### Sample Darkwallet-style stealth address tx

* https://blockchain.info/tx/3b87cb74a83f581d8edf1e64c7b9a8053df8505973d200119f3dd5bbbffbcadb

### First P2SH transaction on blockchain [[source]](https://medium.com/@chjj/ethereum-is-the-op-eval-of-cryptocurrency-d6beaa17eb50)

* https://blockchain.info/tx/9c08a4d78931342b37fd5f72900fb9983087e6f46c4a097d8a1f52c74e28eaf6

### The first OP_CODESEPARATOR transaction aka ["coolest tx ever" according to Christopher Jeffrey](https://medium.com/@chjj/ethereum-is-the-op-eval-of-cryptocurrency-d6beaa17eb50)

* https://blockchain.info/tx/4d932e00d5e20e31211136651f1665309a11908e438bb4c30799154d26812491

### XSS in output script

* https://blockchain.info/tx/a165c82cf21a6bae54dde98b7e00ab43b695debb59dfe7d279ac0c59d6043e24

### Unusual SIGHASH_SINGLE transaction that forked bitcoin-ruby

* https://blockchain.info/tx/315ac7d4c26d69668129cc352851d9389b4a6868f1509c6c8b66bead11e2619f
* https://oxt.me/transaction/315ac7d4c26d69668129cc352851d9389b4a6868f1509c6c8b66bead11e2619f (oxt.me link)
* Reference: https://bitcointalk.org/index.php?topic=260595.0

### First transaction to spend TXO in same block it was created

* https://blockchain.info/tx/6b0f8a73a56c04b519f1883e8aafda643ba61a30bd1439969df21bea5f4e27e2

### Transaction with invalid output scripts

* https://blockchain.info/tx/ebc9fa1196a59e192352d76c0f6e73167046b9d37b8302b6bb6968dfd279b767

## Addresses

* https://blockchain.info/address/1GktTvnY8KGfAS72DhzGYJRyaQNvYrK9Fg (BIP 30)
* https://blockchain.info/address/16va6NxJrMGe5d2LP6wUzuVnzBBoKQZKom (BIP 30)
* https://blockchain.info/address/19VAb9zAhpWLaWfEuqw9HXup2zaNoNPPyE (megatransaction)
* https://blockchain.info/address/12c6DSiU4Rq3P4ZxziKxzrL5LmMBrzjrJX (One of Satoshi's addresses)
* https://blockchain.info/address/13A1W4jLPP75pzvn2qJ5KyyqG3qPSpb9jM (Only used to receive Coinbase rewards)
* https://blockchain.info/address/1JQhWJciZAhDHbjDgjs8Yj6Y7UG1ihfZdK (Large txs, lots of outputs)
* https://blockchain.info/address/1F7w3bZsDeEh3X64kkWoYkhdXkJDZKKdtv (Lots of large txs with lots of inputs)
* https://blockchain.info/address/1ChainLhQ8P1NEv6pFpVU8Z8RkoBKz6gF9 (Coinbase txs)
* https://blockchain.info/address/342ftSRCvFHfCeFFBuz4xwbeqnDw6BGUey (First P2SH address)
* https://blockchain.info/address/1JsJs5d6E5SmJSGUiQ12uF1GDZxTCUWvf (Used in XSS transaction)
* https://blockchain.info/address/1Q3cumLg391Nq6ye5AiE2reWcpZghTm5mZ (Used in SIGHASH_SINGLE forking transaction)

## Blocks

* Block Height 0 (Genesis Block): https://blockchain.info/block/000000000019d6689c085ae165831e934ff763ae46a2a6c172b3f1b60a8ce26f
* Block Height 546 (First block to create TXOs and spend them within same block): https://blockchain.info/block/000000005a4ded781e667e06ceefafb71410b511fe0d5adc3e5a27ecbec34ae6
* Block Height 210000 (First block after first reward halving): https://blockchain.info/block/000000000000048b95347e83192f69cf0366076336c639f9b7228e9ba171342e
* Block Height 124724 (First block that does not create the full block reward): https://blockchain.info/block/0000000000004c78956f8643262f3622acf22486b120421f893c0553702ba7b5
* Block Height 164243 (First block that does not create the full block reward due to missing fees): https://blockchain.info/block/0000000000000c04c9d86de177f9320b3c8eca807b25b6b592b5a2b702eb3544

## Contributions

### Conventions

When possible, please link to blockchain explorers for data artifacts you have added, such as transaction IDs and addresses. For Bitcoin addresses, you should include at least one explorer link that contains a QR code for addresses.

Contributions may be submitted as pull requests to the Master branch or GitHub issues.

## Contributors

* [@kristovatlas](https://github.com/kristovatlas/)
* [@alecalve](https://github.com/alecalve/)
* [@SergioDemianLerner](https://github.com/SergioDemianLerner/)
* [@harrigan](https://github.com/harrigan/)
* [@devinrsmith](https://github.com/devinrsmith/)
