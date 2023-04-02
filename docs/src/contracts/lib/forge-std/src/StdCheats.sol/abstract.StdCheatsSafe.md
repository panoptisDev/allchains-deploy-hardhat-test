# StdCheatsSafe
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/src/StdCheats.sol)


## State Variables
### vm

```solidity
Vm private constant vm = Vm(address(uint160(uint256(keccak256("hevm cheat code")))));
```


### gasMeteringOff

```solidity
bool private gasMeteringOff;
```


## Functions
### assumeNoPrecompiles


```solidity
function assumeNoPrecompiles(address addr) internal virtual;
```

### assumeNoPrecompiles


```solidity
function assumeNoPrecompiles(address addr, uint256 chainId) internal pure virtual;
```

### readEIP1559ScriptArtifact


```solidity
function readEIP1559ScriptArtifact(string memory path) internal view virtual returns (EIP1559ScriptArtifact memory);
```

### rawToConvertedEIPTx1559s


```solidity
function rawToConvertedEIPTx1559s(RawTx1559[] memory rawTxs) internal pure virtual returns (Tx1559[] memory);
```

### rawToConvertedEIPTx1559


```solidity
function rawToConvertedEIPTx1559(RawTx1559 memory rawTx) internal pure virtual returns (Tx1559 memory);
```

### rawToConvertedEIP1559Detail


```solidity
function rawToConvertedEIP1559Detail(RawTx1559Detail memory rawDetail)
    internal
    pure
    virtual
    returns (Tx1559Detail memory);
```

### readTx1559s


```solidity
function readTx1559s(string memory path) internal view virtual returns (Tx1559[] memory);
```

### readTx1559


```solidity
function readTx1559(string memory path, uint256 index) internal view virtual returns (Tx1559 memory);
```

### readReceipts


```solidity
function readReceipts(string memory path) internal view virtual returns (Receipt[] memory);
```

### readReceipt


```solidity
function readReceipt(string memory path, uint256 index) internal view virtual returns (Receipt memory);
```

### rawToConvertedReceipts


```solidity
function rawToConvertedReceipts(RawReceipt[] memory rawReceipts) internal pure virtual returns (Receipt[] memory);
```

### rawToConvertedReceipt


```solidity
function rawToConvertedReceipt(RawReceipt memory rawReceipt) internal pure virtual returns (Receipt memory);
```

### rawToConvertedReceiptLogs


```solidity
function rawToConvertedReceiptLogs(RawReceiptLog[] memory rawLogs)
    internal
    pure
    virtual
    returns (ReceiptLog[] memory);
```

### deployCode


```solidity
function deployCode(string memory what, bytes memory args) internal virtual returns (address addr);
```

### deployCode


```solidity
function deployCode(string memory what) internal virtual returns (address addr);
```

### deployCode

*deploy contract with value on construction*


```solidity
function deployCode(string memory what, bytes memory args, uint256 val) internal virtual returns (address addr);
```

### deployCode


```solidity
function deployCode(string memory what, uint256 val) internal virtual returns (address addr);
```

### makeAddrAndKey


```solidity
function makeAddrAndKey(string memory name) internal virtual returns (address addr, uint256 privateKey);
```

### makeAddr


```solidity
function makeAddr(string memory name) internal virtual returns (address addr);
```

### deriveRememberKey


```solidity
function deriveRememberKey(string memory mnemonic, uint32 index)
    internal
    virtual
    returns (address who, uint256 privateKey);
```

### _bytesToUint


```solidity
function _bytesToUint(bytes memory b) private pure returns (uint256);
```

### isFork


```solidity
function isFork() internal view virtual returns (bool status);
```

### skipWhenForking


```solidity
modifier skipWhenForking();
```

### skipWhenNotForking


```solidity
modifier skipWhenNotForking();
```

### noGasMetering


```solidity
modifier noGasMetering();
```

### assumePayable


```solidity
function assumePayable(address addr) internal virtual;
```

