Assignment 3: Bitcoin Transaction and Generation
Introduction
In this assignment, you will delve into the practical aspects of Bitcoin. Your task will involve understanding Bitcoin transactions, specifically focusing on transaction scripts. You will apply your Python skills to solve a real-world challenge: accepting and spending Bitcoin funds.

Background
In Bitcoin, funds are locked in a transaction output (TXO) using a script (scriptPubKey) that requires a specific input to unlock (i.e., spend).

As seen in class, some of the common types of scriptPubKey are:

P2PK (Pay-to-Public-Key), which specifies a public key (i.e., a verification key of a digital signature scheme) and requires a matching signature on the transaction.
Pay-to-Public-Key-Hash (P2PKH), which specifies a hash digest and requires a public key that hashes to the digest alongside a matching signature on the transaction. A P2PKH script is of the form: "OP_DUP, OP_HASH160, hash, OP_EQUALVERIFY, OP_CHECKSIG"
The corresponding addresses are called "P2PK address" and "P2PKH address" respectively because the owner of a public key can tell people to send money to their public key simply by telling them what scriptPubKey (of either form) to use in a new TXO.

The scriptPubKey can also express other types of conditions for spending the funds.

You can read more about the Bitcoin scripting language in the course reading material and specifically at Bitcoin Script Wiki.

Overview
The course staff have designated some coins for you and locked them with a P2PKH script on the Bitcoin blockchain (or more precisely, a Bitcoin testnet called Signet, which behaves just like the real Bitcoin blockchain, but does not have monetary value).

Your goal is to accept the funds from one of the transaction output and move them to another account. To do so, you need to create a new transaction whose input is an unspent TXO containing the lock script (scriptPubKey), and the new TXO is another address (or script) where you want to send the Bitcoins.

The secret key to unlock your TXO was sent to you via email. Your challenge is to find the relevant TXO, understand how its locking script works and how to satisfy it using the secret text you were given, and create a new transaction that spends that TXO and sends the funds to another address.

Follow the steps below to complete the assignment.
