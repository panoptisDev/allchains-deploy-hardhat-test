# DemoTest
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/lib/ds-test/demo/demo.sol)

**Inherits:**
[DSTest](/contracts/lib/forge-std/lib/ds-test/src/test.sol/contract.DSTest.md)


## Functions
### test_this


```solidity
function test_this() public pure;
```

### test_logs


```solidity
function test_logs() public;
```

### test_old_logs


```solidity
function test_old_logs() public;
```

### test_trace


```solidity
function test_trace() public view;
```

### test_multiline


```solidity
function test_multiline() public;
```

### echo


```solidity
function echo(string memory s1, string memory s2) public pure returns (string memory, string memory);
```

### prove_this


```solidity
function prove_this(uint256 x) public;
```

### test_logn


```solidity
function test_logn() public;
```

### test_events


```solidity
function test_events() public;
```

### test_asserts


```solidity
function test_asserts() public;
```

## Events
### log_old_named_uint

```solidity
event log_old_named_uint(bytes32, uint256);
```

### MyEvent

```solidity
event MyEvent(uint256, uint256 indexed, uint256, uint256 indexed);
```

