### Prepare

https://github.com/tys-hiroshi/tys-hiroshi.github.io/blob/master/npm.md


```
$ npm install -g truffle
$ npm install @openzeppelin/contracts
```


```
E20Z2Token.deployed().then(i=>e20z2Token=i)

truffle(develop)> e20z2Token.name()
'E20Z2Token'
truffle(develop)> e20z2Token.symbol()
'Z2T'
truffle(develop)> e20z2Token.totalSupply()
BN {
  negative: 0,
  words: [ 100000, <1 empty item> ],
  length: 1,
  red: null
}
truffle(develop)> web3.eth.getAccounts().then(a=>accounts=a)
[
  '0x31C1a3e5e4dcCA94ca2c06aE0032a4Ac287c666e',
  '0xaB5dA81C403b4D5B0dba1fEC84808E173DE6e063',
  '0xB03b6d054010bcC81DdB20e324d1404193C7f78d',
  '0xB8659aD378a5584DB9D6E0691dE30976F0667150',
  '0x2091445D80EFde8eCC229F64FEe80c996eE7289c',
  '0x45fc1c6D73560Da0ccEe44Ad754390cDA08df407',
  '0xcb7b735eF37683740c1FaAFbb9417cD9162b178d',
  '0xF16185190De48D25Fd454Fe79e58CE5C0fa1e433',
  '0x7378426dcA392dBa7e46f11f767AC317D428FfCf',
  '0xa6A36cFC4704BA28834e510d7546D12cF4eeb576'
]
truffle(develop)> accounts[0]
'0x31C1a3e5e4dcCA94ca2c06aE0032a4Ac287c666e'
truffle(develop)> e20z2Token.balanceOf(accounts[0]).then(b=>balance=b)
BN {
  negative: 0,
  words: [ 100000, <1 empty item> ],
  length: 1,
  red: null
}
truffle(develop)> web3.utils.fromWei(balance, "ether")
'0.0000000000001'
```

```
Compile:        truffle compile
Migrate:        truffle migrate
Test contracts: truffle test
```


## install vue.js

```
npm install -g @vue/cli
npm install web3
```