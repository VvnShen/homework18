##POA Development Chain - instructions:
1. create new nodes by giving your own password:
geth --datadir node1 account new
geth --datadir node2 account new
<img width="892" alt="image" src="https://user-images.githubusercontent.com/88476898/151476196-d45de5e2-79de-401c-84ef-1917079075f6.png">

2. run puppeth under the tool directory to generate your genesis block 

<img width="734" alt="image" src="https://user-images.githubusercontent.com/88476898/151476981-4446d318-7318-4188-a3cc-64a30cc05b6e.png">
As I have already configured a genesis block, so I can export the configration directly. If you need to configure a new one, you can follow the questions, to choose PoA consensus algorism.

3. initilize nodes
geth --datadir node1 init ./vvncoin.json
geth --datadir node2 init ./vvncoin.json
<img width="1425" alt="image" src="https://user-images.githubusercontent.com/88476898/151477355-a97928a4-672b-4099-970f-8e8f4111da24.png">




	1. Initialize two nodes after you have downloaded attached folders to your local desktop:
../geth --datadir node1 --unlock 0x24a4fC1fC703c91E36C40e3c48EC79d6DcE75c10 --mine --rpc --allow-insecure-unlock

../geth --datadir node2 --unlock 0x33E47e6ff72A7954D2e8b272c2A29d86af4C7881 --mine --port 30304 --bootnodes "enode://200cdd09708b8cddabc6b6802650df2afbaefed1cc8589c1db044323a290a34339c452904d29f1c0fcbfaef5e6bca56c16d9b2340af4f33a8809c45bd1ea5937@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock

2. open mycrypto, change network to customized one
	With network name: viviancoin; chain ID=9875
	
3. Send test transactions![image](https://user-images.githubusercontent.com/88476898/149864800-f52d469e-75d5-4605-a110-7a9e1bdb61c3.png)






##Case study: CryptoKitties
#what is it
Canadian studio Dapper Labs build up an NFT company, for people to buying and selling virtual cats. It's a game based on blockchain network - Ethereum. This is one of the earliest attempt for recreation and leisure. Each cryptoKitty is a non fungibale token. Each is unique and owned by the user, validated through the blockchain, and its value can appreciate or depreciate based on the market. CryptoKitties cannot be replicated and cannot be transferred without the user's permission even by the game developers. Users can interact with their CryptoKitties, having the ability to buy, sell, and sire (breed) them.

#why this matters?
This is one of the earliest attempts for NFT products on Ethereum. It is the exploration of what kind of things could get value and get traded. This is a good idea to turn a game into a NFT trading. Behind the business operation model, of course we have a lot to review, like if it really worth the value for the virtual cats. 

#why this maybe interesting?
NFT market is pretty hot these days. This is a good real case to turn art works/games into smart contract and trades. Due to the virtual cats 'business' is demanding, it slowed down all other smart contracts confirmation in Ethereum. So it was transfered to another blockchain platform. In the new normal world after covid, it appears the gaming and leisuring demand is indeed very high and there's a market there. 

