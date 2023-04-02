# StdCheatsTest
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdCheats.t.sol)

**Inherits:**
[Test](/contracts/lib/forge-std/src/Test.sol/abstract.Test.md)


## State Variables
### test

```solidity
Bar test;
```


## Functions
### setUp


```solidity
function setUp() public;
```

### testSkip


```solidity
function testSkip() public;
```

### testRewind


```solidity
function testRewind() public;
```

### testHoax


```solidity
function testHoax() public;
```

### testHoaxOrigin


```solidity
function testHoaxOrigin() public;
```

### testHoaxDifferentAddresses


```solidity
function testHoaxDifferentAddresses() public;
```

### testStartHoax


```solidity
function testStartHoax() public;
```

### testStartHoaxOrigin


```solidity
function testStartHoaxOrigin() public;
```

### testChangePrankMsgSender


```solidity
function testChangePrankMsgSender() public;
```

### testChangePrankMsgSenderAndTxOrigin


```solidity
function testChangePrankMsgSenderAndTxOrigin() public;
```

### testMakeAddrEquivalence


```solidity
function testMakeAddrEquivalence() public;
```

### testMakeAddrSigning


```solidity
function testMakeAddrSigning() public;
```

### testDeal


```solidity
function testDeal() public;
```

### testDealToken


```solidity
function testDealToken() public;
```

### testDealTokenAdjustTotalSupply


```solidity
function testDealTokenAdjustTotalSupply() public;
```

### testDealERC1155Token


```solidity
function testDealERC1155Token() public;
```

### testDealERC1155TokenAdjustTotalSupply


```solidity
function testDealERC1155TokenAdjustTotalSupply() public;
```

### testDealERC721Token


```solidity
function testDealERC721Token() public;
```

### testDeployCode


```solidity
function testDeployCode() public;
```

### testDeployCodeNoArgs


```solidity
function testDeployCodeNoArgs() public;
```

### testDeployCodeVal


```solidity
function testDeployCodeVal() public;
```

### testDeployCodeValNoArgs


```solidity
function testDeployCodeValNoArgs() public;
```

### deployCodeHelper


```solidity
function deployCodeHelper(string memory what) external;
```

### testDeployCodeFail


```solidity
function testDeployCodeFail() public;
```

### getCode


```solidity
function getCode(address who) internal view returns (bytes memory o_code);
```

### testDeriveRememberKey


```solidity
function testDeriveRememberKey() public;
```

### testBytesToUint


```solidity
function testBytesToUint() public;
```

### testParseJsonTxDetail


```solidity
function testParseJsonTxDetail() public;
```

### testReadEIP1559Transaction


```solidity
function testReadEIP1559Transaction() public view;
```

### testReadEIP1559Transactions


```solidity
function testReadEIP1559Transactions() public view;
```

### testReadReceipt


```solidity
function testReadReceipt() public;
```

### testReadReceipts


```solidity
function testReadReceipts() public view;
```

### testGasMeteringModifier


```solidity
function testGasMeteringModifier() public;
```

### addInLoop


```solidity
function addInLoop() internal pure returns (uint256);
```

### addInLoopNoGas


```solidity
function addInLoopNoGas() internal noGasMetering returns (uint256);
```

### addInLoopNoGasNoGas


```solidity
function addInLoopNoGasNoGas() internal noGasMetering returns (uint256);
```

### bytesToUint_test


```solidity
function bytesToUint_test(bytes memory b) private pure returns (uint256);
```

### testAssumeNoPrecompiles


```solidity
function testAssumeNoPrecompiles(address addr) external;
```

### testAssumePayable


```solidity
function testAssumePayable() external;
```

### testAssumePayable


```solidity
function testAssumePayable(address addr) external;
```