## Structs
### RawTx1559

```solidity
struct RawTx1559 {
    string[] arguments;
    address contractAddress;
    string contractName;
    string functionSig;
    bytes32 hash;
    RawTx1559Detail txDetail;
    string opcode;
}
```

### RawTx1559Detail

```solidity
struct RawTx1559Detail {
    AccessList[] accessList;
    bytes data;
    address from;
    bytes gas;
    bytes nonce;
    address to;
    bytes txType;
    bytes value;
}
```

### Tx1559

```solidity
struct Tx1559 {
    string[] arguments;
    address contractAddress;
    string contractName;
    string functionSig;
    bytes32 hash;
    Tx1559Detail txDetail;
    string opcode;
}
```

### Tx1559Detail

```solidity
struct Tx1559Detail {
    AccessList[] accessList;
    bytes data;
    address from;
    uint256 gas;
    uint256 nonce;
    address to;
    uint256 txType;
    uint256 value;
}
```

### TxLegacy

```solidity
struct TxLegacy {
    string[] arguments;
    address contractAddress;
    string contractName;
    string functionSig;
    string hash;
    string opcode;
    TxDetailLegacy transaction;
}
```

### TxDetailLegacy

```solidity
struct TxDetailLegacy {
    AccessList[] accessList;
    uint256 chainId;
    bytes data;
    address from;
    uint256 gas;
    uint256 gasPrice;
    bytes32 hash;
    uint256 nonce;
    bytes1 opcode;
    bytes32 r;
    bytes32 s;
    uint256 txType;
    address to;
    uint8 v;
    uint256 value;
}
```

### AccessList

```solidity
struct AccessList {
    address accessAddress;
    bytes32[] storageKeys;
}
```

### RawReceipt

```solidity
struct RawReceipt {
    bytes32 blockHash;
    bytes blockNumber;
    address contractAddress;
    bytes cumulativeGasUsed;
    bytes effectiveGasPrice;
    address from;
    bytes gasUsed;
    RawReceiptLog[] logs;
    bytes logsBloom;
    bytes status;
    address to;
    bytes32 transactionHash;
    bytes transactionIndex;
}
```

### Receipt

```solidity
struct Receipt {
    bytes32 blockHash;
    uint256 blockNumber;
    address contractAddress;
    uint256 cumulativeGasUsed;
    uint256 effectiveGasPrice;
    address from;
    uint256 gasUsed;
    ReceiptLog[] logs;
    bytes logsBloom;
    uint256 status;
    address to;
    bytes32 transactionHash;
    uint256 transactionIndex;
}
```

### EIP1559ScriptArtifact

```solidity
struct EIP1559ScriptArtifact {
    string[] libraries;
    string path;
    string[] pending;
    Receipt[] receipts;
    uint256 timestamp;
    Tx1559[] transactions;
    TxReturn[] txReturns;
}
```

### RawEIP1559ScriptArtifact

```solidity
struct RawEIP1559ScriptArtifact {
    string[] libraries;
    string path;
    string[] pending;
    RawReceipt[] receipts;
    TxReturn[] txReturns;
    uint256 timestamp;
    RawTx1559[] transactions;
}
```

### RawReceiptLog

```solidity
struct RawReceiptLog {
    address logAddress;
    bytes32 blockHash;
    bytes blockNumber;
    bytes data;
    bytes logIndex;
    bool removed;
    bytes32[] topics;
    bytes32 transactionHash;
    bytes transactionIndex;
    bytes transactionLogIndex;
}
```

### ReceiptLog

```solidity
struct ReceiptLog {
    address logAddress;
    bytes32 blockHash;
    uint256 blockNumber;
    bytes data;
    uint256 logIndex;
    bytes32[] topics;
    uint256 transactionIndex;
    uint256 transactionLogIndex;
    bool removed;
}
```

### TxReturn

```solidity
struct TxReturn {
    string internalType;
    string value;
}
```

