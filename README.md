# satoshi_flip
sui move development exemple tutorial

# testnet published:
owner: 0xc7a438b549236d129bfe2f87132d69f2b72db305c60faf13d1114464354a0b10
house_data_id = 0x6c0f88486ca1b1639e9ec1fea8f50d8aec1c62f4530c1f4ee3c7c668416fd8eb
house_data::HouseCap ObjectID: 0x8f41fc7239f04af527277d8a423ea353bea337646e7c4e05512777175fc11862
PackageID: 0x568a62471e1a1a94c51c7c50cb33ba1c85c0271ff9e9bc313a667552a2309fc1 
Modules: counter_nft, house_data, single_player_satoshi     

# v2 with microlot
hause cap objectID: 0x4892b157e90695a37b84f5b1774f255538122c45e64754069c3da4c977592287
PackageID: 0x653657b1bd1df2b3bbb853da4b36276a014f1a66c46542e75a1e6bb2b781c675 
houde_data_id: 0x2ea02c0cba80bdba1b03af80039b6cc8877cbb29b1385b78b1f9a30c83739861

# run frontend localy:
cd C:\Tools\sui-code\satoshi-coin-flip-frontend-example
notepad.exe src\constants.ts
pnpm dev
http://localhost:5173

# executed as admin:
House Private Key:
6685f4b12ef12767a7a58190562a772728e349b626710b4164c34694aa0407c0
Public Key:
8f93d500af7586975ea0ca755e0e44c669510333d08564bbdc4f65c379d168a9c7c4dcd4deeda7b941d2afcad98dae6d

help cmds:

sui client new-env --alias devnet --rpc https://fullnode.devnet.sui.io:443
sui client envs
sui client switch --env devnet
sui client faucet
sui client gas
sui move new hello_world
cd hello_world
sui move build
cd ..
sui client publish hello_world --gas-budget 10000000
sui keytool list

sui client publish --skip-dependency-verification

# split 0.1 sui
sui client gas
sui client pay-sui --recipients 0xc7a438b549236d129bfe2f87132d69f2b72db305c60faf13d1114464354a0b10 --amounts 100000000 --input-coins 0x4ecc8767542efff51f7aa183ae3b995a2f86f0da045a7332793246a86585a411 --gas-budget 5000000