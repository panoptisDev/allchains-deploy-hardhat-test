# StdAssertionsTest
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/test/StdAssertions.t.sol)

**Inherits:**
[Test](/contracts/lib/forge-std/src/Test.sol/abstract.Test.md)


## State Variables
### CUSTOM_ERROR

```solidity
string constant CUSTOM_ERROR = "guh!";
```


### EXPECT_PASS

```solidity
bool constant EXPECT_PASS = false;
```


### EXPECT_FAIL

```solidity
bool constant EXPECT_FAIL = true;
```


### SHOULD_REVERT

```solidity
bool constant SHOULD_REVERT = true;
```


### SHOULD_RETURN

```solidity
bool constant SHOULD_RETURN = false;
```


### STRICT_REVERT_DATA

```solidity
bool constant STRICT_REVERT_DATA = true;
```


### NON_STRICT_REVERT_DATA

```solidity
bool constant NON_STRICT_REVERT_DATA = false;
```


### t

```solidity
TestTest t = new TestTest();
```


## Functions
### testShouldFail


```solidity
function testShouldFail() external;
```

### testAssertFalse_Pass


```solidity
function testAssertFalse_Pass() external;
```

### testAssertFalse_Fail


```solidity
function testAssertFalse_Fail() external;
```

### testAssertFalse_Err_Pass


```solidity
function testAssertFalse_Err_Pass() external;
```

### testAssertFalse_Err_Fail


```solidity
function testAssertFalse_Err_Fail() external;
```

### testAssertEq_Bool_Pass


```solidity
function testAssertEq_Bool_Pass(bool a) external;
```

### testAssertEq_Bool_Fail


```solidity
function testAssertEq_Bool_Fail(bool a, bool b) external;
```

### testAssertEq_BoolErr_Pass


```solidity
function testAssertEq_BoolErr_Pass(bool a) external;
```

### testAssertEq_BoolErr_Fail


```solidity
function testAssertEq_BoolErr_Fail(bool a, bool b) external;
```

### testAssertEq_Bytes_Pass


```solidity
function testAssertEq_Bytes_Pass(bytes calldata a) external;
```

### testAssertEq_Bytes_Fail


```solidity
function testAssertEq_Bytes_Fail(bytes calldata a, bytes calldata b) external;
```

### testAssertEq_BytesErr_Pass


```solidity
function testAssertEq_BytesErr_Pass(bytes calldata a) external;
```

### testAssertEq_BytesErr_Fail


```solidity
function testAssertEq_BytesErr_Fail(bytes calldata a, bytes calldata b) external;
```

### testAssertEq_UintArr_Pass


```solidity
function testAssertEq_UintArr_Pass(uint256 e0, uint256 e1, uint256 e2) public;
```

### testAssertEq_IntArr_Pass


```solidity
function testAssertEq_IntArr_Pass(int256 e0, int256 e1, int256 e2) public;
```

### testAssertEq_AddressArr_Pass


```solidity
function testAssertEq_AddressArr_Pass(address e0, address e1, address e2) public;
```

### testAssertEq_UintArr_FailEl


```solidity
function testAssertEq_UintArr_FailEl(uint256 e1) public;
```

### testAssertEq_IntArr_FailEl


```solidity
function testAssertEq_IntArr_FailEl(int256 e1) public;
```

### testAssertEq_AddressArr_FailEl


```solidity
function testAssertEq_AddressArr_FailEl(address e1) public;
```

### testAssertEq_UintArrErr_FailEl


```solidity
function testAssertEq_UintArrErr_FailEl(uint256 e1) public;
```

### testAssertEq_IntArrErr_FailEl


```solidity
function testAssertEq_IntArrErr_FailEl(int256 e1) public;
```

### testAssertEq_AddressArrErr_FailEl


```solidity
function testAssertEq_AddressArrErr_FailEl(address e1) public;
```

### testAssertEq_UintArr_FailLen


```solidity
function testAssertEq_UintArr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEq_IntArr_FailLen


```solidity
function testAssertEq_IntArr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEq_AddressArr_FailLen


```solidity
function testAssertEq_AddressArr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEq_UintArrErr_FailLen


```solidity
function testAssertEq_UintArrErr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEq_IntArrErr_FailLen


