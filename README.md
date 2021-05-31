test app to create nft on ERC721PresetMinterPauserAutoId openzeppelin contract

- create project on https://infura.io/
- save `projectId` to `secrets.json`
- run `yarn run truffle develop`
- save `mnemonic` to `secrets.json`


create nft:
```
migrate
nft = await ERC721PresetMinterPauserAutoId.deployed()
await nft.mint("<account_address>")
```

check nft on opensea 
```
https://rinkeby-api.opensea.io/asset/<account_address>/<token_id>/validate/
```
