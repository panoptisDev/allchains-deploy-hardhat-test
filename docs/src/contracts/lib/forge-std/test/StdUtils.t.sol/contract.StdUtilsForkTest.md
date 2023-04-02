# StdUtilsForkTest
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdUtils.t.sol)

**Inherits:**
[Test](/contracts/lib/forge-std/src/Test.sol/abstract.Test.md)


## State Variables
### SHIB

```solidity
address internal SHIB = 0x95aD61b0a150d79219dCF64E1E6Cc01f0B64C4cE;
```


### SHIB_HOLDER_0

```solidity
address internal SHIB_HOLDER_0 = 0x855F5981e831D83e6A4b4EBFCAdAa68D92333170;
```


### SHIB_HOLDER_1

```solidity
address internal SHIB_HOLDER_1 = 0x8F509A90c2e47779cA408Fe00d7A72e359229AdA;
```


### SHIB_HOLDER_2

```solidity
address internal SHIB_HOLDER_2 = 0x0e3bbc0D04fF62211F71f3e4C45d82ad76224385;
```


### USDC

```solidity
address internal USDC = 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48;
```


### USDC_HOLDER_0

```solidity
address internal USDC_HOLDER_0 = 0xDa9CE944a37d218c3302F6B82a094844C6ECEb17;
```


### USDC_HOLDER_1

```solidity
address internal USDC_HOLDER_1 = 0x3e67F4721E6d1c41a015f645eFa37BEd854fcf52;
```


## Functions
### setUp


```solidity
function setUp() public;
```

### testCannotGetTokenBalances_NonTokenContract


```solidity
function testCannotGetTokenBalances_NonTokenContract() external;
```

### testCannotGetTokenBalances_EOA


```solidity
function testCannotGetTokenBalances_EOA() external;
```

### testGetTokenBalances_Empty


```solidity
function testGetTokenBalances_Empty() external;
```

### testGetTokenBalances_USDC


```solidity
function testGetTokenBalances_USDC() external;
```

### testGetTokenBalances_SHIB


```solidity
function testGetTokenBalances_SHIB() external;
```

