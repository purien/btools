# btools
Tools for Blockchains Transaction Generation for Crypto Currency Bitcoin and Ethereum
Optionally Secured by a Crypto Currency Smartcard (CCSC)

BTOOLS is an open software available for WINDOWS and LINUX, which generates transactions for Bitcoin and Ethereum crypto currency platforms. It is based on the OPENSSL library. In order to provide a strong security, it supports a dedicated Crypto Currency SmartCard (CCSC) uses to generate and store secret keys, and to compute cryptographic (ECDSA) signature.

BTOOLS provides the following services:
- Bitcoin address generation (mainnet and testnet);
- Ethereum address generation;
- Bitcoin transaction generation;
- Ethereum transaction generation;
- Simple Bitcoin node client;
- Bitcoin transaction (via the Bitcoin client);
- Ethereum transaction (via WEB APIs);
- Crypto Currency SmartCard scripts for key generation and transaction signature.

This software, allows a user to electronically sign documents. It first allows the user to generate a private/public key pair (the user signature) and to store the private key on a smartcard’s secure element, for use in the next step, which is the document signature. The Ethertrust company (www.ethertrust.com) can provide the smartcard.

The user needs a smartcard reader connected to his/her computer. To sign a document, the user selects the document to be signed and the location of his private key. The software then creates a hash of the selected document and encrypts the hash with the user private key.

To verify the authenticity of the signed document, a user (verifier) will need to compare the hash of the signed document with a hash of the original document. In order to do this, the verifier needs to decrypt the hash with the user public key, and compare the hashes.

About the Crypto Currency Smartcard

The Crypto Currency smartcard application (CCSC) has three PINs, administrator, user, and user2. The default values are 8 zeros (3030303030303030) for administrator and 4 zeros (30303030) for user and user2.

It is able to generate or to import elliptic curve keys (up to 8), used for the generation of ECDSA signatures used by Bitcoin and Ethereum crypto currencies.

A Read/Write non volatile memory, protected by a dedicated PIN (User2), is available for the storage of any sensitive information.

The main commands are the following:
- Clear Key Pair
- Init Curve
- Generate Key Pair
- Dump KeyPair
- Get Key Parameter
- Set Key Parameter
- SignECDSA
