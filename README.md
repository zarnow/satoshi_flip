# satoshi_flip
sui move development exemple tutorial

# testnet published:
house_data::HouseCap ObjectID: 0x8f41fc7239f04af527277d8a423ea353bea337646e7c4e05512777175fc11862
PackageID: 0x568a62471e1a1a94c51c7c50cb33ba1c85c0271ff9e9bc313a667552a2309fc1 
Modules: counter_nft, house_data, single_player_satoshi      

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