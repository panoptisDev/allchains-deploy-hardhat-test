# stdJson
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/src/StdJson.sol)


## State Variables
### vm

```solidity
VmSafe private constant vm = VmSafe(address(uint160(uint256(keccak256("hevm cheat code")))));
```


## Functions
### parseRaw


```solidity
function parseRaw(string memory json, string memory key) internal pure returns (bytes memory);
```

### readUint


```solidity
function readUint(string memory json, string memory key) internal returns (uint256);
```

### readUintArray


```solidity
function readUintArray(string memory json, string memory key) internal returns (uint256[] memory);
```

### readInt


```solidity
function readInt(string memory json, string memory key) internal returns (int256);
```

### readIntArray


```solidity
function readIntArray(string memory json, string memory key) internal returns (int256[] memory);
```

### readBytes32


```solidity
function readBytes32(string memory json, string memory key) internal returns (bytes32);
```

### readBytes32Array


```solidity
function readBytes32Array(string memory json, string memory key) internal returns (bytes32[] memory);
```

### readString


```solidity
function readString(string memory json, string memory key) internal returns (string memory);
```

### readStringArray


```solidity
function readStringArray(string memory json, string memory key) internal returns (string[] memory);
```

### readAddress


```solidity
function readAddress(string memory json, string memory key) internal returns (address);
```

### readAddressArray


```solidity
function readAddressArray(string memory json, string memory key) internal returns (address[] memory);
```

### readBool


```solidity
function readBool(string memory json, string memory key) internal returns (bool);
```

### readBoolArray


```solidity
function readBoolArray(string memory json, string memory key) internal returns (bool[] memory);
```

### readBytes


```solidity
function readBytes(string memory json, string memory key) internal returns (bytes memory);
```

### readBytesArray


```solidity
function readBytesArray(string memory json, string memory key) internal returns (bytes[] memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bool value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bool[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, uint256 value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, uint256[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, int256 value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, int256[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, address value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, address[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bytes32 value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bytes32[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bytes memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, bytes[] memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, string memory value) internal returns (string memory);
```

### serialize


```solidity
function serialize(string memory jsonKey, string memory key, string[] memory value) internal returns (string memory);
```

### write


```solidity
function write(string memory jsonKey, string memory path) internal;
```

### write


```solidity
function write(string memory jsonKey, string memory path, string memory valueKey) internal;
```

