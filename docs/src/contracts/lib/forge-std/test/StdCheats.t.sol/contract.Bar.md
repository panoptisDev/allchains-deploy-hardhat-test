# Bar
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdCheats.t.sol)


## State Variables
### balanceOf
`DEAL` STDCHEAT


```solidity
mapping(address => uint256) public balanceOf;
```


### totalSupply

```solidity
uint256 public totalSupply;
```


## Functions
### constructor


```solidity
constructor() payable;
```

### bar

`DEAL` STDCHEAT
`HOAX` and `CHANGEPRANK` STDCHEATS


```solidity
function bar(address expectedSender) public payable;
```

### origin


```solidity
function origin(address expectedSender) public payable;
```

### origin


```solidity
function origin(address expectedSender, address expectedOrigin) public payable;
```

