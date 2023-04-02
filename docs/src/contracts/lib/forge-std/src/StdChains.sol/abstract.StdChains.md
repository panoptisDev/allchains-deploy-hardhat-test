# StdChains
[Git Source](https://github.com/erayack/zk-sync-deploy/blob/7f3ddf5f8a514cf5569d053d7217620dd36d01c7/contracts/lib/forge-std/src/StdChains.sol)

StdChains provides information about EVM compatible chains that can be used in scripts/tests.
For each chain, the chain's name, chain ID, and a default RPC URL are provided. Chains are
identified by their alias, which is the same as the alias in the `[rpc_endpoints]` section of
the `foundry.toml` file. For best UX, ensure the alias in the `foundry.toml` file match the
alias used in this contract, which can be found as the first argument to the
`setChainWithDefaultRpcUrl` call in the `initialize` function.
There are two main ways to use this contract:
1. Set a chain with `setChain(string memory chainAlias, ChainData memory chain)` or
`setChain(string memory chainAlias, Chain memory chain)`
2. Get a chain with `getChain(string memory chainAlias)` or `getChain(uint256 chainId)`.
The first time either of those are used, chains are initialized with the default set of RPC URLs.
This is done in `initialize`, which uses `setChainWithDefaultRpcUrl`. Defaults are recorded in
`defaultRpcUrls`.
The `setChain` function is straightforward, and it simply saves off the given chain data.
The `getChain` methods use `getChainWithUpdatedRpcUrl` to return a chain. For example, let's say
we want to retrieve `mainnet`'s RPC URL:
- If you haven't set any mainnet chain info with `setChain`, you haven't specified that
chain in `foundry.toml` and no env var is set, the default data and RPC URL will be returned.
- If you have set a mainnet RPC URL in `foundry.toml` it will return that, if valid (e.g. if
a URL is given or if an environment variable is given and that environment variable exists).
Otherwise, the default data is returned.
- If you specified data with `setChain` it will return that.
Summarizing the above, the prioritization hierarchy is `setChain` -> `foundry.toml` -> environment variable -> defaults.


## State Variables
### vm

```solidity
VmSafe private constant vm = VmSafe(address(uint160(uint256(keccak256("hevm cheat code")))));
```


### initialized

```solidity
bool private initialized;
```


### chains

```solidity
mapping(string => Chain) private chains;
```


### defaultRpcUrls

```solidity
mapping(string => string) private defaultRpcUrls;
```


### idToAlias

```solidity
mapping(uint256 => string) private idToAlias;
```


### fallbackToDefaultRpcUrls

```solidity
bool private fallbackToDefaultRpcUrls = true;
```


## Functions
### getChain


```solidity
function getChain(string memory chainAlias) internal virtual returns (Chain memory chain);
```

### getChain


```solidity
function getChain(uint256 chainId) internal virtual returns (Chain memory chain);
```

### setChain


```solidity
function setChain(string memory chainAlias, ChainData memory chain) internal virtual;
```

### setChain


```solidity
function setChain(string memory chainAlias, Chain memory chain) internal virtual;
```

### _toUpper


```solidity
function _toUpper(string memory str) private pure returns (string memory);
```

### getChainWithUpdatedRpcUrl


```solidity
function getChainWithUpdatedRpcUrl(string memory chainAlias, Chain memory chain) private returns (Chain memory);
```

### setFallbackToDefaultRpcUrls


```solidity
function setFallbackToDefaultRpcUrls(bool useDefault) internal;
```

### initialize


```solidity
function initialize() private;
```

### setChainWithDefaultRpcUrl


```solidity
function setChainWithDefaultRpcUrl(string memory chainAlias, ChainData memory chain) private;
```

## Structs
### ChainData

```solidity
struct ChainData {
    string name;
    uint256 chainId;
    string rpcUrl;
}
```

### Chain

```solidity
struct Chain {
    string name;
    uint256 chainId;
    string chainAlias;
    string rpcUrl;
}
```

