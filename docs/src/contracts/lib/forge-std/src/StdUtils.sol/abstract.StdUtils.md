# StdUtils
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/src/StdUtils.sol)


## State Variables
### multicall

```solidity
IMulticall3 private constant multicall = IMulticall3(0xcA11bde05977b3631167028862bE2a173976CA11);
```


### vm

```solidity
VmSafe private constant vm = VmSafe(address(uint160(uint256(keccak256("hevm cheat code")))));
```


### CONSOLE2_ADDRESS

```solidity
address private constant CONSOLE2_ADDRESS = 0x000000000000000000636F6e736F6c652e6c6f67;
```


### INT256_MIN_ABS

```solidity
uint256 private constant INT256_MIN_ABS = 57896044618658097711785492504343953926634992332820282019728792003956564819968;
```


### UINT256_MAX

```solidity
uint256 private constant UINT256_MAX = 115792089237316195423570985008687907853269984665640564039457584007913129639935;
```


### CREATE2_FACTORY

```solidity
address private constant CREATE2_FACTORY = 0x4e59b44847b379578588920cA78FbF26c0B4956C;
```


## Functions
### _bound


```solidity
function _bound(uint256 x, uint256 min, uint256 max) internal pure virtual returns (uint256 result);
```

### bound


```solidity
function bound(uint256 x, uint256 min, uint256 max) internal view virtual returns (uint256 result);
```

### bound


```solidity
function bound(int256 x, int256 min, int256 max) internal view virtual returns (int256 result);
```

### bytesToUint


```solidity
function bytesToUint(bytes memory b) internal pure virtual returns (uint256);
```

### computeCreateAddress

adapted from Solmate implementation (https://github.com/Rari-Capital/solmate/blob/main/src/utils/LibRLP.sol)

*Compute the address a contract will be deployed at for a given deployer address and nonce*


```solidity
function computeCreateAddress(address deployer, uint256 nonce) internal pure virtual returns (address);
```

### computeCreate2Address


```solidity
function computeCreate2Address(bytes32 salt, bytes32 initcodeHash, address deployer)
    internal
    pure
    virtual
    returns (address);
```

### computeCreate2Address

*returns the address of a contract created with CREATE2 using the default CREATE2 deployer*


```solidity
function computeCreate2Address(bytes32 salt, bytes32 initCodeHash) internal pure returns (address);
```

### hashInitCode

*returns the hash of the init code (creation code + no args) used in CREATE2 with no constructor arguments*


```solidity
function hashInitCode(bytes memory creationCode) internal pure returns (bytes32);
```
**Parameters**

|Name|Type|Description|
|----|----|-----------|
|`creationCode`|`bytes`|the creation code of a contract C, as returned by type(C).creationCode|


### hashInitCode

*returns the hash of the init code (creation code + ABI-encoded args) used in CREATE2*


```solidity
function hashInitCode(bytes memory creationCode, bytes memory args) internal pure returns (bytes32);
```
**Parameters**

|Name|Type|Description|
|----|----|-----------|
|`creationCode`|`bytes`|the creation code of a contract C, as returned by type(C).creationCode|
|`args`|`bytes`|the ABI-encoded arguments to the constructor of C|


### getTokenBalances


```solidity
function getTokenBalances(address token, address[] memory addresses)
    internal
    virtual
    returns (uint256[] memory balances);
```

### addressFromLast20Bytes


```solidity
function addressFromLast20Bytes(bytes32 bytesValue) private pure returns (address);
```

### console2_log


```solidity
function console2_log(string memory p0, uint256 p1) private view;
```

### console2_log


```solidity
function console2_log(string memory p0, string memory p1) private view;
```