```solidity
function testAssertEq_IntArrErr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEq_AddressArrErr_FailLen


```solidity
function testAssertEq_AddressArrErr_FailLen(uint256 lenA, uint256 lenB) public;
```

### testAssertEqUint


```solidity
function testAssertEqUint() public;
```

### testFailAssertEqUint


```solidity
function testFailAssertEqUint() public;
```

### testAssertApproxEqAbs_Uint_Pass


```solidity
function testAssertApproxEqAbs_Uint_Pass(uint256 a, uint256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_Uint_Fail


```solidity
function testAssertApproxEqAbs_Uint_Fail(uint256 a, uint256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_UintErr_Pass


```solidity
function testAssertApproxEqAbs_UintErr_Pass(uint256 a, uint256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_UintErr_Fail


```solidity
function testAssertApproxEqAbs_UintErr_Fail(uint256 a, uint256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbsDecimal_Uint_Pass


```solidity
function testAssertApproxEqAbsDecimal_Uint_Pass(uint256 a, uint256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_Uint_Fail


```solidity
function testAssertApproxEqAbsDecimal_Uint_Fail(uint256 a, uint256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_UintErr_Pass


```solidity
function testAssertApproxEqAbsDecimal_UintErr_Pass(uint256 a, uint256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_UintErr_Fail


```solidity
function testAssertApproxEqAbsDecimal_UintErr_Fail(uint256 a, uint256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbs_Int_Pass


```solidity
function testAssertApproxEqAbs_Int_Pass(int256 a, int256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_Int_Fail


```solidity
function testAssertApproxEqAbs_Int_Fail(int256 a, int256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_IntErr_Pass


```solidity
function testAssertApproxEqAbs_IntErr_Pass(int256 a, int256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbs_IntErr_Fail


```solidity
function testAssertApproxEqAbs_IntErr_Fail(int256 a, int256 b, uint256 maxDelta) external;
```

### testAssertApproxEqAbsDecimal_Int_Pass


```solidity
function testAssertApproxEqAbsDecimal_Int_Pass(int256 a, int256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_Int_Fail


```solidity
function testAssertApproxEqAbsDecimal_Int_Fail(int256 a, int256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_IntErr_Pass


```solidity
function testAssertApproxEqAbsDecimal_IntErr_Pass(int256 a, int256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqAbsDecimal_IntErr_Fail


```solidity
function testAssertApproxEqAbsDecimal_IntErr_Fail(int256 a, int256 b, uint256 maxDelta, uint256 decimals) external;
```

### testAssertApproxEqRel_Uint_Pass


```solidity
function testAssertApproxEqRel_Uint_Pass(uint256 a, uint256 b, uint256 maxPercentDelta) external;
```

### testAssertApproxEqRel_Uint_Fail


```solidity
function testAssertApproxEqRel_Uint_Fail(uint256 a, uint256 b, uint256 maxPercentDelta) external;
```

### testAssertApproxEqRel_UintErr_Pass


```solidity
function testAssertApproxEqRel_UintErr_Pass(uint256 a, uint256 b, uint256 maxPercentDelta) external;
```

### testAssertApproxEqRel_UintErr_Fail


```solidity
function testAssertApproxEqRel_UintErr_Fail(uint256 a, uint256 b, uint256 maxPercentDelta) external;
```

### testAssertApproxEqRelDecimal_Uint_Pass


```solidity
function testAssertApproxEqRelDecimal_Uint_Pass(uint256 a, uint256 b, uint256 maxPercentDelta, uint256 decimals)
    external;
```

### testAssertApproxEqRelDecimal_Uint_Fail


```solidity
function testAssertApproxEqRelDecimal_Uint_Fail(uint256 a, uint256 b, uint256 maxPercentDelta, uint256 decimals)
    external;
```

### testAssertApproxEqRelDecimal_UintErr_Pass


```solidity
function testAssertApproxEqRelDecimal_UintErr_Pass(uint256 a, uint256 b, uint256 maxPercentDelta, uint256 decimals)
    external;
```

### testAssertApproxEqRelDecimal_UintErr_Fail


```solidity
function testAssertApproxEqRelDecimal_UintErr_Fail(uint256 a, uint256 b, uint256 maxPercentDelta, uint256 decimals)
    external;
```

### testAssertApproxEqRel_Int_Pass


```solidity
function testAssertApproxEqRel_Int_Pass(int128 a, int128 b, uint128 maxPercentDelta) external;
```

### testAssertApproxEqRel_Int_Fail


```solidity
function testAssertApproxEqRel_Int_Fail(int128 a, int128 b, uint128 maxPercentDelta) external;
```

### testAssertApproxEqRel_IntErr_Pass


```solidity
function testAssertApproxEqRel_IntErr_Pass(int128 a, int128 b, uint128 maxPercentDelta) external;
```

### testAssertApproxEqRel_IntErr_Fail


```solidity
function testAssertApproxEqRel_IntErr_Fail(int128 a, int128 b, uint128 maxPercentDelta) external;
```

### testAssertApproxEqRelDecimal_Int_Pass


```solidity
function testAssertApproxEqRelDecimal_Int_Pass(int128 a, int128 b, uint128 maxPercentDelta, uint128 decimals)
    external;
```

### testAssertApproxEqRelDecimal_Int_Fail


```solidity
function testAssertApproxEqRelDecimal_Int_Fail(int128 a, int128 b, uint128 maxPercentDelta, uint128 decimals)
    external;
```

### testAssertApproxEqRelDecimal_IntErr_Pass


```solidity
function testAssertApproxEqRelDecimal_IntErr_Pass(int128 a, int128 b, uint128 maxPercentDelta, uint128 decimals)
    external;
```

### testAssertApproxEqRelDecimal_IntErr_Fail


```solidity
function testAssertApproxEqRelDecimal_IntErr_Fail(int128 a, int128 b, uint128 maxPercentDelta, uint128 decimals)
    external;
```

### testAssertEqCall_Return_Pass


```solidity
function testAssertEqCall_Return_Pass(
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory returnData,
    bool strictRevertData
) external;
```

### testAssertEqCall_Return_Fail


```solidity
function testAssertEqCall_Return_Fail(
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory returnDataA,
    bytes memory returnDataB,
    bool strictRevertData
) external;
```

### testAssertEqCall_Revert_Pass


```solidity
function testAssertEqCall_Revert_Pass(
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory revertDataA,
    bytes memory revertDataB
) external;
```

### testAssertEqCall_Revert_Fail


```solidity
function testAssertEqCall_Revert_Fail(
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory revertDataA,
    bytes memory revertDataB
) external;
```

### testAssertEqCall_Fail


```solidity
function testAssertEqCall_Fail(
    bytes memory callDataA,
    bytes memory callDataB,
    bytes memory returnDataA,
    bytes memory returnDataB,
    bool strictRevertData
) external;
```

