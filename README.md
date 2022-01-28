##POA Development Chain - instructions:
1. create new nodes by giving your own password:
geth --datadir node1 account new
geth --datadir node2 account new
<img width="894" alt="image" src="https://user-images.githubusercontent.com/88476898/151478790-dd66d5f3-8c53-4aa1-990a-6a5adbba07ce.png">
make a note of the two public keys:
node1: 0xE597D6E5d2AC1D7e1dc12B04623648ACEB9F36dB
node 2: 0xD408f4eBb7aF6ce085Ac9c47D826A9B0AC05eBdE

2. run puppeth under the tool directory to generate your genesis block 
<img width="668" alt="image" src="https://user-images.githubusercontent.com/88476898/151479054-1444547c-23d1-45c1-9c9e-54f0701371b7.png">
D408f4eBb7aF6ce085Ac9c47D826A9B0AC05eBdE


3. initilize nodes
geth --datadir node1 init ./viviancoin.json
geth --datadir node2 init ./viviancoin.json
<img width="1430" alt="image" src="https://user-images.githubusercontent.com/88476898/151479419-6129b1c5-75b5-4b30-8fa3-335ea057667a.png">


4. begin mining by opening two terminals. type in password.
../geth --datadir node1 --unlock 0xE597D6E5d2AC1D7e1dc12B04623648ACEB9F36dB --mine --rpc --allow-insecure-unlock

../geth --datadir node2 --unlock 0xD408f4eBb7aF6ce085Ac9c47D826A9B0AC05eBdE --mine --port 30304 --bootnodes "enode://3b5f6c15ebcca24eb1e384e416f09fb9200d1ca3faf56d2c42aab7a5beff5fe87f9872a91b6b4b0e2485ba10b8fe98fb6419dfae2a2fd046fe5e201fb0bfc64d@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock
<img width="1435" alt="image" src="https://user-images.githubusercontent.com/88476898/151480392-57a55b31-6dfb-4373-9d41-a63c838a5746.png">
<img width="1430" alt="image" src="https://user-images.githubusercontent.com/88476898/151480552-33dbdaff-f1f9-4913-8d88-5e3a81cb7645.png">


5.  open mycrypto, change network to customized one
	With network name: viviancoin; chain ID=50599
	
6. Send test transactions



##Case study: CryptoKitties
#what is it
Canadian studio Dapper Labs build up an NFT company, for people to buying and selling virtual cats. It's a game based on blockchain network - Ethereum. This is one of the earliest attempt for recreation and leisure. Each cryptoKitty is a non fungibale token. Each is unique and owned by the user, validated through the blockchain, and its value can appreciate or depreciate based on the market. CryptoKitties cannot be replicated and cannot be transferred without the user's permission even by the game developers. Users can interact with their CryptoKitties, having the ability to buy, sell, and sire (breed) them.

#why this matters?
This is one of the earliest attempts for NFT products on Ethereum. It is the exploration of what kind of things could get value and get traded. This is a good idea to turn a game into a NFT trading. Behind the business operation model, of course we have a lot to review, like if it really worth the value for the virtual cats. 

#why this maybe interesting?
NFT market is pretty hot these days. This is a good real case to turn art works/games into smart contract and trades. Due to the virtual cats 'business' is demanding, it slowed down all other smart contracts confirmation in Ethereum. So it was transfered to another blockchain platform. In the new normal world after covid, it appears the gaming and leisuring demand is indeed very high and there's a market there. 

