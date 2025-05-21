# bitcoinbrainwallet
>Bitcoin Brainwallet Generator, Construct Transaction and Offline Sign Transaction, Demonstration of Bitcoin Brain Password, Private Key, Public Key, and Address Generation Steps and Relationships

# Brainwallet Generator

Make your algorithms to derive private keys. For example,

Passphrase: Who is Satoshi?

H1 = SHA512(Who)

H2 = SHA512(is)

H3 = SHA512(Satoshi)

H4 = SHA512(?)

Seed = SHA512(H1+H2+H3+H4)

Serial number: 1,2,3…

Private key 1: SHA256(Seed + SHA512(1))

Private key 2: SHA256(Seed + SHA512(2))

You also can make replacement or cropping modifications to the hash values. This brain wallet generator can convert the seed to mnemonics according to BIP39. You can make your derivation algorithms to generate private keys. Download this brainwallet program onto an offline device, and then generate private keys.
You should record the key information of your algorithms in a certain place and practice the process of generating private keys at regular intervals to ensure that you can firmly remember your brain wallet. At the same time, compile the seed mnemonics into a story to facilitate memorizing the mnemonics and achieve a double insurance for memorizing the brain wallet.

Warning: Don't use the private key = SHA256(Who is Satoshi?) to generate your address!!! That's very dangerous. Some people have created large databases of phrase-address correspondences and constantly monitor the balances on these addresses. Once you transfer Bitcoin to these addresses, it will be instantly stolen.

# Airgap Send Bitcoin

First, download this brain wallet program onto an offline mobile phone. And then,

Step 1: Online transaction construction. This brain wallet program can construct Bitcoin transactions online, and generate hexadecimal strings of unsigned transactions and corresponding QR codes.

Step 2: Offline transaction signing. Scan the QR code generated in the first step with an offline phone, and use this brain wallet program downloaded on the phone to generate the corresponding private key to sign the unsigned transaction, and generate a signed transaction string and its corresponding QR code.
Step 3: Online transaction broadcasting. Scan the QR code generated in the second step with an online phone and broadcast the transaction.
