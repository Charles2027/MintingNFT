# MintingNFT

# Steps Perfromed 
## wallet setup :

1. Create a solana keypair `solana-keygen new --outfile wallet/id.json`.
2. set connection to devnet solana cluster `solana config set --url https://api.devnet.solana.com`.
3. Request airdrop : `solana airdrop 2`.
4. set keyPair: `solana config set --keypair wallet/id.json`.

## Steps to Create a SPL Token :

1. run command on solana cli : `spl-token create-token`
2. log :  `Token Address : 4DCzKjnDuTGLZYVpuHPkVinpZCjnYyRSKUzpTU2gbqQk.`
3. run command to create token account : ` spl-token create-account 4DCzKjnDuTGLZYVpuHPkVinpZCjnYyRSKUzpTU2gbqQk`.
4. log:  `Creating account EyHh8m5NraW3kqMxU2qeCkJqsAmJrBTzkwUMEwyamBme `
5. run command to mint token : `spl-token mint 4DCzKjnDuTGLZYVpuHPkVinpZCjnYyRSKUzpTU2gbqQk  10000  EyHh8m5NraW3kqMxU2qeCkJqsAmJrBTzkwUMEwyamBme`.
6. Minting 10,000 Tokens
   - Token ID: 4DCzKjnDuTGLZYVpuHPkVinpZCjnYyRSKUzpTU2gbqQk
   - Recipient Address: EyHh8m5NraW3kqMxU2qeCkJqsAmJrBTzkwUMEwyamBme
   - Transaction Signature: 4iANRVWeYG2vSevKAg54HxVhDLmeuALB1E9LsGPLrDkJf6Jc5f12y8HvDwWpZRb324DRuTE7rrvQpP1eN2emPEr6
     
![image](https://github.com/user-attachments/assets/473118f8-e6ef-4f13-a521-23a721bc2f26)

## Steps to Deploy CandyMachine
1 . sugar upload 
 ```
[1/4] 🗂 Loading assets
Found 11 asset pair(s), uploading files:
+--------------------+
| images | 11 |
| metadata | 11 |
+--------------------+

[2/4] 🖥 Initializing upload
▪▪▪▪▪ Connected
Funding address:
-> pubkey: 1xATrkzv8UfzRttR2iE7EGaY18sim8RWxMxc4aNZ8oT
-> lamports: 557799 (◎ 0.000557799)
Signature: 3tj6R8jFo8GnBGjFv6Uza6zH5YHrAu3cRe4ghAdvCKQYAsRxZAcBA4i812LT8xLQekaCYzRP94m2ok4UjKpDLn1Q

[3/4] 📤 Uploading image files

Sending data: (Ctrl+C to abort)
[00:00:00] Upload successful ███████████████████████████████████████████████████████████████████████████████████████████████████ 11/11

[4/4] 📤 Uploading metadata files

Sending data: (Ctrl+C to abort)
[00:00:00] Upload successful ███████████████████████████████████████████████████████████████████████████████████████████████████ 11/11

11/11 asset pair(s) uploaded.
```
2. sugar deploy :
   
  ```
[1/3] 🍬 Creating candy machine
Candy machine ID: 7ByzXofGSL2mF3mewcK8RScpFTPX7gSQaMvd4SLpS1Cf

[2/3] 📦 Creating and setting the collection NFT for candy machine
Collection mint ID: 7GMUC45h3Qm1jeh5jVf8xqusEBvSdfXeuNMPv6Nq7BHx

[3/3] 📝 Writing config lines
Sending config line(s) in 1 transaction(s): (Ctrl+C to abort)
[00:00:03] Write config lines successful █████████████████████████████████████████████████████████████████████████████████████████ 1/1

✅ Command successful.
```
3.sugar mint
```
[1/2] 🔍 Loading candy machine
Candy machine ID: 7ByzXofGSL2mF3mewcK8RScpFTPX7gSQaMvd4SLpS1Cf
▪▪▪▪▪ Done

[2/2] 🍬 Minting from candy machine

Minting to 1xATrkzv8UfzRttR2iE7EGaY18sim8RWxMxc4aNZ8oT
▸▹▹▹▹ 10 item(s) remaining
▪▪▪▪▪ Mint success

✅ Command successful.
```
## Getting Started :
- git clone : clone the repo
- run npm install to get dependencies
- change .env properties according to your candymachine
- run npm run dev to start application
- test the application by connecting wallet and miniting nft

# Author 
- Charles Finni.
  



