# TestTest
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdAssertions.t.sol)

**Inherits:**
[Test](/contracts/lib/forge-std/src/Test.sol/abstract.Test.md)


## Functions
### expectFailure


```solidity
modifier expectFailure(bool expectFail);
```

### _fail


```solidity
function _fail(string memory err) external expectFailure(true);
```

### _assertFalse


```solidity
function _assertFalse(bool data, bool expectFail) external expectFailure(expectFail);
```

### _assertFalse


```solidity
function _assertFalse(bool data, string memory err, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(bool a, bool b, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(bool a, bool b, string memory err, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(bytes memory a, bytes memory b, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(bytes memory a, bytes memory b, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(uint256[] memory a, uint256[] memory b, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(int256[] memory a, int256[] memory b, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(address[] memory a, address[] memory b, bool expectFail) external expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(uint256[] memory a, uint256[] memory b, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(int256[] memory a, int256[] memory b, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertEq


```solidity
function _assertEq(address[] memory a, address[] memory b, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbs


```solidity
function _assertApproxEqAbs(uint256 a, uint256 b, uint256 maxDelta, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbs


```solidity
function _assertApproxEqAbs(uint256 a, uint256 b, uint256 maxDelta, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbsDecimal


```solidity
function _assertApproxEqAbsDecimal(uint256 a, uint256 b, uint256 maxDelta, uint256 decimals, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbsDecimal


```solidity
function _assertApproxEqAbsDecimal(
    uint256 a,
    uint256 b,
    uint256 maxDelta,
    uint256 decimals,
    string memory err,
    bool expectFail
) external expectFailure(expectFail);
```

### _assertApproxEqAbs


```solidity
function _assertApproxEqAbs(int256 a, int256 b, uint256 maxDelta, bool expectFail) external expectFailure(expectFail);
```

### _assertApproxEqAbs


```solidity
function _assertApproxEqAbs(int256 a, int256 b, uint256 maxDelta, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbsDecimal


```solidity
function _assertApproxEqAbsDecimal(int256 a, int256 b, uint256 maxDelta, uint256 decimals, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqAbsDecimal


```solidity
function _assertApproxEqAbsDecimal(
    int256 a,
    int256 b,
    uint256 maxDelta,
    uint256 decimals,
    string memory err,
    bool expectFail
) external expectFailure(expectFail);
```

### _assertApproxEqRel


```solidity
function _assertApproxEqRel(uint256 a, uint256 b, uint256 maxPercentDelta, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRel


```solidity
function _assertApproxEqRel(uint256 a, uint256 b, uint256 maxPercentDelta, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRelDecimal


```solidity
function _assertApproxEqRelDecimal(uint256 a, uint256 b, uint256 maxPercentDelta, uint256 decimals, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRelDecimal


```solidity
function _assertApproxEqRelDecimal(
    uint256 a,
    uint256 b,
    uint256 maxPercentDelta,
    uint256 decimals,
    string memory err,
    bool expectFail
) external expectFailure(expectFail);
```

### _assertApproxEqRel


```solidity
function _assertApproxEqRel(int256 a, int256 b, uint256 maxPercentDelta, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRel


```solidity
function _assertApproxEqRel(int256 a, int256 b, uint256 maxPercentDelta, string memory err, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRelDecimal


```solidity
function _assertApproxEqRelDecimal(int256 a, int256 b, uint256 maxPercentDelta, uint256 decimals, bool expectFail)
    external
    expectFailure(expectFail);
```

### _assertApproxEqRelDecimal


```solidity
function _assertApproxEqRelDecimal(
    int256 a,
    int256 b,
    uint256 maxPercentDelta,
    uint256 decimals,
    string memory err,
    bool expectFail
) external expectFailure(expectFail);
```

### _assertEqCall


```solidity
function _assertEqCall(
    address targetA,
    address targetB,
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory returnDataA,
    bytes memory returnDataB,
    bool strictRevertData,
    bool expectFail
) external expectFailure(expectFail);
```

