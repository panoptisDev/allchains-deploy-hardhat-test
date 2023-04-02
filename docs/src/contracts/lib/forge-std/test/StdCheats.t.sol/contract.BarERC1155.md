# BarERC1155
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdCheats.t.sol)


## State Variables
### _balances
`DEALERC1155` STDCHEAT


```solidity
mapping(uint256 => mapping(address => uint256)) private _balances;
```


### _totalSupply

```solidity
mapping(uint256 => uint256) private _totalSupply;
```


## Functions
### constructor


```solidity
constructor() payable;
```

### balanceOf

`DEALERC1155` STDCHEAT


```solidity
function balanceOf(address account, uint256 id) public view virtual returns (uint256);
```

### totalSupply


```solidity
function totalSupply(uint256 id) public view virtual returns (uint256);
```

