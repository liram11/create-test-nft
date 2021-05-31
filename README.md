test app to create nft on ERC721PresetMinterPauserAutoId openzeppelin contract

- create project on https://infura.io/
- save projectId to secret

start truffle
```
yarn run truffle develop
```

create nft:
```
migrate

nft = await ERC721PresetMinterPauserAutoId.deployed()

# 0x2c2Ad69353466eD58bC6694163908A533173cD4A
await nft.mint("<account_address>")

```

deploy to rinkedby 
```
touch .secret
# then add memonic to the .secret

yarn run truffle console --network rinkeby
```
