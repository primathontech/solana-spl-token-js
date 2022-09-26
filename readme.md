
# SPL Token Utility 
Steps to setup
1. clone the repo
1. ensure nodejs and typescript are installed
1. run `npm install`
1. create `.env` file with `PUB_KEY=<PUBKEY>` and `RPC_URL=https://api.devnet.solana.com` change for mainnet
1. run `ts-node mint.ts`


ts-node mint.ts
```
---STEP 1: Uploading MetaData---
Arweave URL:  https://arweave.net/loXp6e5rwBps8LOxAr2mvq8i5B2KXp7pZHeNaenLzDc
---STEP 2: Creating Mint Transaction---
New Mint Address:  GBKx7sUr6iPBprbATuVJ6kpRizHiUyFbvK9iYPwyrHsZ
---STEP 3: Executing Mint Transaction---
Transaction ID:  4tvg3Xq93Wg8vvpT5TcsfSehUPCRCYvbokhi4BsN41zXEeUAED3mqEJ756RoE9va2BXZrkm4LWvcCFCkA9HQukJB
Succesfully minted 1337 $FUN to CwumMpNFmAzq6Bxyidda3QNs1giATZndPv5WNHXyCZtK.
View Transaction: https://explorer.solana.com/tx/4tvg3Xq93Wg8vvpT5TcsfSehUPCRCYvbokhi4BsN41zXEeUAED3mqEJ756RoE9va2BXZrkm4LWvcCFCkA9HQukJB?cluster=devnet
```


# Metadata Manage

```sh
metaboss update uri -k ~/.config/solana/devnet.json -a CQNKXw1rw2eWwi812Exk4cKUjKuomZ2156STGRyXd2Mp -u https://arweave.net/N36gZYJ6PEH8OE11i0MppIbPG4VXKV4iuQw1zaq3rls

metaboss update data --keypair <PATH_TO_KEYPAIR> --account <MINT_ACCOUNT> --new-data-file <PATH_TO_NEW_DATA_FILE>

https://explorer.solana.com/address/7fwNEMWUqVKRpo2aBycg8JjHhuWeYBUtUSxToSazMAfk/metadata?cluster=devnet

metaboss update data -a 7fwNEMWUqVKRpo2aBycg8JjHhuWeYBUtUSxToSazMAfk -k owner-wallet.json --new-data-file token-meta.json

```
