# StdCheats
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/src/StdCheats.sol)

**Inherits:**
[StdCheatsSafe](/contracts/lib/forge-std/src/StdCheats.sol/abstract.StdCheatsSafe.md)


## State Variables
### stdstore

```solidity
StdStorage private stdstore;
```


### vm

```solidity
Vm private constant vm = Vm(address(uint160(uint256(keccak256("hevm cheat code")))));
```


## Functions
### skip


```solidity
function skip(uint256 time) internal virtual;
```

### rewind


```solidity
function rewind(uint256 time) internal virtual;
```

### hoax


```solidity
function hoax(address msgSender) internal virtual;
```

### hoax


```solidity
function hoax(address msgSender, uint256 give) internal virtual;
```

### hoax


```solidity
function hoax(address msgSender, address origin) internal virtual;
```

### hoax


```solidity
function hoax(address msgSender, address origin, uint256 give) internal virtual;
```

### startHoax


```solidity
function startHoax(address msgSender) internal virtual;
```

### startHoax


```solidity
function startHoax(address msgSender, uint256 give) internal virtual;
```

### startHoax


```solidity
function startHoax(address msgSender, address origin) internal virtual;
```

### startHoax


```solidity
function startHoax(address msgSender, address origin, uint256 give) internal virtual;
```

### changePrank


```solidity
function changePrank(address msgSender) internal virtual;
```

### changePrank


```solidity
function changePrank(address msgSender, address txOrigin) internal virtual;
```

### deal


```solidity
function deal(address to, uint256 give) internal virtual;
```

### deal


```solidity
function deal(address token, address to, uint256 give) internal virtual;
```

### dealERC1155


```solidity
function dealERC1155(address token, address to, uint256 id, uint256 give) internal virtual;
```

### deal


```solidity
function deal(address token, address to, uint256 give, bool adjust) internal virtual;
```

### dealERC1155


```solidity
function dealERC1155(address token, address to, uint256 id, uint256 give, bool adjust) internal virtual;
```

### dealERC721


```solidity
function dealERC721(address token, address to, uint256 id) internal virtual;
```

